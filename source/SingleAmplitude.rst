.. _单振幅量子虚拟机:

单振幅量子虚拟机
===============
----

目前我们可以通过量子计算的相关理论，用经典计算机实现模拟量子虚拟机。
量子虚拟机的模拟主要有全振幅与单振幅两种解决方案，其主要区别在于，全振幅一次模拟计算就能算出量子态的所有振幅，单振幅一次模拟计算只能计算出 :math:`2^{N}` 个振幅中的一个。

然而全振幅模拟量子计算时间较长，计算量随量子比特数指数增长，
在现有硬件下，无法模拟超过49量子比特。通过单振幅量子虚拟机技术可以模拟超过49比特，同时模拟速度有较大提升，且算法的计算量不随量子比特数指数提升。

使用介绍
>>>>>>>>>>>>>>>>
----

QPanda2中设计了 ``SingleAmplitudeQVM`` 类用于运行单振幅模拟量子计算，同时提供了相关接口，它的使用也很简单。

    .. code-block:: c

        #include "QPanda.h"

        USING_QPANDA

        int main(void)
        {

            //首先构建一个单振幅量子虚拟机
            SingleAmplitudeQVM qvm;

            //初始化和配置量子虚拟机环境
            qvm.init();
            auto qlist = qvm.qAllocMany(10);
            auto clist = qvm.cAllocMany(10);

            //构建量子算法对应的量子线路
            QProg prog;
            prog << HadamardQCircuit(qlist) << CNOT(qlist[1], qlist[5]) << CZ(qlist[3], qlist[5]);

        }

以上是前期的准备工作，最后调用计算接口来获取结果，我们设计多种返回值的接口用于满足不同的计算需求，具体见如下完整的计算示例所述：

完整示例代码
>>>>>>>>>>
----

.. _单振幅示例程序:
以下示例展示了单振幅量子虚拟机接口的使用方式

    .. code-block:: c

        #include "QPanda.h"

        USING_QPANDA

        int main(void)
        {
            SingleAmplitudeQVM qvm;

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
                << CR(qlist[7], qlist[8], PI);;

            //获取二进制下标对应的量子态振幅
            auto bin_index_result = qvm.PMeasure_bin_index(prog, "0000000000");

            //获取十进制下标对应的量子态振幅
            auto dec_index_result = qvm.PMeasure_dec_index(prog, "1");

            std::cout << bin_index_result << std::endl;
            std::cout << dec_index_result << std::endl;

            return 0;
        }

    ``bin_index_result`` 与 ``dec_index_result`` 接口分别计算量子态指定二进制和十进制下标的概率，上述程序的计算结果如下

    .. code-block:: c

        0.00166709
        0.00166709

    .. note::

        1. 部分接口，比如 ``getQState()`` 、 ``PMeasure(string)`` 、 ``PMeasure(string)`` 、 ``pMeasureBinIndex(string)`` 以及 ``getProbDict(qvec,string)`` 等即将舍弃，在此不做过多介绍
        2. 单振幅虚拟机适合模拟高比特低复杂度的量子线路，不适合模拟低比特高复杂度的线路。
