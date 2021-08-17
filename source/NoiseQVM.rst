.. _NoiseQVM:

含噪声量子虚拟机
===================

在真实的量子计算机中，受制于量子比特自身的物理特性，常常存在不可避免的计算误差。为了能在量子虚拟机中更好的模拟这种误差，在 :ref:`QuantumMachine` 的基础上，
QPanda2带来了含噪声量子虚拟机。含噪声量子虚拟机的模拟更贴近真实的量子计算机，我们可以自定义支持的逻辑门类型，自定义逻辑门支持的噪声模型，
通过这些自定义形式，我们使用QPanda2开发量子程序的现实应用程度将更高。


噪声模型介绍
--------------------------------------

QPanda2的含噪声量子虚拟机为我们提供了丰富的噪声模型，我们可以自定义噪声模型和量子逻辑门的对应关系。噪声模型主要分为两种：单门噪声模型和双门噪声模型。

单门噪声模型
>>>>>>>>>>>>>>

DAMPING_KRAUS_OPERATOR
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

DAMPING_KRAUS_OPERATOR是量子比特的弛豫过程噪声模型，它的kraus算符和表示方法如下所示：

:math:`K_1 = \begin{bmatrix} 1 & 0 \\ 0 & \sqrt{1 - p} \end{bmatrix},   K_2 = \begin{bmatrix} 0 & \sqrt{p} \\ 0 & 0 \end{bmatrix}`

需要一个噪声参数。

DEPHASING_KRAUS_OPERATOR
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

DEPHASING_KRAUS_OPERATOR是量子比特的退相位过程噪声模型，它的kraus算符和表示方法如下所示：

:math:`K_1 = \begin{bmatrix} \sqrt{1 - p} & 0 \\ 0 & \sqrt{1 - p} \end{bmatrix},   K_2 = \begin{bmatrix} \sqrt{p} & 0 \\ 0 & -\sqrt{p} \end{bmatrix}`

需要一个噪声参数。

DECOHERENCE_KRAUS_OPERATOR
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

DECOHERENCE_KRAUS_OPERATOR是退相干噪声模型，为上述两种噪声模型的综合，他们的关系如下所示：

:math:`P_{damping} = 1 - e^{-\frac{t_{gate}}{T_1}}, P_{dephasing} = 0.5 \times (1 - e^{-(\frac{t_{gate}}{T_2} - \frac{t_{gate}}{2T_1})})`

:math:`K_1 = K_{1_{damping}}K_{1_{dephasing}}, K_2 = K_{1_{damping}}K_{2_{dephasing}}`

:math:`K_3 = K_{2_{damping}}K_{1_{dephasing}}, K_4 = K_{2_{damping}}K_{2_{dephasing}}`

需要三个噪声参数。

DEPOLARIZING_KRAUS_OPERATOR
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

DEPOLARIZING_KRAUS_OPERATOR去极化噪声模型，即单量子比特有一定的概率被完全混合态I/2代替, 它的kraus算符和表示方法如下所示：

:math:`K_1 = \sqrt{1 - 3p/4} \times I, K_2 = \sqrt{p}/2 \times X` 

:math:`K_3 = \sqrt{p}/2 \times Y, K_4 = \sqrt{p}/2 \times Z`

其中I、X、Y、Z分别代表其量子逻辑门对应的矩阵

需要一个参数

BITFLIP_KRAUS_OPERATOR
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

BITFLIP_KRAUS_OPERATOR是比特反转噪声模型，它的kraus算符和表示方法如下所示：

:math:`K_1 = \begin{bmatrix} \sqrt{1 - p} & 0 \\ 0 & \sqrt{1 - p} \end{bmatrix}, K_2 = \begin{bmatrix} 0 & \sqrt{p} \\ \sqrt{p} & 0 \end{bmatrix}`

需要一个噪声参数。

BIT_PHASE_FLIP_OPRATOR
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

BIT_PHASE_FLIP_OPRATOR是比特-相位反转噪声模型，它的kraus算符和表示方法如下所示：

