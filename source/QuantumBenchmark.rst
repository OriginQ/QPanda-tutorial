
量子基准评测
==========================

量子体积基准简介
--------------
量子体积（\ **Quantum
Volume**\ ），是一个用于评估量子计算系统性能的协议。它表示可以在系统上执行的最大等宽度深度的随机线路。量子计算系统的操作保真度越高，关联性越高，有越大的校准过的门操作集合便会有越高的量子体积。量子体积与系统的整体性能相关联，即与系统的整体错误率，潜在的物理比特关联和门操作并行度相联系。总的来说，量子体积是一个用于近期整体评估量子计算系统的一个实用方法，数值越高，系统整体错误率就越低，性能就越好。

测量量子体积的标准做法就是对系统使用规定的量子线路模型执行随机的线路操作，尽可能地将比特纠缠在一起，然后再将实验得到的结果与模拟的结果进行比较。按要求分析统计结果。

量子体积被定义为指数形式：

.. math::


   V_Q=2^n

，其中n表示在给定比特数目m（m大于n）和完成计算任务的条件下，系统操作的最大逻辑深度，如果芯片能执行的最大逻辑深度n大于比特数m，那么系统的量子体积就是

.. math::


   2^m


接口说明
--------------
``calculate_quantum_volume``
输入参数分别噪声虚拟机或者量子云机器，待测量的量子比特，随机迭代次数，测量次数
。输出为 ``size_t`` 数据，为量子体积大小。

实例
--------------
.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA
    int main()
    {
        // 构建噪声虚拟机，设置噪声参数
        auto qvm = new NoiseQVM();
        qvm->init();
        qvm->set_noise_model(NOISE_MODEL::DEPOLARIZING_KRAUS_OPERATOR, CZ_GATE, 0.005);

        // 同样可以申请云计算机器（采用真实芯片），采用真实芯片要考虑芯片构造
        //auto qvm = new QCloudMachine();
        //qvm->init("898D47CF515A48CEAA9F2326394B85C6")

        // 构建待测量的量子比特组合， 这里比特组合为2组，其中 量子比特3、4为一组；量子比特2，3，5为一组
        std::vector <std::vector<int> >qubit_lists = { {3,4}, {2,3,5} };

        // 设置随机迭代次数
        int ntrials = 100;

        // 设置测量次数,即真实芯片或者噪声虚拟机shots数值
        int shots = 4000;

        // 测量量子体积
        auto qv_result = calculate_quantum_volume(qvm, qubit_lists, ntrials, shots);

        // 调整噪声虚拟机参数，数值会根据噪声数值大小而受到影响，噪声越大，qv数值越小。
        std::cout << "Quantum Volume : " << qv_result << std::endl;
        
        qvm->finalize();
        delete qvm;
        return 0;
    }


运行结果：

::

    Quantum Volume ： 8


随机基准简介
--------------

随机基准测试（RB）是使用随机化方法对量子门进行基准测试。由于完整的过程层析成像对于大型系统是不可行的，因此越来越关注可扩展方法，
以部分表征影响量子系统的噪声。在\ `[1] <https://arxiv.org/pdf/1009.3639>`__\ 中提出了一种可扩展的、鲁棒的算法（n个量子位组成的系统），
使用随机技术通过单个参数对整个Clifford门进行基准测试的鲁棒算法。

接口说明
--------------
``single_qubit_rb`` 的输入参数分别噪声虚拟机或者量子云机器，待测量的量子比特，随机线路clifford门集的不同数量组合、随机线路的数量、测量次数、验证基本逻辑门（默认无），输出为\ ``std::map``
数据， 关键值为clifford门集数量，数值对应符合期望概率的大小。

``double_qubit_rb`` 的输入参数分别噪声虚拟机或者量子云机器，待测量的量子比特0，待测量的量子比特1，随机线路clifford门集的不同数量组合、随机线路的数量、测量次数、验证基本逻辑门（默认无）输出为\ ``std::map``
数据， 关键值为clifford门集数量，数值对应符合期望概率的大小。

实例
--------------
.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA
    int main()
    {
        // 构建噪声虚拟机，以及设置参数
        auto qvm = new NoiseQVM();
        qvm->init();
        qvm->set_noise_model(NOISE_MODEL::DEPOLARIZING_KRAUS_OPERATOR, CZ_GATE, 0.005);
        qvm->set_noise_model(NOISE_MODEL::DEPOLARIZING_KRAUS_OPERATOR, PAULI_Y_GATE, 0.005);

        // 同样可以申请云计算机器（采用真实芯片）
        //auto qvm = new QCloudMachine();
        //qvm->init("898D47CF515A48CEAA9F2326394B85C6")

        auto qv = qvm->qAllocMany(4);

        // 设置随机线路中clifford门集数量
        std::vector<int > range = { 5,10,15 };

        // 测量单比特随机基准
        std::map<int, double> res = single_qubit_rb(qvm, qv[0], range, 10, 1000);

        // 同样可以测量两比特随机基准
        //std::map<int, double> res = double_qubit_rb(qvm, qv[0], qv[1], range, 10, 1000);
       
        // 对应的数值随噪声影响，噪声数值越大，所得结果越小，且随clifford门集数量增多，结果数值越小。
        for (auto it : res)
        {
            std::cout << it.first << "  :  " << it.second << std::endl;
        }

        qvm->finalize();
        delete qvm;
        return 0;
    }

运行结果：

::
    
    5   :  0.9998
    10  :  0.9984
    15  :  0.998


交叉熵基准简介
--------------

交叉熵基准测试（xeb）是一种通过应用随机电路并测量观察到的位串测量值与从模拟获得的这些位串的预期概率之间的交叉熵来评估门性能的方法。

接口说明
--------------
``double_gate_xeb`` 输入参数分别噪声虚拟机或者量子云机器、待测量的量子比特0、待测量的量子比特1、线路不同层数、随机线路的数量、测量次数、验证双门类型（默认CZ门）。
输出为 ``std::map`` 数据，关键值为线路层数，数值对应符合期望概率的大小。

实例
--------------
.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA
    using namespace std;
    int main()
    {
        // 创建噪声虚拟机
        auto qvm = new NoiseQVM();
        qvm->init();
        
        // 同样可以申请云计算机器（采用真实芯片）
        //auto qvm = new QCloudMachine();
        //qvm->init("898D47CF515A48CEAA9F2326394B85C6")

        auto qv = qvm->qAllocMany(4);

        // 设置噪声参数
        std::vector<QVec> qvs = { { qv[0], qv[1] } };
        qvm->set_noise_model(DEPOLARIZING_KRAUS_OPERATOR, CZ_GATE, 0.1, qvs);

        // 设置不同层数组合
        std::vector<int> range = { 2,4,6,8,10 };
        auto res = double_gate_xeb(qvm, qv[0], qv[1], range, 10, 1000, CZ_GATE);
       
        // 对应的数值随噪声影响，噪声数值越大，所得结果越小，且层数增多，结果数值越小。
        for (auto it : res)
        {
            std::cout << it.first << "  :  " << it.second << std::endl;
        }
        qvm->finalize();
        delete qvm;
        return 0;
    }

运行结果：
::

    2   :  0.963627
    4   :  0.914385
    6   :  0.752838
    8   :  0.722809
    10  :  0.742715