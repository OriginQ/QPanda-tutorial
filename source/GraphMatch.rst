.. _量子线路查询替换:

量子线路查询替换
=========================

在量子计算中，存在一些量子逻辑门或量子线路是可以相互替代的，比如如下替换过程：

H(0)->CNOT(1,0)->H(0)
可以替换为
CZ(1,0)

使用接口介绍
>>>>>>>>>>>>>>>>


在量子程序中，可能存在多个相同结构的子量子线路或多个相同的量子逻辑门，查询替换量子程序中指定结构的量子线路的功能就是找这些相同结构的子量子线路并把它们替换成目标量子线路。

通过sub_cir_replace接口实现该功能，输入参数一为待替换修改的量子程序节点，输入参数二为查询线路、 替换线路的有序对。

示例
>>>>>>>>>>>>>>>>

.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA

    int main(void)
    {
        auto qvm = initQuantumMachine();
        auto q = qvm->qAllocMany(5);
        auto c = qvm->cAllocMany(5);

        QProg prog;
        QCircuit replace_cir, query_cir;

        // 构建量子程序
        prog << H(q[0])
            << H(q[2])
            << H(q[3])
            << CNOT(q[1], q[0])
            << H(q[0])
            << CNOT(q[1], q[2])
            << H(q[2])
            << CNOT(q[2], q[3])
            << H(q[3]);

        std::cout << "查询替换前：" << std::endl;
        std::cout << convert_qprog_to_originir(prog, qvm) << std::endl;

        // 构建查询线路、 构建替换线路
        query_cir << H(q[0]) << CNOT(q[1], q[0]) << H(q[0]);
        replace_cir << CZ(q[0], q[1]);
        const std::vector<std::pair<QCircuit, QCircuit>>  replace_cir_vec = { {query_cir, replace_cir} };

        // 搜索量子程序中的查询线路，并用替换线路替代,但会改变原来prog的结构
        sub_cir_replace(prog, replace_cir_vec);

        std::cout << std::endl;
        std::cout << "查询替换后：" << std::endl;
        std::cout << convert_qprog_to_originir(prog, qvm) << std::endl;

        destroyQuantumMachine(qvm);
        return 0;
    }

运行结果如下：

::

    查询替换前：
    QINIT 5
    CREG 5
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
    QINIT 5
    CREG 5
    CZ q[0],q[1]
    CZ q[2],q[1]
    CZ q[3],q[2]


.. warning::

    1. 查询量子线路和替代量子线路控制的量子比特必须一一对应。
    2. 查询量子线路和替代量子线路对应的有向无环图必须为连通图。
