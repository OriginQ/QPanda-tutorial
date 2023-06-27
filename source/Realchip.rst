真实芯片计算服务
=============================
----

本源悟源超导芯片
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

``本源悟源`` 是2020年9月12日本源量子自主研发的超导量子计算机（搭载6比特超导量子处理器夸父 KF C6-130）。得益于本源超导量子计算云平台，量子计算机可以走出实验室，为众多潜在行业提供探索量子计算的基础条件，推进量子计算产业落地与工程化发展，真正为人类社会服务。

超导量子计算云平台作为连接用户和量子计算系统之间的桥梁，在用户向量子系统发起计算任务到量子系统完成计算任务后返回计算结果过程中，发挥着重要的协调中转作用。

本源悟源的 ``芯片拓扑结构图`` 如下：

.. image:: images/tuopu.png
   :align: center

对应的 ``芯片参数`` 信息如下图：

.. image:: images/param.png
   :align: center

接口介绍如下：

    - 1. **蒙特卡洛测量接口：**  ``real_chip_measure`` ,使用示例如下：
 
    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            //通过QCloudMachine创建量子云虚拟机
            QCloudMachine QCM;;

            //通过传入当前用户的token来初始化
            QCM.init("302e020100301006072a8648ce3d020106052b8104001c041730150201010410634a5b6d0a2a9a2b03b9d7c17c57405f/13082", true);
            auto q = QCM.allocateQubits(6);
            auto c = QCM.allocateCBits(6);

            //构建量子程序
            auto measure_prog = QProg();
            measure_prog << HadamardQCircuit(q)
                        << RX(q[1], PI / 4)
                        << RX(q[2], PI / 4)
                        << RX(q[1], PI / 4)
                        << CZ(q[0], q[1])
                        << CZ(q[1], q[2])
                        << Measure(q[0], c[0])
                        << Measure(q[1], c[1]);

            //调用真实芯片计算接口，至少需要量子程序和测量次数两个参数，后面的三个默认参数依次为芯片类型，是否开启线路映射与线路优化功能。
            auto result = QCM.real_chip_measure(measure_prog, 1000, RealChipType::ORIGIN_WUYUAN_D4,true,true);
            for (auto val : result)
            {
                cout << val.first << " : " << val.second << endl;
            }

            QCM.finalize();
            return 0;
        }

    上述过程需要注意的是， ``init`` 需要用户传入量子云平台用户验证标识token，可以从本源量子云平台个人信息下获取，具体见下方截图。

        .. image:: images/token.png
           :align: center  

    输出结果如下，左侧是量子态的二进制表示，右边表示测量次数对应的概率：
            
    .. code-block:: c

        00 : 0.25849
        01 : 0.235175
        10 : 0.248353
        11 : 0.257983

    - 2. **获取量子态qst层析结果接口：**  ``get_state_tomography_density`` ,使用示例如下：
 
    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            //通过QCloudMachine创建量子云虚拟机
            QCloudMachine QCM;;

            //通过传入当前用户的token来初始化
            QCM.init("302e020100301006072a8648ce3d020106052b8104001c041730150201010410634a5b6d0a2a9a2b03b9d7c17c57405f/13082", true);
            auto q = QCM.allocateQubits(6);
            auto c = QCM.allocateCBits(6);

            //构建量子程序
            auto measure_prog = QProg();
            measure_prog << HadamardQCircuit(q)
                        << RX(q[1], PI / 4)
                        << RX(q[2], PI / 4)
                        << RX(q[1], PI / 4)
                        << CZ(q[0], q[1])
                        << CZ(q[1], q[2])
                        << Measure(q[0], c[0])
                        << Measure(q[1], c[1]);

            //调用真实芯片计算接口，至少需要量子程序和测量次数两个参数，后面的三个默认参数依次为芯片类型，是否开启线路映射与线路优化功能。
            auto result = QCM.get_state_tomography_density(measure_prog, 1000, RealChipType::ORIGIN_WUYUAN_D4);
            for (auto val : result)
            {
                cout << val << endl;
            }

            QCM.finalize();
            return 0;
        }

    输出结果如下：
            
    .. code-block:: c

        (0.270653826659909, 0)(0.210086163203244, -0.018499746578814)(-0.00228079067410038, -0.0114039533705018)(-0.00126710593005575, -0.0103902686264572)
        (0.210086163203244, 0.018499746578814)(0.225038013177902, 0)(0.00202736948808921, 0.00456158134820069)(0.0187531677648251, -0.00304105423213379)
        (-0.00228079067410038, 0.0114039533705018)(0.00202736948808921, -0.00456158134820069)(0.26862645717182, 0)(-0.207298530157121, -0.0146984287886467)
        (-0.00126710593005575, 0.0103902686264572)(0.0187531677648251, 0.00304105423213379)(-0.207298530157121, 0.0146984287886467)(0.23568170299037, 0)

    - 3. **获取量子态保真度接口：**  ``get_state_fidelity`` ,使用示例如下：
 
    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            //通过QCloudMachine创建量子云虚拟机
            QCloudMachine QCM;;

            //通过传入当前用户的token来初始化
            QCM.init("302e020100301006072a8648ce3d020106052b8104001c041730150201010410634a5b6d0a2a9a2b03b9d7c17c57405f/13082", true);
            auto q = QCM.allocateQubits(6);
            auto c = QCM.allocateCBits(6);

            //构建量子程序
            auto measure_prog = QProg();
            measure_prog << HadamardQCircuit(q)
                        << RX(q[1], PI / 4)
                        << RX(q[2], PI / 4)
                        << RX(q[1], PI / 4)
                        << CZ(q[0], q[1])
                        << CZ(q[1], q[2])
                        << Measure(q[0], c[0])
                        << Measure(q[1], c[1]);

            //调用真实芯片计算接口，至少需要量子程序和测量次数两个参数，后面的三个默认参数依次为芯片类型，是否开启线路映射与线路优化功能。
            auto result = QCM.get_state_fidelity(measure_prog, 1000, RealChipType::ORIGIN_WUYUAN_D4);
            cout << result << endl;

            QCM.finalize();
            return;
        }

    输出结果如下：
            
    .. code-block:: c

        0.942748

    在使用本源悟源真实芯片测量操作时，经常会遇到各种错误，下面给出部分错误信息，可以根据抛出的错误异常信息进行对号入座。

    -  ``server connection failed`` ：该异常表示服务器宕机或与服务器连接失败
    -  ``api key error`` ：该异常表示用户的API-Key参数异常，请去官网确认个人资料的信息
    -  ``un-activate products or lack of computing power`` ：该异常表示用户未开通该产品或算力不足
    -  ``build system error`` ：该异常表示编译系统运行出错
    -  ``exceeding maximum timing sequence`` ：该异常表示量子程序时序过长
    -  ``unknown task status`` ：其他任务状态异常的情况

.. note:: 
            - 使用对应的计算接口时，需要确认当前用户已经开通了该产品，否则可能会导致提交计算任务失败。
            - 在噪声模拟时，退相干的单门噪声和双门参数参数分别有3个，不同于其他噪声
            - 本源悟源测量操作支持的测量次数范围在1000至10000之间，且目前仅支持6及以下量子比特的量子线路模拟，未来会加入其他的量子芯片，敬请期待。
            - 在使用时遇到任何问题，请给我们提交 `用户反馈 <https://qcloud.qubitonline.cn/userFeedback>`_ ，我们看到后会尽快解决你的问题
