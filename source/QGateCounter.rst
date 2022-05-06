.. _QGateCounter:

逻辑门统计
===============

简介
--------------

逻辑门的统计是指统计量子程序、量子线路、量子循环控制或量子条件控制中所有的量子逻辑门（这里也会将测量门统计进去）个数方法。

接口介绍
--------------

``QGateCounter`` 类是统计一个量子程序(量子线路、量子循环控制、量子条件控制)中量子逻辑门个数的工具类，我们先用QPanda2构建一个量子程序：

    .. code-block:: c
          
        auto qubits = qvm.qAllocMany(4);
        auto cbits = qvm.cAllocMany(4);

        QProg prog;
        prog << X(qubits[0])
            << Y(qubits[1])
            << H(qubits[0])
            << RX(qubits[0], 3.14)
            << Measure(qubits[1], cbits[0]);

然后调用 ``QGateCounter`` 类统计量子逻辑门的个数，

    .. code-block:: c
          
        QGateCounter t;
        t.traversal(prog);
        size_t num = t.count(prog);;

我们还可以使用QPanda2封装的一个接口：

    .. code-block:: c
          
        size_t num = getQGateNum(prog);

.. note::  统计 ``QCircuit`` 、 ``QWhileProg`` 、``QIfProg`` 中量子逻辑门的个数和 ``QProg`` 类似。

实例
-------------

    .. code-block:: c
    
        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            auto qvm = CPUQVM();
            qvm.init();
            auto qubits = qvm.qAllocMany(4);
            auto cbits = qvm.cAllocMany(4);

            QProg prog;

            // 构建量子程序
            prog << X(qubits[0])
                << Y(qubits[1])
                << H(qubits[0])
                << RX(qubits[0], 3.14)
                << Measure(qubits[1], cbits[0]);

            // 统计逻辑门个数
            size_t num = getQGateNum(prog);

            std::cout << "QGate number: " << num << std::endl;
            return;
        }

运行结果：

    .. code-block:: c

        QGate number: 4



    
