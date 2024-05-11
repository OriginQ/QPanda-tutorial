Change Log
>>>>>>>>>>>>>>>>>>>>>>>>

2.8 - 2024-5-1
********

**新增功能和重要更新：**

1.本源量子云计算服务有较大更新升级，主要包括以下内容

    - **（1）量子计算服务适配了本源悟空芯片上线** ， 对应的 ``RealChipType::ORIGIN_72`` 即为72比特芯片类型。

    - **（2）量子云虚拟机添加了批量任务提交** ，目前仅可用于芯片任务的批量任务提交。

        .. code-block:: c
            
            #include "QPanda.h"
            USING_QPANDA

            int main(void)
            {

                //替换为自己的apikey
                std::string api_key = "XXXXX";

                auto machine = QCloudMachine();
                machine.setConfigure({ 72,72 });

                //online
                machine.init(online_api_key, true, true, false);

                auto q = machine.qAllocMany(6);
                auto c = machine.cAllocMany(6);

                std::vector<QProg> prog_array;

                for (size_t i = 0; i < 2; i++)
                {
                    auto measure_prog = QProg();
                    measure_prog 
                        << H(q[0]) 
                        << CNOT(q[0], q[1]) 
                        << CNOT(q[1], q[2])
                        << Measure(q[0], c[0]) 
                        << Measure(q[1], c[1]);

                    prog_array.emplace_back(measure_prog);
                }

                auto prog = QProg();
                prog << H(q[1]) << Measure(q[1], c[0]);

                auto batch_result = machine.batch_real_chip_measure(prog_array, 1000, RealChipType::ORIGIN_72);
                for (auto val : batch_result)
                {
                    for (auto single_item : val)
                        cout << single_item.first << " : " << single_item.second << endl;
                }
            }

    -  **（3）本源量子云计算服务新增了混合加密配置使用选项**，用于对量子计算任务传输和通信中的任务数据开启 **混合加密** 从而保护数据安全和隐私，可以根据需要选择开启或打开。

        开启方式为：将 **QCloud** 初始化函数的参数 ``enable_pqc_encryption`` 设置为 ``true`` 即可，默认为 ``False`` 不开启。

        .. code-block:: c

            #include "QPanda.h"
            USING_QPANDA

            int main(void)
            {
                //替换为自己的apikey
                std::string api_key = "XXXXX";

                auto machine = QCloudMachine();
                machine.setConfigure({ 72,72 });

                //online
                machine.init(online_api_key, true, true, false);
            }

        当今，随着量子计算机在硬件技术、纠错方法、算法理论与应用等多个维度的不断进步，传统的公钥算法由于无法抵御量子计算机的攻击逐渐变得脆弱，面临着被未来量子计算机攻击的风险。为了提供更强大的安全保护，本源量子云平台引入了一种端到端的 **后量子(PQC)混合加密** 方法，以保护云服务的用户端和服务端之间的信息传输，在有效抵御量子计算机的各种攻击的同时考虑了现有后量子密码极低但潜在的风险，并借助融合传统公钥密钥(RSA类、ECC类)算法规避了这一隐患。

        **混合加密**： 混合加密是一种结合了两种密码算法的模式，该模式或部分或完整地继承各部分密码模块的某些特性，用于混合的两个功能相近的算法可以均为经典密码算法，也可以同时来自PQC。考虑到现有公钥密码算法面对量子计算机的脆弱性以及现阶段PQC算法潜在的风险，混合算法的两部分“原料”一般一半来自经典，一半来自PQC。例如，苹果于最近推出的iMessage加密方案以及谷歌在其浏览器中部署的混合加密方案均为Kyber(PQC的一种)与ECC类算法的混合。

        本源量子云采用的混合加密方法来自NIST将要形成标准的 ``格基密码算法Kyber`` 以及 ``ECC类算法`` ，并且在具体的实现过程中尽量采用国家认证的SM系列算法，例如，ECC类算法选取SM2算法，混合流程中用以密钥导出的函数(KDF)选用SM3算法，建立会话密钥后后续加解密采用SM4算法，并使用了安全度较高的CBC模式。

    - **（4）初始化混合加密配置新增了指定随机数功能** ，用于对量子计算任务传输和通信中的数据加密过程添加用户指定的随机数。

        设置方式为将 **QCloud** 初始化函数的参数 ``enable_pqc_encryption`` 设置为 ``true`` 即可，默认为 ``false`` 不开启，同时可以传入用户指定的随机数，接受 **192字符大小的16进制字符串** ，如果参数长度不符合要求，内部会自动进行处理。

        .. code-block:: c

            
            #include "QPanda.h"
            USING_QPANDA

            int main(void)
            {
                //替换为自己的apikey
                std::string api_key = "XXXXX";

                auto machine = QCloudMachine();
                machine.setConfigure({ 72,72 });

                //online
                machine.init(online_api_key, true, true, "xxx"); //参数为随机16进制字符串
            }

    - **（5）量子云计算服务芯片任务添加了相关限制** ，单个任务的层数不能超过 **500** 层，并且单门控制比特数量不能超过 **2** 个（Toffoli门除外），双门不支持添加控制比特，如果量子线路中有相关计算需求，需要先调用多控门分解接口 **ldd_decompose** ，参考如下代码：

