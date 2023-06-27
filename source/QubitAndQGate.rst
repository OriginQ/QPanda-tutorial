基础概念回顾
####
----

基础定义
****

在物理学中，量子是物理量的最小的不可分的基本单位。比特是计算机术语，指信息量最小单位。
不同于经典比特，量子比特不再只能取值0或1，还可以处于0和1的任意比例叠加的中间态。

对量子比特进行的基本运算操作叫做量子门。

量子门分为单比特门和多比特门。
单比特门有Hadamard门、Pauli-X/Y/Z门和旋转X/Y/Z门等。二比特门既有受控的单比特门（例如CNOT门等）也有交换门。
通过受控等扩展方式，可以将单比特门和二比特门进一步扩展为多比特门。
注意，测量是一种特殊的量子门，它是不可逆的，会改变量子比特的状态。

任何量子算法，都是由这些基本的量子门组合得到的。

普适量子门的定义参见 `常见量子逻辑门矩阵形式 <https://qpanda-tutorial.readthedocs.io/zh/latest/QGate.html>`_\。

QPanda接口函数
****

在QPanda-2.0中，量子门的定义函数形式如下：

.. code-block:: c
        
        QGate H(Qubit *qubit);

.. note:: 输入参数为量子比特Qubit及其他参数，返回值为可以插入量子线路的量子门QGate。

在QPanda-2.0中定义的量子门种类非常丰富。\
特别地，QPanda-2.0中支持完全自定义的量子门U4门，它的接口函数同时有以下几种重载：

.. code-block:: c
        
        QGate U4(double alpha, double beta, double gamma, double delta, Qubit *qubit);
        QGate U4(Qubit *qubit, double alpha, double beta, double gamma, double delta);
        QGate U4(QStat &matrix, Qubit *qubit);
        QGate U4(Qubit *qubit, QStat &matrix);

如前文所述，量子门的接口函数有两种拓展操作：转置共轭和受控。两种操作都各有两种实现方式。

转置共轭操作的两种接口函数定义如下：

.. code-block:: c
        
        QGate gate = H(qubit);
        QGate gate1 = gate.dagger();
        gate.setDagger(true);

.. note:: dagger函数返回的是一个基于目标量子门的新量子门，setDagger返回的则是进行转置共轭后的目标量子门。

受控操作的两种接口函数定义如下：

.. code-block:: c
        
        QGate gate = H(qubit);
        QGate gate1 = gate.control(QVec);
        gate.setControl(QVec);

.. note:: 区别与转置共轭操作类似，但受控函数入参是Qvec（qubit的vector）而非单个qubit。



实例
****

下面以一个程序实例，来展示基本的量子比特和量子门操作的代码实现。

.. code-block:: c

    #include "QPanda.h"
    using namespace QPanda;

    int main(void)
    {
        auto qvm = CPUQVM();
        qvm.init();
        // 申请寄存器并初始化
        QVec q = qvm.qAllocMany(3);
        // 基于已有QVec定义
        QVec qubits = { q[0],q[1] };

        // 构建量子线路
        auto prog = QProg();
        prog << H(q[0])
            << H(q[1])
            << H(q[0]).dagger()         // 转置共轭
            << X(q[2]).control(qubits); // 受控

        // 以概率方法输出结果量子态的理论值（并非测量）
        auto result = qvm.probRunDict(prog, q);

        // 输出结果
        for (auto& aiter : result)
        {
            cout << aiter.first << " : " << aiter.second << endl;
        }

        return 0;
    }

输出结果应如下所示，分别以0.5的概率得到 :math:`\left|0\right\rangle`\和 :math:`\left|2\right\rangle` ：

.. code-block:: c
    
    000 : 0.5
    001 : 0
    010 : 0.5
    011 : 0
    100 : 0
    101 : 0
    110 : 0
    111 : 0

以上就是量子比特和量子门的基本定义和在QPanda-2.0中的调用介绍。