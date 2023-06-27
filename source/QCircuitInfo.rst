.. 量子线路信息查询:

获取量子线路对应矩阵
====================

接口 ``getCircuitMatrix`` 可以获得输入线路的对应矩阵，有3个输出参数，一个量子线路QCircuit(或者Qprog)，另外两个是可选参数：迭代器开始位置和结束位置，用于指定一个要获取对应矩阵信息的线路区间，如果这两个参数为空，代表要获取整个量子线路的矩阵信息。

.. note:: 使用 getCircuitMatrix 需要注意的是量子线路中不能包含测量操作。

实例
---------------

.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA

    int main(void)
    {
        auto qvm = CPUQVM();
        qvm.init();
        auto q = qvm.qAllocMany(2);
        auto c = qvm.cAllocMany(2);

        // 构建量子线路
        QCircuit cir;
        cir << H(q[1])
            << CNOT(q[0], q[1])
            << H(q[1]);
        
        // 获取线路对应矩阵
        QStat cir_matrix = getCircuitMatrix(cir);

        // 打印矩阵信息
        std::cout << cir_matrix << std::endl;

        return 0;
    }


具体步骤如下:

1. 首先在主程序中用 CPUQVN() 生成一个虚拟机
   再初始化这个虚拟机，用于管理后续一系列行为
2. 接着用 qAllocMany() 和 cAllocMany()初始化量子比特与经典寄存器数目
3. 然后构建量子线路 cir
4. 最后调用接口 getCircuitMatrix() 输出量子线路的对应矩阵，并打印矩阵


判断量子逻辑门是否匹配量子拓扑结构
====================================

每一款量子芯片都有其特殊的量子比特拓扑结构,例如IBM QX3：

.. figure:: ./images/IBM_Qubits.png
   :alt:

从图中可知，量子芯片中的每个量子比特不是两两相连的，不相连的量子比特之间是不能直接执行多门操作的。所以在执行量子程序之前需要先判断量子程序中的双门（多门）操作是否适配量子比特拓扑结构。

接口介绍
---------------

isMatchTopology：判断量子逻辑门是否符合量子比特拓扑结构。第一个输入参数是目标量子逻辑门QGate，第二个输入参数是量子比特拓扑结构，返回值为布尔值，表示目标量子逻辑门是否满足量子比特拓扑结构。True为满足，False为不满足。

::

    vector<vector<int>> qubits_topology = { {0,1,1,0},
                                            {1,0,0,1},
                                            {1,0,0,1},
                                            {0,1,1,0} };

    bool result = isMatchTopology(CNOT(q[1],q[3]),qubits_topology);

在使用isMatchTopology前需要先构建指定量子芯片的量子比特拓扑结构邻接矩阵qubits_topology。

从以上示例可以看出，qubits_topology有四个量子比特，量子比特拓扑图如下：

.. figure:: ./images/My_Qubits.png
   :alt:

CNOT逻辑门操作的是1,3号量子比特，而从图中可以看出1,3号量子比特是相连的，所以得到的结果为true。

获得指定位置的量子逻辑门的相邻量子逻辑门
========================================

接口 getAdjacentQGateType 可以获得量子程序中指定位置的量子逻辑门的相邻逻辑门。第一个输入参数为目标量子程序QProg，第二个是目标量子逻辑门在量子程序中的迭代器，第三个输出参数是目标量子逻辑门的相邻量子逻辑门迭代器的集合。

实例
---------------

.. code-block:: c
 
    #include "QPanda.h"
    USING_QPANDA
    int main(void)
    {
        auto qvm = CPUQVM();
        qvm.init();
        auto q = qvm.qAllocMany(4);
        auto c = qvm.cAllocMany(4);
        QProg prog;

        // 构建量子程序
        prog << H(q[0]) 
            << H(q[1]) 
            << H(q[2]) 
            << H(q[3])
            << RX(q[0], PI / 2) 
            << CNOT(q[1], q[2])
            << RX(q[1], PI / 2) 
            << RX(q[2], PI / 2)
            << RX(q[3], PI / 2) 
            << CNOT(q[2], q[3]);

        auto node_iter = prog.getFirstNodeIter();
        std::vector<NodeInfo> node_iter_vector;

        // 获取量子程序中node_iter位置上的的相邻节点
        getAdjacentQGateType(prog, node_iter, node_iter_vector);

        // 打印前后相邻节点类型
        std::cout << "The previous node type : " << node_iter_vector[0].m_node_type << std::endl;
        std::cout << "The node type that follows :" << node_iter_vector[1].m_node_type << std::endl;

        return 0;
    }



以上实例展示 getAdjacentQGateType 接口的使用方式：

  1. 构建一个量子程序prog；
  2. 获取prog的第一个量子逻辑门的迭代器node_iter；
  3. 调用getAdjacentQGateType接口获取node_iter的相邻逻辑门的迭代器集合。