2.ldd多控门分解接口( ``ldd_decompose`` )适配了RXX,RYY,RZX,RZZ,MS等特殊双门以及 ``QOracle`` 的受控形式，示例程序如下

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            CPUQVM machine;
            machine.init();

            auto q = machine.qAllocMany(5);
            auto c = machine.cAllocMany(5);

            auto tar_qubits = QVec{ q[0], q[1], q[2] };
            auto ctr_qubits = QVec{ q[3], q[4] };

            auto rand_circuit = random_qcircuit(tar_qubits, 10);
            auto rand_prog = QProg(rand_circuit);

            auto rand_matrix = get_unitary(rand_prog);

            QProg prog;
            prog << X(q[3]) << X(q[4])
                << RX(q[0], 1)
                << MS(q[0], q[1]).control(ctr_qubits)
                << RXX(q[0], q[1], 1).control(ctr_qubits)
                << RYY(q[0], q[1], 2).control(ctr_qubits)
                << RZZ(q[0], q[1], 3).control(ctr_qubits)
                << RZX(q[0], q[1], 4).control(ctr_qubits)
                << QOracle(tar_qubits, rand_matrix).control(ctr_qubits);

            machine.directlyRun(prog);
            auto origin_state = machine.getQState();

            auto ldd_prog = ldd_decompose(prog);
            machine.initState();
            machine.directlyRun(ldd_prog);
            auto ldd_state = machine.getQState();

            for (auto val : origin_state)
                std::cout << val << endl;

            std::cout << "================" << endl;

            for (auto val : ldd_state)
                std::cout << val << endl;

            std::cout << prog << endl;
            std::cout << ldd_prog << endl;

            if (state_compare(origin_state, ldd_state))
                cout << "Test Ldd Decompose Multi Control Oracle Passed." << endl;
            else
                cout << "Test Ldd Decompose Multi Control Oracle Failed." << endl;

            return;
        }

3.新增了稀疏态量子态初态接口 **initSparseState** ，参数为 **std::map<std::string, qcomplex_t>** 和 **QVec** 用于稀疏方式进行初态制备，需要满足初态归一化条件，代码示例：

4.虚拟机计算模拟和originir指令添加了Mlmer–Srensen"逻辑门（MS门）

    .. code-block:: c

        auto gate = MS(q[0], q[1]);

5.基于Clifford的 ``stabilizer`` 模拟器添加了噪声模拟，目前仅支持比特翻转,相位反转,比特相位反转,去极化以及相位阻尼这五个噪声模型，具体可以参考下面的代码和 :ref:`Stabilizer` 中的接口介绍。

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            Stabilizer simulator;
            simulator.init();

            auto q = simulator.qAllocMany(6);
            auto c = simulator.cAllocMany(6);

            simulator.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, GateType::PAULI_X_GATE, 0.5);

            auto prog = QProg();
            prog<< X(q[0])
                << X(q[1])
                << X(q[2])
                << X(q[3])
                << X(q[4])
                << X(q[5])
                << Measure(q[0], c[0])
                << Measure(q[1], c[1])
                << Measure(q[2], c[2]);

            auto result = simulator.runWithConfiguration(prog, 1000);

            for (auto val : result)
            {
                std::cout << val.first << " : " << val.second << std::endl;
            }

            return;
        }

