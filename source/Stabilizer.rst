.. _Stabilizer:

稳定器与Clifford模拟器
=========================
----

概述
>>>>>>>>>>>>>>>>
----

**叠加和纠缠** 都是量子优势的典型来源，但是当系统包含的量子比特个数N增加时，量子态系数的个数随N指数增加，将无法使用经典计算机实现传统的全振幅模拟，这一问题称为 **指数墙问题** 。

基于 **Gottesman_knill定理** ，我们可以得知，在基于特定门集形成的稳定器线路中，我们是可以通过多项式复杂度进行模拟的，而这也意味着，可以在某些特定逻辑门构造的线路中打破量子的指数级加速霸权，将经典模拟应用到量子线路中，从而验证量子计算机的结果是否正确。并且在未来的容错量子计算机中，必然是需要冗余信息进行编码，从而达到容错计算的可能，这显然在基于目前量子计算模拟框架中是无法实现大比特线路的。

我们可以另辟蹊径，通过 **stabilizer** 及对应的 **Clifford** 门集模拟器可以有效利用其多项式模拟的特性，解决基于pauli噪声的容错量子计算。同时，为了推广到通用量子计算，也可以将stabilizer的理论性质带入到 **Clifford+T** 的模拟中，基于 **Clifford+T** 的模拟器，我们可以解决大比特下的non-clifford逻辑门较少前提下的量子模拟(Clifford+T可以近似分解任意逻辑门)。

原理介绍
>>>>>>>>>>>>>>>>
----

对于一个量子态 :math:`|\psi\rangle` （一般指纯态），如果存在一个酉矩阵U使得 :math:`U|\psi\rangle = |\psi\rangle` ，那么称 :math:`|\psi\rangle` 可以被U所stabilize，U是 :math:`|\psi\rangle` 的一个stabilizer，比如 :math:`Z|0\rangle = |0\rangle` 。

很明显，一个量子态存在多个stabilizer，当有多个stabilizer时，这些stabilizer的乘积自然也是stabilizer。

 :math:`Z_{1}Z_{2}X_{1}X_{2}|\psi\rangle = Z_{1}Z_{2}|\psi\rangle = |\psi\rangle` 

这种乘法封闭性告诉我们stabilizer会形成一个 **群** 。

对于量子态 :math:`|\psi\rangle` ，若幺正变换群S中的每个元素都是 :math:`|\psi\rangle` 的stabilizer，则称整个幺正变换群S是 :math:`|\psi\rangle` 的stabilizer group。

一般情况下我们只关注 :math:`P\text{auli}` 矩阵 :math:`\left\{ X,Y,Z,I \right\}` 作为stabilizer的情况，即
幺正变换群由Pauli群构成，即

 :math:`Stab(|\psi\rangle) = \left\{ P \in \mathcal{P}_{n}:P|\psi\rangle = |\psi\rangle \right\}` 

上述式子中，Pauli群 :math:`\mathcal{P}_{n}` 定义为作用在n比特上的 :math:`P\text{auli}` 操作符的集合，其中相位系数为 :math:`\pm 1` 和 :math:`\pm i` 。

 :math:`\mathcal{P}_{n} = \left\{ i^{\gamma}X(a)Z(b):\gamma \in \{ 0,1,2,3\},a,b \in \{ 0,1\}^{n} \right\}` 

该Pauli群中 :math:`P^{(1)},\ldots,P^{(m)} \in \mathcal{P}_{n}` 各个元素均是独立的。那么我们依据Pauli群的特殊性质可以得到：

 :math:`\begin{matrix} \text{Stab}(|00\rangle)\& = \left\{ I,Z_{1},Z_{2},Z_{1}Z_{2} \right\}\& = \left\langle Z_{1},Z_{2} \right\rangle \\ \text{Stab}(| + + \rangle)\& = \left\{ I,X_{1},X_{2},X_{1}X_{2} \right\}\& = \left\langle X_{1},X_{2} \right\rangle \\ \text{Stab}\left( \frac{\left| 00 \right\rangle + \left| 11 \right\rangle}{\sqrt{2}} \right)\& = \left\{ I,X_{1}X_{2},Z_{1}Z_{2}, - Y_{1}Y_{2} \right\}\& = \ \left\langle X_{1}X_{2},Z_{1}Z_{2} \right\rangle \\ \text{Stab}\left( \left| 0^{n} \right\rangle \right)\& = \left\{ Z(a):a \in \{ 0,1\}^{n} \right\}\& = \left\langle Z_{1},\ldots,Z_{n} \right\rangle \\ \end{matrix}` 

