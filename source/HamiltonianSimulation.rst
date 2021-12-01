哈密顿量模拟
=========================

哈密顿量以威廉·罗文·汉密尔顿（William Rowan Hamilton）命名，他也创造了牛顿力学的革命性改革，现在称为哈米尔顿力学，这在量子物理学中是重要的。
哈密顿量是所有粒子的动能的总和加上与系统相关的粒子的势能。 对于不同的情况或数量的粒子，哈密顿量是不同的，因为它包括粒子的动能之和以及对应于这种情况的势能函数。



指数上的哈密顿量
>>>>>>>>>>>>>>>>

在量子力学中，波函数 :math:`\Psi( |t \rangle)` 的时间演化由含时薛定谔方程控制。

将普朗克常量视为1，将积分上下限分别定为 0、t，并经过一系列数学运算后，可以得到 :math:`\Psi( |t \rangle) = e^{-iHt} \Psi( |0 \rangle)`



哈密顿量模拟的复杂性
>>>>>>>>>>>>>>>>>>>>>>>

哈密顿量（哈密顿算符）在数学上被表示为Hermitian矩阵,而随着qubit数量的增加，其希尔伯特空间是指数增长的，相对应的哈密顿量的维度也是呈指数增长。
因此，需要使用一些近似方法，最简单的近似方法就是在关于矩阵的矩阵的泰勒展开式  :math:`\Psi( |t \rangle) \approx  (I-iHt) \Psi( |0 \rangle)` 
通过更高阶的近似，可以得到更高的精度逼近。


模拟步骤及相关接口介绍
>>>>>>>>>>>>>>>>>>>>>>>

step1:构造相关矩阵；

step2:构造模拟线路；

step3:使用 ``QOperator`` 操作将线路构造成算符操作，并获取线路的对应矩阵；

step4:使用 ``expMat()`` 接口计算 ``e`` 的复数矩阵的真实值；

step4:使用 ``average_gate_fidelity()`` 接口计算两个矩阵的相似度；


示例
>>>>>>>>>>>>>>>>

Pauli-X 模拟
----------------
.. code-block:: c++

    #include "QPanda.h"
    USING_QPANDA

    int main()
    {
        QuantumMachine* machine = initQuantumMachine(CPU);
        auto q = qAllocMany(4);
        auto cbits = cAllocMany(4);

        auto prog = createEmptyQProg();

        Matrix2cd mat_operator;
        mat_operator.real() << 0, 1, 1, 0;
        mat_operator.imag() << 0, 0, 0, 0;

        QCircuit circuit;
        circuit << H(q[0])
                << X(q[0])
                << RZ(q[0], -PI)
                << X(q[0])
                << RZ(q[0], PI)
                << H(q[0]);
        QOperator sss(circuit);
        QStat unitary = sss.get_matrix();
        std::complex<double> conf(0, -1);
        qmatrix_t U = expMat(conf, mat_operator, PI);

        double www = average_gate_fidelity(U, unitary);
        std::cout << "The state_fidelity is " << www << endl;
        return 0;
    }

运行结果如下：

::

    The state_fidelity is 1


Pauli-Y 模拟
----------------
.. code-block:: c++

    #include "QPanda.h"
    USING_QPANDA

    int main()
    {
        QuantumMachine* machine = initQuantumMachine(CPU);
        auto q = qAllocMany(4);
        auto cbits = cAllocMany(4);

        auto prog = createEmptyQProg();
        QCircuit circuit;

        Matrix2cd mat_operator;
        mat_operator.real() << 0, 0, 0, 0;
        mat_operator.imag() << 0, -1, 1, 0;

        circuit << RX(q[0], PI / 2)
                << X(q[0])
                << RZ(q[0], -PI)
                << X(q[0])
                << RZ(q[0], PI)
                << RX(q[0], -PI / 2);
        QOperator sss(circuit);
        QStat unitary = sss.get_matrix();

        qcomplex_t conf(0, 1);
        qmatrix_t U = expMat(conf, mat_operator, PI);

        double www = average_gate_fidelity(U, unitary);
        std::cout << "The state_fidelity is " << www << endl;
  
        return 0;
    }

运行结果如下：

::

    The state_fidelity is 1


Pauli-Z 模拟
----------------
.. code-block:: c++

    #include "QPanda.h"
    USING_QPANDA

    int main()
    {
        QuantumMachine* machine = initQuantumMachine(CPU);
        auto q = qAllocMany(4);
        auto cbits = cAllocMany(4);

        auto prog = createEmptyQProg();
        QCircuit circuit;

        Matrix2cd mat_operator;
        mat_operator.real() << 1, 0, 0, -1;
        mat_operator.imag() << 0, 0, 0, 0;

        circuit << X(q[0])
                << RZ(q[0], -PI)
                << X(q[0])
                << RZ(q[0], PI);
        QOperator sss(circuit);
        QStat unitary = sss.get_matrix();

        std::complex<double> conf(0, -1);
        qmatrix_t U = expMat(conf, mat_operator, PI);

        double www = average_gate_fidelity(U, unitary);
        std::cout << "The state_fidelity is " << www << endl;
        return 0;
    }

运行结果如下：

::

    The state_fidelity is 1