6. 密度矩阵噪声设置现在可以正确叠加，参考如下代码:
   
    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            DensityMatrixSimulator simulator;
            simulator.init();

            auto q = simulator.qAllocMany(6);
            auto c = simulator.cAllocMany(6);

            auto prog = QProg();
            prog << H(q[0]) << H(q[1]) << H(q[2]) << H(q[3]) << H(q[4]) << H(q[5]);
            prog << T(q[0]);
            prog << S(q[1]);
            prog << X(q[1]);
            prog << Y(q[0]);
            prog << Z(q[1]);
            prog << U1(q[1], 1);
            prog << RX(q[1], -1);
            prog << RY(q[1], -1);
            prog << RZ(q[1], -1);
            prog << CZ(q[4], q[5]);
            prog << CNOT(q[0], q[1]);
            prog << SWAP(q[0], q[5]);
            prog << iSWAP(q[1], q[4]);
            prog << Toffoli(q[0], q[1], q[2]);
            prog << RXX(q[1], q[3], 10);
            prog << RYY(q[1], q[3], 10);
            prog << RZZ(q[1], q[3], 10);
            prog << RZX(q[1], q[3], 10);

            auto density_matrix = simulator.get_density_matrix(prog);

            const QVec noise_qubits = { q[0] };
            simulator.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, { GateType::PAULI_X_GATE, GateType::HADAMARD_GATE }, 0.5);
            simulator.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, { GateType::T_GATE }, 0.5, noise_qubits);
            simulator.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, { GateType::CNOT_GATE }, 0.5);

            std::vector<QVec> qnum_qubits = { {q[0], q[1], q[2]} };
            simulator.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, GateType::PAULI_X_GATE, 0.5, qnum_qubits);
            prob_vec probs = simulator.get_probabilities(prog);

            return;
        }

7. ClassicalCondition添加c_and、c_or、c_not功能，用于构建量子逻辑分支程序时实现复杂的表达式判断，可以参考下面的代码

**修复和解决的问题：**

1.修复了ISWAP的dagger形式在多个虚拟机下的计算结果错误

2.修复量子态编码中关于复数数据重载函数在python中调用出现丢失虚部，导致只索引double类型接口错误。

3.解决某些使用GPU虚拟机情况下，cuda与Eigen3的运行冲突问题

4.修改了经典寄存器部分情况下有误，造成无法使用qif和qwhile的问题

5.优化了量子线路映射和转化过程中的错误
   
6.解决CPUQVM部分初始化和虚拟机释放场景下使用引入的内存泄漏问题  
   
7.解决了部分映射接口在使用时异常出现程序崩溃和死循环的错误

8.修改了所有模拟器可能在计算含有BARRIER的量子程序过程中出错的问题

9.解决控制swap逻辑门，进行多控门分解时，控制信息丢失问题

10.解决单个比特在释放时(qFree接口)程序异常退出的严重性bug

11.修复了qasm相关指令集转化接口，在重复调用时比特重复申请的异常

12.修复量子虚拟机set_configure设置与init的冲突，该问题会导致部分情况下的内存泄露

13.修改了量子虚拟机初始化错误，该错误会导致多个量子虚拟机重复初始化过程引发未知异常，涉及到的虚拟机有张量网络虚拟机,部分振幅虚拟机，单振幅虚拟机，密度矩阵模拟器和Clifford模拟器等

14.修改了量子比特池初始化和清空操作不彻底的错误，该错误会导致清空后设置最大容量时内存异常

15.解决了部分情况下由于全局虚拟机导致的originir转换异常

16.修改了量子云计算服务12进制与二进制转换未正确生效以及结果前后不一致的问题

17..修改了几处由于C++17升级导致的GPU量子虚拟机运行异常错误

2.7.17 - 2023-5-22
********

新增功能和重要更新
===================

1.新增 ``Clifford模拟器`` ，主要用于基础量子纠错场景以及高比特且稀疏的Clifford门集构成的量子线路模拟，具体接口可以参考 :ref:`Stabilizer` 。 

2.量子云虚拟机相关更新

    （1）为了适配了新版本的本源量子云平台做了相关改动，对每个用户的认证标识符做了签名加密处理，但接口使用方式与之前相同
    （2）完善相关的错误处理，现在出错和异常信息输出更加具体明确

