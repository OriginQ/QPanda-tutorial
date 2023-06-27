多控门分解
=====================

在量子算法实现过程中，经常会用到多控门，如下图所示：
    
.. figure:: ./images/multiControlGate.png

量子程序员在设计量子算法时经常会用到多控门，如上图所示，从图中我们可以看到有一个6个qubit受控的CZ门，在更加复杂的量子算法场景下，将会出现更多的、受控维度更高的多控门。目前实现的物理量子计算机基本都不支持多控门，并且我们无法保证所有的受控物理qubit都处于连通状态（目前的物理量子芯片都有固定的拓扑结构），所以想要在真实物理量子计算机上运行量子算法，首先要对多控门进行拆解，使其转换成N个量子芯片支持的逻辑门的组合，以适配目标量子芯片。

目前QPanda中实现了两种多控门分解算法，并封装成对应的算法接口，下面分别对两种分解方法做详细介绍。
    
算法概述及接口介绍
>>>>>>>>>>
----

1. **传统多控门分解算法**：该算法的实现过程如下流程图所示：

.. figure:: ./images/multiControlGateDecompose_1.png
   :alt:


对应的接口如下：

.. code-block:: c

    /**
     * @brief Decompose multiple control QGate
     * @ingroup Utilities
     * @param[in] QProg& Quantum Program
     * @param[in] QuantumMachine* quantum machine pointer
     * @param[in] const std::string& It can be configuration file or configuration data, which can be distinguished by file suffix, so the configuration file must be end with ".json", default is CONFIG_PATH
     * @return
     */
    void decompose_multiple_control_qgate(QProg& prog,  QuantumMachine *quantum_machine, const std::string& config_data = CONFIG_PATH);
    void decompose_multiple_control_qgate( QCircuit& cir, QuantumMachine *quantum_machine, const std::string& config_data = CONFIG_PATH);
    
**使用介绍**

通过调用decompose_multiple_control_qgate接口，可将目标量子线路中的多控门转换为指定的基础逻辑门组合，其中基础逻辑门包括基础单门和基础单门，通过配置文件给出。该接口需要3个参数，第一个是目标量子线路或者量子程序，第二个是目标量子线路或者量子程序对应的量子虚拟机，第三个参数用于指定配置信息，配置信息可以json文件或者json字符串，配置文件中指定了基础逻辑门信息。

**实例**

.. _多控门分解示例程序:

以下示例展示了多控门分解接口的使用方式：

.. code-block:: c
  
    #include <iostream>
    #include "QPanda.h"
    USING_QPANDA

    int main()
    {
        CPUQVM machine;
    machine.init();

    auto q = machine.qAllocMany(6);
    auto c = machine.cAllocMany(6);

    /* 构造测试量子线路 */
    QProg prog;
    prog << H(q[1]) << H(q[2]) << Z(q[0]).control({ q[1],q[2] });
    cout << "Src prog:" << prog << endl;

    /* 获取原始量子线路矩阵 */
    const auto mat_1 = getCircuitMatrix(prog);

    /* 执行多控门分解操作 */
    decompose_multiple_control_qgate(prog, &machine);
    cout << "after decompose_multiple_control_qgate prog:" << prog << endl;

    /* 获取多控门分解后的量子线路矩阵 */
    const auto mat_2 = getCircuitMatrix(prog);

    /* 结果验证：
     * 如果分解前后矩阵一致，则表示多控门被正确分解，否则，表示分解错误。
     */
    if (mat_1 == mat_2)
    {
        cout << "The multi-control gate was successfully decomposed." << endl;
        return -1;
    }
    
    cout << "Decompose error !" << endl;
    return 0;
    }

上述实例运行的结果如下：

.. figure:: ./images/multi_control_gate_decompose_result_1.png
   :alt:

根据测试程序数据结果可知，量子线路中的多控门被成功分解，且分解前后，量子线路矩阵形式不变，达到预期效果。

2. **ldd多控门分解算法**
   
该算法的实现原理大致如下：我们定义 :math:`a_jU_{a_k}` 表示一个由单量子位控制的单门，其中控制比特是 :math:`{a_j}` ，目标比特是 :math:`a_k` ，同时 :math:`C^{n}U` 表示多量子位控制，控制比特是 :math:`{a_1,···,a_n}` ，目标比特是 :math:`{a_{n+1}}` 

接着进行如下定义

.. math::

    \begin{aligned}
    \large P_n=\prod_{k=2}^na_kR_x(\frac{\pi}{2^{n-k+1}})
    \end{aligned}

.. math::

    \begin{aligned}
    \large Q_n=\prod_{k=1}^{n-1}C^kR_x(\pi)
    \end{aligned}

对于 :math:`C^{n}Rx(\pi)` 的分解方案可以写成

.. math::

    \begin{aligned}
    \large C^{n}Rx(\pi)=Q_{n}^{\dagger}p_{n}^{\dagger}Q_{n}(a_1R_x(\pi/2^{n-1})a_{n+1})p_n
    \end{aligned}

上述算法可进行改进，将其中的 :math:`R_x(\pi/k)` 替换为 :math:`\sqrt[k]{U}` ，以及将 :math:`R_x(-\pi/k)` 替换为 :math:`\sqrt[k]{U}^\dagger` ，对应的

.. math::

    \begin{aligned}
    \large P_n(U)=\prod_{k=2}^na_k\sqrt[2^{n-k+1}]{U}a_n)
    \end{aligned}

对于 :math:`U\in SU(2),C^{n}U` 的分解方案为

.. math::

    \begin{aligned}
    \large C^{n}U=Q_{n}^{\dagger}P_n(U)^{\dagger}Q_{n}(a_1\sqrt[2^{n-1}]{U}a_{n+1})P_n(U)
    \end{aligned}

以下示例展示了基于线性深度的多控门分解算法(LDD)接口的使用方式：

.. code-block:: c
  
    #include <iostream>
    #include "QPanda.h"
    USING_QPANDA

    int main()
    {
        CPUQVM machine;
        machine.init();

        auto q = machine.qAllocMany(6);
        auto c = machine.cAllocMany(6);

        /* 构造测试量子线路 */
        QProg prog;
        prog << H(q[1]) << H(q[2])
             << Z(q[0]).control({ q[1],q[2] });

        cout << "src prog:" << prog << endl;

        /* 获取原始量子线路矩阵 */
        const auto mat_1 = getCircuitMatrix(prog);

        /* 执行ldd多控门分解操作 */
        auto ldd_prog = ldd_decompose(prog);

        cout << "after ldd decompose_multiple_control_gate prog:" << ldd_prog << endl;

        /* 获取多控门分解后的量子线路矩阵 */
        const auto mat_2 = getCircuitMatrix(ldd_prog);

        /* 结果验证：如果分解前后矩阵一致，则表示多控门被正确分解，否则，表示分解错误。*/
        if (mat_1 == mat_2)
        {
            cout << "The multi-control gate was successfully decomposed." << endl;
            return true;
        }

        cout << "Decompose error !" << endl;
        return false;
}

上述实例运行的结果如下：

.. figure:: ./images/multi_control_gate_decompose_result_2.png
   :alt:

.. note:: 
        从对比图可以看出，ldd分解算法分解的结果量子线路深度较低，时间复杂度为O(n)，与量子比特数增加呈线性关系。由于ldd多控门分解产生的量子量子线路更加精简，后续将通过ldd多控门分解算法逐步替换传统的多控门分解算法。
    