.. _张量网络量子电路模拟器:

张量网络量子电路模拟器
=================
----

对于一个 :math:`N` 个量子比特的自旋体系，对应的希尔伯特空间维数为 :math:`2^{N}` 。

对于该复杂系统的状态演化，传统的全振幅模拟器将其看做一个有 :math:`2^{N}` 个元素的一维向量。

然而从张量网络的角度来看，整个系统量子态的系数对应 :math:`2^{N}` 维张量（即N阶张量，即有 :math:`N` 个指标，每个指标的维数是2），量子操作算符的系数为 :math:`2^{2N}` 维张量（ :math:`2N` 阶张量，即有个 :math:`2N` 指标，每个指标的维数是2），我们可以用如下图形来表示量子态：

.. image:: images/state.png
   :align: center  

当量子系统的自旋个数增加时，量子态系数的个数随指数增加，称为指数墙问题，这一障碍限制了传统全振幅模拟器的最大模拟自旋数和模拟性能。

但是可通过张量网络处理这一问题，从而绕过指数墙障碍，在张量网络中，我们对量子系统的模拟，包括量子逻辑门操作和测量操作，均可以通过对于张量的缩并与分解来实现。矩阵乘积态是张量网络中最常用的表示形式，在多线性代数中称为张量列或TT（Tensor-Train），示意图如下。

.. image:: images/MPS.png
   :align: center  

将量子态分解成等式右边的表示形式，对于量子线路中部分量子逻辑门操作，可以将全局问题转化为局部的张量处理问题，从而有效地降低了时间复杂度和空间复杂度。

使用介绍
>>>>>>>>>>>>>>>>
----

QPanda2中设计了 ``MPSQVM`` 类用于使用这一方法的模拟器进行模拟量子电路
和许多量子虚拟机的使用方法一样，需要先进行如下前期工作：

    .. code-block:: c

        #include "QPanda.h"

        USING_QPANDA

        int main(void)
        {
            //首先构建一个张量网络模拟器
            MPSQVM qvm;

            //初始化和配置量子虚拟机环境
            qvm.init();
            auto qlist = qvm.qAllocMany(30);
            auto clist = qvm.cAllocMany(30);

            //构建量子算法对应的量子线路
            QProg prog;
            prog << HadamardQCircuit(qlist) << CNOT(qlist[1], qlist[5]) << CZ(qlist[3], qlist[5]);

        }

    然后使用不同的接口去模拟目标量子线路

完整示例代码
>>>>>>>>>>
----

.. _张量网络模拟器示例程序:
以下示例展示了张量网络模拟器接口的使用方式

    .. code-block:: c

        #include "QPanda.h"

        USING_QPANDA

        int main(void)
        {
            MPSQVM qvm;

            qvm.init();
            auto qlist = qvm.qAllocMany(10);
            auto clist = qvm.cAllocMany(10); 

            QProg prog;
            prog << HadamardQCircuit(qlist)
                << CZ(qlist[1], qlist[5])
                << CZ(qlist[3], qlist[5])
                << CZ(qlist[2], qlist[4])
                << CZ(qlist[3], qlist[7])
                << CZ(qlist[0], qlist[4])
                << RY(qlist[7], PI / 2)
                << RX(qlist[8], PI / 2)
                << RX(qlist[9], PI / 2)
                << CR(qlist[0], qlist[1], PI)
                << CR(qlist[2], qlist[3], PI)
                << RY(qlist[4], PI / 2)
                << RZ(qlist[5], PI / 4)
                << RX(qlist[6], PI / 2)
                << RZ(qlist[7], PI / 4)
                << CR(qlist[8], qlist[9], PI)
                << CR(qlist[1], qlist[2], PI)
                << RY(qlist[3], PI / 2)
                << RX(qlist[4], PI / 2)
                << RX(qlist[5], PI / 2)
                << CR(qlist[9], qlist[1], PI)
                << RY(qlist[1], PI / 2)
                << RY(qlist[2], PI / 2)
                << RZ(qlist[3], PI / 4)
                << CR(qlist[7], qlist[8], PI)
                <<MeasureAll(qlist,clist);

                auto measure_result = qvm.runWithConfiguration(prog, clist, 1000);
                for (auto val : measure_result)
                {
                    cout << val.first << " : " << val.second << endl;
                }

                auto pmeasure_result = qvm.probRunDict(prog, qlist, -1);
                for (auto val : pmeasure_result)
                {
                    cout << val.first << " : " << val.second << endl;
                }

                return 0;
        }

    ``runWithConfiguration`` 与 ``probRunDict`` 接口分别用于Monte Carlo采样模拟和概率测量，他们分别输出模拟采样的结果和对应振幅的概率，上述程序的计算结果如下

    .. code-block:: c

        //Monte Carlo 采样模拟结果
        0000000111 : 1
        0000110110 : 1
        0000111000 : 2
        0001000001 : 3
        0001000100 : 1
        0001001101 : 1
        0001010000 : 2
        0001101100 : 1
        0001110110 : 1
        ...

        //概率测量结果
        0000000000 : 0.0016671
        0000000001 : 0.0016671
        0000000010 : 0.000286029
        0000000011 : 0.000286029
        0000000100 : 0.000286029
        0000000101 : 0.000286029
        0000000110 : 0.0016671
        0000000111 : 0.0016671
        0000001000 : 0.0016671
        0000001001 : 0.0016671
        0000001010 : 0.000286029
        0000001011 : 0.000286029
        ...

    .. note::

        1. 概率测量还支持其他输出类型的接口，比如 ``getProbTupleList(QVec, int)`` 、 ``probRunTupleList(QProg &, QVec, int)`` 、 ``probRunList(QProg &, QVec, int)`` 、 ``getQState()`` 以及 ``pMeasure(QVec, int)`` 等，在此不做过多介绍。
        2. 单后续张量网络模拟器会支持含噪声的模拟，使量子电路的模拟更贴近真实的量子计算机，支持自定义的逻辑门类型和噪声模型，关于噪声的详细介绍可参考 :ref:`NoiseQVM` 部分