:math:`K_1 = \begin{bmatrix} \sqrt{1 - p} & 0 \\ 0 & \sqrt{1 - p} \end{bmatrix}, K_2 = \begin{bmatrix} 0 & -i \times \sqrt{p} \\ i \times \sqrt{p} & 0 \end{bmatrix}`

需要一个噪声参数。

PHASE_DAMPING_OPRATOR
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

PHASE_DAMPING_OPRATOR是相位阻尼噪声模型，它的kraus算符和表示方法如下所示：

:math:`K_1 = \begin{bmatrix} 1 & 0 \\ 0 & \sqrt{1 - p} \end{bmatrix}, K_2 = \begin{bmatrix} 0 & 0 \\ 0 & \sqrt{p} \end{bmatrix}`

需要一个噪声参数。

双门噪声模型
>>>>>>>>>>>>>>

双门噪声模型同样也分为上述几种：DAMPING_KRAUS_OPERATOR、DEPHASING_KRAUS_OPERATOR、DECOHERENCE_KRAUS_OPERATOR、DEPOLARIZING_KRAUS_OPERATOR、BITFLIP_KRAUS_OPERATOR、BIT_PHASE_FLIP_OPRATOR、PHASE_DAMPING_OPRATOR。
它们的输入参数与单门噪声模型一致，双门噪声模型的kraus算符和表示与单门噪声模型存在着对应关系：假设单门噪声模型为： :math:`\{ K1, K2 \}` ，那么对应的双门噪声模型为
:math:`\{K1\otimes K1, K1\otimes K2, K2\otimes K1, K2\otimes K2\}`。


接口介绍
------------

含噪声量子虚拟机的接口和其他量子虚拟机的接口大部分是相同的，但含噪声量子虚拟机不能使用PMEASURE系列的概率测量接口。
使用含噪声虚拟机时，只需要在初始化前设置一些量子逻辑门的噪声模型和对应的参数即可。

目前QPanda2中含噪声量子逻辑门支持的噪声模型有：

    .. code-block:: c

        enum NOISE_MODEL
        {            
            DAMPING_KRAUS_OPERATOR,
            DEPHASING_KRAUS_OPERATOR,
            DECOHERENCE_KRAUS_OPERATOR_P1_P2,
            BITFLIP_KRAUS_OPERATOR,
            DEPOLARIZING_KRAUS_OPERATOR,
            BIT_PHASE_FLIP_OPRATOR,
            PHASE_DAMPING_OPRATOR,
            DECOHERENCE_KRAUS_OPERATOR,
        };

设置一个参数的噪声模型：

    .. code-block:: c

        void set_noise_model(const NOISE_MODEL &model, const GateType &type, double prob)
        void set_noise_model(const NOISE_MODEL &model, const GateType &type, double prob, const QVec &qubits)
        void set_noise_model(const NOISE_MODEL &model, const GateType &type, double prob, const std::vector<QVec> &qubits)

        //设置线路中所有GateType噪声
        void set_noise_model(const NOISE_MODEL& model, const std::vector<GateType> &types, double prob)
        void set_noise_model(const NOISE_MODEL &model, const std::vector<GateType> &types, double T1, double T2, double t_gate)
        void set_noise_model(const NOISE_MODEL &model, const std::vector<GateType> &types, double T1, double T2,double t_gate, const QVec &qubits)

第一个参数为噪声模型类型，第二个参数为量子逻辑门类型，第三个参数为噪声模型所需的参数, 第四个参数是对单个比特设置噪声参数（包含单门和双门），若没有第四个参数则对所有的比特设置相应的噪声模型。

