本源高性能计算集群云服务
=================================
----

本源量子的高性能计算集群提供多种功能强大的虚拟机计算后端，适用于不同情况下的量子线路模拟需求，完整示例程序介绍如下：

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main()
        {
            /*需下载curl并将其加入环境变量
            通过QCloudMachine创建量子云虚拟机*/
            QCloudMachine QCM;

            //通过传入当前用户的token来初始化
            QCM.init("3B1AC640AAC248C6A7EE4E8D8537370D");
            auto qlist = QCM.allocateQubits(6);
            auto clist = QCM.allocateCBits(6);

            //构建量子程序
            auto measure_prog = QProg();
            measure_prog << HadamardQCircuit(qlist)
                            << CZ(qlist[1], qlist[5])
                            << CZ(qlist[0], qlist[4])
                            << RX(qlist[2], PI / 4)
                            << RX(qlist[1], PI / 4)
                            << CZ(qlist[2], qlist[3])
                            << Measure(qlist[0], clist[0])
                            << Measure(qlist[1], clist[1])
                            << Measure(qlist[2], clist[2]);

            auto pmeasure_prog = QProg();
            pmeasure_prog << HadamardQCircuit(qlist)
                            << CZ(qlist[1], qlist[5])
                            << RX(qlist[2], PI / 4)
                            << RX(qlist[1], PI / 4);

            //调用全振幅蒙特卡洛测量操作接口，需要量子程序和测量次数两个参数
            auto result0 = QCM.full_amplitude_measure(measure_prog, 100);
            for (auto val : result0)
            {
                std::cout << val.first << " : " << val.second << std::endl;
            }
            
            QCM.finalize();
            return 0;
        }


全振幅模拟云计算
>>>>>>>>>>>>>>>>>>

    - ``full_amplitude_measure(全振幅蒙特卡洛测量操作)`` ：

        .. code-block:: c

            auto result0 = QCM.full_amplitude_measure(measure_prog, 100);
            for (auto val : result0)
            {
                std::cout << val.first <<" : "<< val.second << std::endl;
            }
        
        输出结果如下，左侧是量子态的二进制表示，右边表示测量次数对应的概率：
        
        .. code-block:: c

            000 : 0.12
            001 : 0.14
            010 : 0.15
            011 : 0.12
            100 : 0.11
            101 : 0.11
            110 : 0.11
            111 : 0.14

    - ``full_amplitude_pmeasure(全振幅概率测量操作)`` ：

        .. code-block:: c

            auto result1 = QCM.full_amplitude_pmeasure(pmeasure_prog, { 0, 1, 2 });
            for (auto val : result1)
            {
                std::cout << val.first << " : " << val.second << std::endl;
            }

        需要传入的第二个参数是测量的比特，输出结果如下，左侧是量子态的二进制表示，右边表示测量对应的概率：

        .. code-block:: c

            000 : 0.125
            001 : 0.125
            010 : 0.125
            011 : 0.125
            100 : 0.125
            101 : 0.125
            110 : 0.125
            111 : 0.125

部分振幅模拟云计算
>>>>>>>>>>>>>>>>>>

    - ``partial_amplitude_pmeasure(部分振幅概率测量操作)`` ：

        .. code-block:: c

            auto result2 = QCM.partial_amplitude_pmeasure(pmeasure_prog, { "0", "1", "2"});
            for (auto val : result2)
            {
                std::cout << val.first << " : " << val.second << std::endl;
            }
        
        需要传入的第二个参数是测量的量子态振幅的十进制表示，输出结果如下，左侧是量子态振幅的十进制表示，右边表示复数形式的振幅值：
        
        .. code-block:: c

            0 : (0.0883883,-0.0883883)
            1 : (0.0883883,-0.0883883)
            2 : (0.0883883,-0.0883883)

单振幅云计算
>>>>>>>>>>>>>>>>>>

    - ``single_amplitude_pmeasure(单振幅概率测量操作)`` ：

        .. code-block:: c

            auto result3 = QCM.single_amplitude_pmeasure(pmeasure_prog, "0");
            std::cout << "0" << " : " << result3 << std::endl;
        
        需要传入的第二个参数是测量的振幅（十进制表示），输出结果如下，只会输出一个量子态对应的复数形式的振幅值：
        
        .. code-block:: c

            0 : (0.0883883,-0.0883883)

噪声模拟云计算
>>>>>>>>>>>>>>>>>>

    - ``noise_measure(噪声虚拟机测量操作)`` ：

        .. code-block:: c

            QCM.set_noise_model(NOISE_MODEL::BIT_PHASE_FLIP_OPRATOR, { 0.01 }, { 0.02 });
            auto result4 = QCM.noise_measure(measure_prog, 100);
            for (auto val : result4)
            {
                std::cout << val.first << " : " << val.second << std::endl;
            }
        
        通过 ``set_noise_model`` 设置噪声参数，第一个参数是噪声模型，后面分别是单门噪声参数和双门噪声参数，噪声模型的定义如下：

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
                PAULI_KRAUS_MAP,
                KRAUS_MATRIX_OPRATOR,
                MIXED_UNITARY_OPRATOR,
            };

        该接口输出结果如下，左侧是量子态的二进制表示，右边表示测量对应的概率：
        
        .. code-block:: c

            000 : 0.10
            001 : 0.08
            010 : 0.13
            011 : 0.08
            100 : 0.20
            101 : 0.23
            110 : 0.08
            111 : 0.10

.. note:: 
            - 使用对应的计算接口时，需要确认当前用户已经开通了该产品，否则可能会导致提交计算任务失败。
            - 在噪声模拟时，退相干的单门噪声和双门参数参数分别有3个，不同于其他噪声
            - 本源悟源测量操作支持的测量次数范围在1000至10000之间，且目前仅支持6及以下量子比特的量子线路模拟，未来会加入其他的量子芯片，敬请期待。
            - 在使用时遇到任何问题，请给我们提交 `用户反馈 <https://qcloud.qubitonline.cn/userFeedback>`_ ，我们看到后会尽快解决你的问题
