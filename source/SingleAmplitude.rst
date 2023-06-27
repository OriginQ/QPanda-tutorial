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

以上是前期的准备工作，最后调用计算接口来获取结果，我们设计多种返回值的接口用于满足不同的计算需求，
主要接口有以下几种：

``run`` ：输入参数为执行的量子程序，申请的量子比特，最大RANK，quickBB优化的最大运行时间

``pMeasureBinindex`` ：输入参数为二进制索引字符串，如 ``pMeasureBinindex("0000000000")`` ，输出为该索引下的量子态，同时保证字符串长度与测量的比特数相同

``pMeasureDecindex`` ：输入参数为十进制索引字符串，如 ``pMeasureDecindex("1")``

``probRunDict`` ：输入参数为要执行的量子程序，以及要测量的量子比特。输出为对应量子比特的所有态结果。需要注意的是该接口要求量子比特数为30个以内时使用

具体见如下完整的计算示例所述：

完整示例代码
>>>>>>>>>>
----

.. _单振幅示例程序:
以下示例展示了单振幅量子虚拟机接口的使用方式

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA
        using namespace std;
        int main()
        {
            //申请单振幅量子虚拟机
            auto qvm = new SingleAmplitudeQVM();
            qvm->init();
            auto qv = qvm->qAllocMany(10);
            auto cv = qvm->cAllocMany(10);

            // 构建测试线路
            auto prog = QProg();
            for_each(qv.begin(), qv.end(), [&](Qubit* val) { prog << H(val); });
            prog << CZ(qv[1], qv[5])
                << CZ(qv[3], qv[5])
                << CZ(qv[2], qv[4])
                << CZ(qv[3], qv[7])
                << CZ(qv[0], qv[4])
                << RY(qv[7], PI / 2)
                << RX(qv[8], PI / 2)
                << RX(qv[9], PI / 2)
                << CR(qv[0], qv[1], PI)
                << CR(qv[2], qv[3], PI)
                << RY(qv[4], PI / 2)
                << RZ(qv[5], PI / 4)
                << RX(qv[6], PI / 2)
                << RZ(qv[7], PI / 4)
                << CR(qv[8], qv[9], PI)
                << CR(qv[1], qv[2], PI)
                << RY(qv[3], PI / 2)
                << RX(qv[4], PI / 2)
                << RX(qv[5], PI / 2)
                << CR(qv[9], qv[1], PI)
                << RY(qv[1], PI / 2)
                << RY(qv[2], PI / 2)
                << RZ(qv[3], PI / 4)
                << CR(qv[7], qv[8], PI);

            // pMeasureBinindex : 获取对应（二进制）量子态概率
            // run 有三个参数，默认2个，
            // 第一个执行的量子程序;
            // 第二个为申请的量子比特
            // 第三个为最大RANK，这里根据内存设置，默认30；
            // 第四个就是quickBB优化的最大运行时间，默认5s
            qvm->run(prog, qv);
            cout << qvm->pMeasureBinindex("0001000000") << endl;

            // pMeasureDecindex : 获取对应（10进制）量子态概率
            qvm->run(prog, qv);
            cout << qvm->pMeasureDecindex("1") << endl;

            // getProbDict 获取对应量子比特所有量子态（如果申请比特数超过30， 该接口不提供使用）
            qvm->run(prog, qv);
            auto res_1 = qvm->getProbDict(qv);

            // probRunDict  上面两个接口run和getProbDict的封装
            auto res = qvm->probRunDict(prog, qv);
            for (auto val : res)
            {
                std::cout << val.first << " : " << val.second << std::endl;
            }

            qvm->finalize();
            delete(qvm);
            return 0;
        }

    
    上述程序的计算结果如下，输出了所有态的概率

    .. code-block:: c

        0.00166709
        0.00166709
        ...
