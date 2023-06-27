.. _密度矩阵模拟器:

密度矩阵模拟器
=================
----

目前量子计算机的主要局限在于通用量子计算机所需的量子系统规模非常大，技术实现困难，因而人们主要利用中小规模量子体系，解决特定问题。

对于纯态和混合态量子比特系统，需要找到一种在低比特情况下，正确模拟噪声测量以及对哈密顿算符期望进行求解，而 ``密度矩阵模拟器`` 提供这一问题的解决方案。

密度矩阵相关学习可以参考 :ref:`密度矩阵介绍` 。

应用场景
>>>>>>>>>>>>>>>>
----

密度矩阵是表达量子态的另一种方式。而密度矩阵模拟器用于求解量子线路对应的密度矩阵，以及计算量子态概率分布、模拟含噪声量子线路和计算哈密顿量期望值等等。


使用介绍
>>>>>>>>>>>>>>>>
----

 ``QPanda`` 中可以通过 ``DensityMatrixSimulator`` 类实现用密度矩阵模拟器。和许多其他模拟器的使用方法一样，都具有相同的量子虚拟机接口，比如下述简单的使用示例代码:

    .. code-block:: c

        #include "QPanda.h"

        USING_QPANDA

        int main(void)
        {
            auto machine = DensityMatrixSimulator();
            machine.init();

            auto prog = QProg();
            auto q = machine.qAllocMany(2);
            auto c = machine.cAllocMany(2);

            prog << HadamardQCircuit(q)
                << Y(q[1])
                << X(q[0])
                << CNOT(q[0], q[1]);

            auto density_matrix = machine.get_density_matrix(prog);
            cout << density_matrix << endl;
        }

完整示例代码
>>>>>>>>>>
----

.. _密度矩阵模拟器示例程序:
以下示例展示了密度矩阵模拟器计算部分接口的使用方式

    .. code-block:: c

        #include "QPanda.h"

        USING_QPANDA

        int main(void)
        {
            auto machine = DensityMatrixSimulator();
            machine.init();

            auto q = machine.qAllocMany(2);
            auto c = machine.cAllocMany(2);

            auto prog = QProg();
            prog << H(q[0])
                << Y(q[1])
                << RY(q[0], PI / 3)
                << RX(q[1], PI / 6)
                << RX(q[1], PI / 9)
                << CZ(q[0], q[1]);

            //获取对应量子程序的密度矩阵
            std::cout << machine.get_density_matrix(prog) << std::endl;

            //获取对应量子程序的在指定量子比特下的约化密度矩阵
            std::cout << machine.get_reduced_density_matrix(prog, { q[0] }) << std::endl;

            //获取对应量子程序指定量子态的概率
            std::cout << machine.get_probability(prog, "00") << std::endl;

            //获取对应量子程序所有量子态的概率分布
            auto probs = machine.get_probabilities(prog);
            for (auto prob : probs)
                std::cout << prob << std::endl;

            //获取对应量子程序指定哈密顿量下演化的期望值
            auto opt = 0.23 * x(1) + 0.2 * y(1) + 1.6 * z(0);
            std::cout << machine.get_expectation(prog, opt.toHamiltonian(false), { 0,1 });

            //设置噪声模型和参数
            machine.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, GateType::HADAMARD_GATE, 0.3);
            machine.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, GateType::CZ_GATE, 0.3);

            //获取加入噪声后，密度矩阵信息和概率分布
            std::cout << machine.get_density_matrix(prog) << std::endl;

            auto noise_probs = machine.get_probabilities(prog);
            for (auto prob : noise_probs)
                std::cout << prob << std::endl;

            machine.finalize();
        }

    
    输出结果如下：

    .. code-block:: python

        # 对应量子程序的密度矩阵
        (0.0119643,0)   (0.0446515,0)  (0,-0.0256576)   (0,0.0957556)
        (0.0446515,0)    (0.166642,0)  (0,-0.0957556)    (0,0.357365)
        (0,0.0256576)   (0,0.0957556)    (0.055023,0)   (-0.205348,0)
        (-0,-0.0957556)  (-0,-0.357365)   (-0.205348,0)   (0.766371,-0)

        # 对应量子程序的在指定量子比特下的约化密度矩阵
        (0.0669873,0) (-0.160697,0)
        (-0.160697,0)  (0.933013,0)

        # 对应量子程序指定量子态的概率
        0.0119643

        # 对应量子程序所有量子态的概率分布
        0.0119643
        0.166642
        0.055023
        0.766371

        # 对应量子程序指定哈密顿量下演化的期望值
        -1.5183234356888893 

        # 加入噪声后，密度矩阵信息
        (0.121386,0) (-0.0303485,0)  (0,0.0356996)  (0,0.0383022)
        (-0.0303485,0)   (0.250057,0) (0,-0.0383022)  (0,0.0969832)
        (0,-0.0356996)  (0,0.0383022)   (0.205409,0)  (-0.130348,0)
        (0,-0.0383022) (0,-0.0969832)  (-0.130348,0)   (0.423148,0)

        # 加入噪声后，概率分布
        0.12138551462195893
        0.25005696344073314
        0.20540940462115326
        0.4231481173161546
       