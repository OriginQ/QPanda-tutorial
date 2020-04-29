.. _量子线路查询替换:

量子线路查询替换
=========================
----

在量子计算中，存在一些量子逻辑门或量子线路是可以相互替代的，比如如下替换过程：

H(0)->CNOT(1,0)->H(0)
可以替换为
CZ(1,0)

使用接口介绍
>>>>>>>>>>>>>>>>
----

在量子程序中，可能存在多个相同结构的子量子线路或多个相同的量子逻辑门，查询替换量子程序中指定结构的量子线路的功能就是找这些相同结构的子量子线路并把它们替换成目标量子线路。

通过graph_query_replace接口实现该功能，输入参数一为待替换修改的量子程序节点，输入参数二为查询图量子线路节点，输入参数三为替换图量子线路节点，输入参数四为空的量子程序，输入参数五为量子虚拟机指针。

示例
>>>>>>>>>>>>>>>>
----

     .. code-block:: c

        include "Core/QPanda.h"
        USING_QPANDA

        int main(void)
        {
            auto qvm = initQuantumMachine();
            auto q = qvm->allocateQubits(5);
            auto c = qvm->allocateCBits(5);

            auto prog = QProg();
            prog << H(q[0]) << H(q[2]) << H(q[3])
                << CNOT(q[1], q[0]) << H(q[0]) << CNOT(q[1], q[2])
                << H(q[2]) << CNOT(q[2], q[3]) << H(q[3]);

            cout << prog;
            auto query_cir = QCircuit();
            query_cir << H(q[0]) << CNOT(q[1], q[0]) << H(q[0]);

            auto replace_cir = QCircuit();
            replace_cir << CZ(q[0], q[1]);

            QProg update_prog;
            graph_query_replace(prog, query_cir, replace_cir, update_prog, qvm);

            cout << update_prog;

            return 0;
        }

运行结果如下：

查询替换前：

    .. code-block:: c

        QINIT 4
        CREG 0
        H q[0]
        H q[2]
        H q[3]
        CNOT q[1],q[0]
        H q[0]
        CNOT q[1],q[2]
        H q[2]
        CNOT q[2],q[3]
        H q[3]

查询替换后： 

    .. code-block:: c

        QINIT 4
        CREG 0
        CZ q[0],q[1]
        CZ q[2],q[1]
        CZ q[3],q[2]

    .. warning::

        1. 查询量子线路和替代量子线路控制的量子比特必须一一对应。
        2. 查询量子线路和替代量子线路对应的有向无环图必须为连通图。