在使用getAdjacentQGateType接口时，我们需要注意以下几点： 

  1. 目标量子逻辑门相邻量子逻辑门迭代器的集合永远包含两个元素；第一个元素是前一个量子逻辑门的迭代器，第二个元素是后一个量子逻辑门的迭代器。
  2. 如果目标量子逻辑门是量子程序的第一个节点，那么输出的参数目标量子逻辑门相邻量子逻辑门迭代器的集合中则只能获取目标量子逻辑门后一个量子逻辑门的迭代器，集合的第一个元素为空迭代器。
  3. 如果目标量子逻辑门是量子程序的最后一个量子逻辑门，那么输出的参数目标量子逻辑门相邻量子逻辑门迭代器的集合中则只能获取目标量子逻辑门前一个量子逻辑门的迭代器，集合的第二个元素为空迭代器。
  4. 如果目标量子逻辑门前一个节点是QIf或者QWhile，那么输出的参数目标量子逻辑门相邻量子逻辑门迭代器的集合中则只能获取目标量子逻辑门后一个量子逻辑门的迭代器，集合的第一个元素为空迭代器。
  5. 如果目标量子逻辑门后一个节点是QIf或者QWhile，那么输出的参数目标量子逻辑门相邻量子逻辑门迭代器的集合中则只能获取目标量子逻辑门前一个量子逻辑门的迭代器，集合的第二个元素为空迭代器。
  6. 如果目标量子逻辑门是QWhile的第一个量子逻辑门，那么输出的参数目标量子逻辑门相邻量子逻辑门迭代器的集合中则只能获取目标量子逻辑门后一个量子逻辑门的迭代器，集合的第一个元素为空迭代器。
  7. 如果目标量子逻辑门是QWhile的最后量子逻辑门，那么输出的参数目标量子逻辑门相邻量子逻辑门迭代器的集合中则只能获取目标量子逻辑门前一个量子逻辑门的迭代器，集合的第二个元素为空迭代器。

判断两个量子逻辑门是否可交换位置
================================

接口isSwappable可判断量子程序中两个指定位置的量子逻辑门是否可以交换位置。输入参数一为量子程序QProg，输入参数二，三是需要判断的两个量子逻辑门的迭代器。返回值为布尔值，True表示可交换，False表示不可交换。

实例
---------------

以下实例展示isSwappable接口的使用方式：

  1. 构建一个量子程序prog； 
  2. 获取prog的第一个量子逻辑门的迭代器node_iter和最后一个量逻辑门的迭代器last_node_iter；
  3. 调用isSwappable接口判断指定位置的两个逻辑门能否交换位置。

.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA
    int main(void)
    {
        auto qvm = CPUQVM();
        qvm.init();
        auto q = qvm.qAllocMany(4);
        auto c = qvm.cAllocMany(4);
        QProg prog;

        // 构建量子程序
        prog << H(q[0]) 
            << H(q[1]) 
            << H(q[2]) 
            << H(q[3])
            << RX(q[0], PI / 2) 
            << CNOT(q[1], q[2])
            << RX(q[1], PI / 2) 
            << RX(q[2], PI / 2)
            << RX(q[3], PI / 2) 
            << CNOT(q[2], q[3]);
        
        // 获取待判断的节点
        auto node_iter = prog.getFirstNodeIter();
        auto last_node_iter = prog.getLastNodeIter();

        // 判断节点是否可交换
        bool result = isSwappable(prog, node_iter, last_node_iter);

        if (result)
            std::cout << "is  swappable! " << std::endl;
        else
            std::cout << "is not swappable! " << std::endl;

        return 0;
    }


判断逻辑门是否属于量子芯片支持的量子逻辑门集合
==============================================

量子芯片支持的量子逻辑门集合可在元数据配置文件QPandaConfig.json
中配置。如果我们没有设置配置文件，QPanda会默认设置一个默认量子逻辑门集合。

默认集合如下所示：

::

        single_gates.push_back("RX");
        single_gates.push_back("RY");
        single_gates.push_back("RZ");
        single_gates.push_back("X1");
        single_gates.push_back("H");
        single_gates.push_back("S");

        double_gates.push_back("CNOT");
        double_gates.push_back("CZ");
        double_gates.push_back("ISWAP");

配置文件可仿照下面设置:

::


    "QGate": {
        "SingleGate": {
        "RX": { "time": 2 },
        "RY": { "time": 2 },
        "RZ": { "time": 2 },
        "S":  { "time": 2 },
        "H":  { "time": 2 },
        "X1": { "time": 2 },
        },
        "DoubleGate": {
        "CNOT":  { "time": 5 },
        "CZ":    { "time": 5 },
        "ISWAP": { "time": 5 },
        }
    },  

从上面的示例中我们可以得到，量子芯片支持RX，RY，RZ，S，H，X1，CNOT，CZ，ISWAP门。在配置文件配置完成后，我们可以调用接口isSupportedGateType，判断逻辑门是否属于量子芯片支持的量子逻辑门集合。isSupportedGateType接口只有一个参数：目标量子逻辑门；

.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA

    int main(void)
    {
        auto qvm = CPUQVM();
        qvm.init();
        auto q = qvm.qAllocMany(5);
        QProg prog;

        // 构建待判断的逻辑门
        prog << H(q[1]);

        // 判断逻辑门类型是否支持
        bool result = isSupportedGateType(prog.getFirstNodeIter());

        if (result)
            std::cout << "Gate type is supported !";
        else
            std::cout << "Gate type is not supported !";

        return 0;
    }

.. note:: 用户可通过如下链接地址获取默认配置文件 `QPandaConfig.json <https://github.com/OriginQ/QPanda-2/blob/master/CMakeSettings.json>`_ , 将该默认配置文件放在执行程序同级目录下，可执行程序会自动解析该文件。