问题在于如何构造 **Stabilizer Group** ，这里就不得不提到，当 **Cliffford Group** 门集中的元素作用在Pauli群上会有这样一组变换:

 :math:`\mathbf{P|\psi\rangle = |\psi\rangle \Longleftrightarrow}\left( \mathbf{\text{UP}}\mathbf{U}^{\mathbf{\dagger}} \right)\mathbf{U|\psi\rangle = U|\psi\rangle}` 

当我们将群写成形式 :math:`P = i^{\gamma}X(a)Z(b)` ， **Cliffford Group** 的作用形式如下：

 :math:`U_{j}PU_{j}^{\dagger} = i^{\gamma}X^{a_{1}}Z^{b_{1}} \otimes \ldots \otimes X^{a_{j - 1}}Z^{b_{j - 1}} \otimes UX^{a_{j}}Z^{b_{j}}U^{\dagger} \otimes X^{a_{j + 1}}Z^{b_{j + 1}} \otimes \ldots \otimes X^{a_{n}}Z^{b_{n}}` 

我们会惊讶的发现， :math:`\mathbf{U}_{\mathbf{j}}\mathbf{P}\mathbf{U}_{\mathbf{j}}^{\mathbf{\dagger}}\mathbf{=}\mathbf{P}_{\mathbf{\text{new}}}` 。也就如下图所示：

.. image:: images/clifford.png
   :align: center   

这里可以发现，我们将 :math:`\mathcal{P}_{n}` 中的Y的变换去除了，这是由于 :math:`Y = IXZ` 。

 :math:`|\psi\rangle \rightarrow U|\psi\rangle` 

等价的只需要追踪stabilizer的演化，同样可以得到系统完整的动力学信息。

 :math:`S \rightarrow USU^{\dagger}` 

这里将量子态的逻辑门演化问题转化为更新量子态对应的 **Stabilizer Group** 问题，即使用 **Stabilizer** 模拟量子线路的核心思想是使用 **Stabilizer Group** 表征量子态，而不是传统模拟器的振幅。

也就是说，在基于特定门集形成的稳定器线路中，根据线路特性，通过多项式复杂度即可进行模拟超大数量的量子线路 **（仅限由Clifford量子逻辑门集合和衍生集合组成：H, S, X, Y, Z, CNOT, CY, CZ, SWAP ）** 

使用介绍
>>>>>>>>>>>>>>>>
----

``pyqpanda`` 中可以通过 ``Stabilizer`` 类实现对大比特的Clifford线路模拟。和许多其他模拟器有类似的功能接口，主要分为以下两个:

采样测量
>>>>>>>>>>
----

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        //初始化Clifford模拟器，默认最大支持6000比特
        auto machine = Stabilizer();
        machine.init();

        auto q = machine.qAllocMany(100);
        auto c = machine.cAllocMany(100);

        //构建量子线路，支持的门集为{ H, S, X, Y, Z, CNOT, CY, CZ, SWAP }
        auto prog = QProg();
        prog << X(q[1])
            << H(q[2])
            << H(q[49])
            << Z(q[2])
            << CZ(q[0], q[22])
            << CNOT(q[2], q[39])
            << MeasureAll(q, c);

            //runWithConfiguration用于获取测量操作的测量结果
        auto result = machine.runWithConfiguration(prog, 1000);

        for (auto val : result)
        {
            std::cout << val.first << " : " << val.second << std::endl;
        }

        machine.finalize();
    
    输出结果如下：

    .. code-block:: c

       '000000000000000000000000000000000000000000000000000000000010': 244, 
       '000000000000000000001000000000000000000000000000000000000110': 278, 
       '000000000010000000000000000000000000000000000000000000000010': 252, 
       '000000000010000000001000000000000000000000000000000000000110': 226
      
概率测量
>>>>>>>>>>
----

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        //初始化Clifford模拟器，默认最大支持6000比特
        auto machine = Stabilizer();
        machine.init();

        auto q = machine.qAllocMany(100);
        auto c = machine.cAllocMany(100);

        //构建量子线路，支持的门集为{ H, S, X, Y, Z, CNOT, CY, CZ, SWAP }
        auto prog = QProg();
        prog << X(q[0])
            << H(q[2])
            << H(q[22])
            << Z(q[2])
            << CZ(q[0], q[22])
            << CNOT(q[2], q[10]);

            //runWithConfiguration用于获取测量操作的测量结果
        auto result = machine.probRunDict(prog, { q[0],q[2],q[10],q[22] });

        for (auto val : result)
        {
            std::cout << val.first << " : " << val.second << std::endl;
        }

        machine.finalize();
    
    输出结果如下：

    .. code-block:: c

        0000 : 0
        0001 : 0.25
        0010 : 0
        0011 : 0
        0100 : 0
        0101 : 0
        0110 : 0
        0111 : 0.25
        1000 : 0
        1001 : 0.25
        1010 : 0
        1011 : 0
        1100 : 0
        1101 : 0
        1110 : 0
        1111 : 0.25