3.新增Pauli算符与矩阵的转化接口，通过矩阵转换Pauli算符接口名为 ``matrix_decompose_hamiltonian`` ,示例如下：

    .. code-block:: c

        auto matrix = EigenMatrixX(4, 4);
        auto hamiltonian = matrix_decompose_hamiltonian(matrix);
        std::cout << hamiltonian << endl;

4.提供一种利用矩阵乘积态（MPS）的低秩表达近似分布振幅制备算法，可以通过一种较少的CNOT的门完成对分布振幅的表达，并且这种表达是一种近邻接形式，因此可以直接作用于芯片，由于双门个数的减少，也有利于增加分布制备的成功率。

5.Pauli算符的构造函数现在提供可选参数，用于决定是否合并同类项，同时也可以显式调用手动合并函数

    .. code-block:: c

        //默认不合并同类项
        auto opt = PauliOperator({ {"X0 Y2",-0.044750},
                                    {"Z0 Z1",0.189766},
                                    {"Z1 Z0",0.270597},
                                    {"Z3",-0.242743 } });

        std::cout << opt << endl;

        //合并同类项
        auto opt1 = PauliOperator({ {"X0 Y2",-0.044750},
                                    {"Z0 Z1",0.189766},
                                    {"Z1 Z0",0.270597},
                                    {"Z3",-0.242743 } }, true);

        std::cout << opt1 << endl;

        //手动合并
        opt.reduceDuplicates();

        std::cout << opt1 << endl;

    输出结果如下：

    .. code-block:: c


        //默认不合并同类项
        {
            "X0 Y2" : -0.044750,
            "Z0 Z1" : 0.189766,
            "Z0 Z1" : 0.270597,
            "Z3" : -0.242743
        }

        //合并同类项
        {
            "X0 Y2" : -0.044750,
            "Z0 Z1" : 0.460363,
            "Z3" : -0.242743
        }

        //手动合并
        {
            "X0 Y2" : -0.044750,
            "Z0 Z1" : 0.460363,
            "Z3" : -0.242743
        }

    上述可选合并默认参数的使用方式适用于以下Pauli算符的构造函数

    .. code-block:: c

        auto operator1 = pq.PauliOperator({{"X0 X1",-0.044750}, {"Z0 Z1",0.189766}}, true);
        auto operator2 = PauliOperator(EigenMatrixX(2,2), true);
        auto operator3 = pq.PauliOperator("X0 X1", 0.122, true);

其他更新
========

1.修复在某些情况下，GPU虚拟机无法在linux下运行的问题

2.修复QPanda画量子线路时，Barrier门会出现比特和图像不符的现象

3.在编译优化方面，解决了高深度量子线路编译时，偶尔出现的内存崩溃问题

4.修复部分振幅虚拟机，分解Toffoli门和CU门无法正确识别分解结果的问题，现在部分振幅虚拟机对全部的单双门和Toffoli门均有很好地支持

5.噪声虚拟机添加线程数量控制

6.解决密度矩阵噪声在算符类噪声施加比特参数的错误

2.7.16 - 2023-1-12
********

新增功能
========

1.新增密度矩阵模拟器，适用于小型量子系统下的密度矩阵模拟，同时提供约化密度矩阵，概率分布，哈密顿量期望以及噪声线路模拟等接口，具体可以参考 :ref:`密度矩阵模拟器` 。 

2.优化了泡利算符的构造方式，新增了通过矩阵来构造泡利算符的接口。

3.优化了泡利算符的构造方式，新增了形如 ``auto operator = 1.5 * x(0) + 0.6 * y(1) + 2.1 * z(2)`` 的更简洁的构造方式。

4.单振幅虚拟机添加获取对应振幅接口。

其他更新
========

1.修复在只有measure线路等情况下，输出latex信息显示和转换失败的问题。

2.更新变分组件，添加三角函数相关接口。

3.优化了获取矩阵接口，添加了量子比特可选参数，可以获取一个量子线路中指定比特对应的矩阵。

4.修复退相干噪声计算错误的问题。

5.修复某些情况下GPU模拟器运行错误问题。

6.修复ISWAP门默认参数未统一的问题。

7.删除Encode类中归一化函数，并修改为入参检测归一化。