例如：

    .. code-block:: c

        NoiseQVM qvm;
        qvm.init();
        auto q = qvm.qAllocMany(4);
        auto c = qvm.cAllocMany(4);

        // X门所有比特设置比特反转噪声模型
        qvm.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, GateType::PAULI_X_GATE, 0.1);
        
        // H门作用在q0和q1上时设置去极化噪声模型
        QVec qv = {q[0], q[1]};
        qvm.set_noise_model(NOISE_MODEL::DEPHASING_KRAUS_OPERATOR, GateType::HADAMARD_GATE, 0.1, qv);

        // CNOT门作用在q0、q1和q1、q2上时设置幅值阻尼噪声模型
        std::vector<QVec> qves = {{q[0], q[1]}, {q[1], q[2]}};
        qvm.set_noise_model(NOISE_MODEL::DAMPING_KRAUS_OPERATOR, GateType::CNOT_GATE, 0.1, qves);

    .. code-block:: c

        void set_noise_model(const NOISE_MODEL &model, const GateType &type, double T1, double T2, double t_gate);
        void set_noise_model(const NOISE_MODEL &model, const GateType &type, double T1, double T2, double t_gate,
                             const QVec &qubits);
        void set_noise_model(const NOISE_MODEL &model, const GateType &type, double T1, double T2, double t_gate,
                             const std::vector<QVec> &qubits);

用法与上面的方法相同，只有噪声参数变为退相干的噪声的三个参数。

    .. code-block:: c

        void set_measure_error(const NOISE_MODEL &model, double prob, const QVec &qubits = {});
        void set_measure_error(const NOISE_MODEL &model, double T1, double T2, double t_gate,
                               const QVec &qubits = {});

用法类似于量子逻辑门的噪声模型，第一个参数为噪声模型类型，后面的参数和量子逻辑门的噪声参数。

    .. code-block:: c

        void set_reset_error(double p0, double p1, const QVec &qubits = {});

p0 表示重置到 :math:`\left|0\right\rangle`\ 的概率，p1表示重置到 :math:`\left|1\right\rangle`\ 的概率，未被重置的概率为 1-p0-p1。

    .. code-block:: c

        void set_readout_error(const std::vector<std::vector<double>> &probs_list, const QVec &qubits = {});

示例：

    .. code-block:: c

        double f0 = 0.9;
        double f1 = 0.85'
        noise_qm->set_readout_error({{f0, 1 - f0},{1 - f1, f1}}, {q[0]});

表示在读取q0时0读为0的概率为0.9，读为1的概率为1 - f0，
1读为1的概率为0.85，读为0的概率为1 - f1


含噪声虚拟机还支持设置设置带有角度的量子逻辑门的转转角度误差，其接口使用方式如下：

    .. code-block:: c

        qvm.set_rotation_error(0.05);

即设置角度旋转误差为0.05。


实例
----------------

    .. code-block:: c

        #include "QPanda.h"

        int main()
        {
            NoiseQVM qvm;
            qvm.init();
            auto q = qvm.qAllocMany(4);
            auto c = qvm.cAllocMany(4);

            qvm.set_noise_model(NOISE_MODEL::BITFLIP_KRAUS_OPERATOR, GateType::PAULI_X_GATE, 0.1);
            QVec qv0 = {q[0], q[1]};
            qvm.set_noise_model(NOISE_MODEL::DEPHASING_KRAUS_OPERATOR, GateType::HADAMARD_GATE, 0.1, qv0);
            std::vector<QVec> qves = {{q[0], q[1]}, {q[1], q[2]}};
            qvm.set_noise_model(NOISE_MODEL::DAMPING_KRAUS_OPERATOR, GateType::CNOT_GATE, 0.1, qves);

            double f0 = 0.9;
            double f1 = 0.85;
            qvm.set_readout_error({{f0, 1-f0}, {1-f1, f1}});
            qvm.set_rotation_error(0.05);

            QProg prog;
            prog << X(q[0]) << H(q[0])
                << CNOT(q[0], q[1])
                << CNOT(q[1], q[2])
                << CNOT(q[2], q[3])
                << MeasureAll(q, c);

            auto result = qvm.runWithConfiguration(prog, c, 1000);
            for (auto &item : result)
            {
                std::cout << item.first << " : " << item.second << std::endl;
            }

            return 0;
        }


运行结果：

    .. code-block:: c

        0000 : 341
        0001 : 82
        0010 : 37
        0011 : 41
        0100 : 37
        0101 : 16
        0110 : 15
        0111 : 28
        1000 : 48
        1001 : 23
        1010 : 19
        1011 : 29
        1100 : 16
        1101 : 51
        1110 : 46
        1111 : 171

