.. _QuantumMachine:

全振幅量子虚拟机
====================

全振幅量子虚拟机一次可以模拟计算出量子态的所有振幅，计算方式支持CPU、单线程计算和GPU，可以在初始化时配置，使用方式是完全一样的，只是其计算效率不同。

接口介绍
----------------

全振幅量子虚拟机类型：

.. code-block:: c

    enum QMachineType {
        CPU,  /**< Cpu quantum machine  */
        GPU, /**< Gpu quantum machine  */
        CPU_SINGLE_THREAD, /**< Cpu quantum machine with single thread */
        NOISE  /**< Cpu quantum machine with  noise */
    };

QPanda2中在构造量子虚拟机时有以下几种方式：

    .. code-block:: c

        init(QMachineType::CPU);  // 使用init,不会返回qvm，会在代码中生成一个全局的qvm
        auto qvm = initQuantumMachine(QMachineType::CPU); // 通过接口得到qvm指针
        CPUQVM *qvm = new CPUQVM; // 直接new一个需要qvm类

.. note:: ``init`` 和 ``initQuantumMachine`` 这两个函数不是线程安全的，不适用于多线程编程，而且其最大的量子比特个数和经典寄存器个数均为默认值25。

设置量子虚拟机的配置(当前配置只有最大量子比特个数和最大经典寄存器个数):

    .. code-block:: c

        Configuration conf;
        conf.maxQubit = 30;
        conf.maxCMem = 30;
        qvm->setConfigure(conf);

.. note:: 量子虚拟机默认的最大量子比特个数和经典寄存器个数均为25。

设置好配置之后要初始化量子虚拟机：

    .. code-block:: c

        qvm->init();

.. note:: 调用 ``init`` 和 ``initQuantumMachine`` 接口， 就不需要初始化了。

下面我们就需要去申请量子比特和经典寄存器。

例如我们申请4个量子比特：

    .. code-block:: c

        QVec qubits = qvm->qAllocMany(4);

申请一个量子比特时也可以用这个接口：

    .. code-block:: c

        Qubit* qubit = qvm->qAlloc();

如果我们想在固定的量子比特虚拟地址上申请一个量子比特可以用下面的方法：

    .. code-block:: c

        Qubit* qubit = qvm->allocateQubitThroughVirAddress(0x01);

申请经典寄存器也有类似于申请量子比特的接口，其使用方法和申请量子比特的方法一样，如申请4个经典寄存器的方法：

    .. code-block:: c

        std::vector<ClassicalCondition> cbits = qvm->cAllocMany(4);

申请一个经典寄存器时也可以用这个接口：

    .. code-block:: c

        ClassicalCondition cbit = qvm->cAlloc();

固定的经典寄存器虚拟地址上申请一个量子比特可以用下面的方法：

    .. code-block:: c

        ClassicalCondition cbit = qvm->cAlloc(0x01);

在一个量子虚拟机中，申请了几次量子比特或经典寄存器，我们想知道一共申请了多少个量子比特或经典寄存器可以用下面的方法：

    .. code-block:: c

        size_t num_qubit = qvm->getAllocateQubitNum(); // 申请量子比特的个数
        size_t num_cbit = qvm->getAllocateCMemNum(); // 申请经典寄存器的个数

我们该如何使用量子虚拟机来执行量子程序呢？ 可以用下面的方法：

    .. code-block:: c

        QProg prog;
        prog << H(qubits[0])
            << CNOT(qubits[0], qubits[1])
            << Measure(qubits[0], cbits[0]); // 构建一个量子程序
        
        map<string, bool> result = qvm->directlyRun(prog); // 执行量子程序

如果想多次运行一个量子程序，并得到每次量子程序的结果，除了循环调用 ``directlyRun`` 方法外， 我们还提供了一个接口 ``runWithConfiguration`` 。
``runWithConfiguration`` 有两个重载方法，一个是int类型的配置参数，另一个是rapidjson::Document类型的配置参数。其中int类型的配置参数用法如下：
      .. code-block:: c

        int shots = 1000;
        qvm->runWithConfiguration(prog, cbits, shots);

如果想得到量子程序运行之后各个量子态的振幅值，可以调用 ``getQState`` 函数获得：

    .. code-block:: c

        QStat stat = qvm->getQState();

量子虚拟机中测量和概率使用方法与 :ref:`Measure` 和 :ref:`PMeasure` 中介绍的相同，在这里就不多做赘述。

实例1
-----------------

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            CPUQVM qvm;
            qvm.init();
            auto qubits = qvm.qAllocMany(4);
            auto cbits = qvm.cAllocMany(4);

            // 构建量子程序
            QProg prog;
            prog << H(qubits[0])
                << CNOT(qubits[0], qubits[1])
                << CNOT(qubits[1], qubits[2])
                << CNOT(qubits[2], qubits[3])
                << Measure(qubits[0], cbits[0]);

            // 量子程序运行1000次，并返回测量结果
            auto result = qvm.runWithConfiguration(prog, cbits, 1000);

            // 打印量子态在量子程序多次运行结果中出现的次数
            for (auto &val : result)
            {
                std::cout << val.first << ", " << val.second << std::endl;
            }

            qvm.finalize();
            return 0;
        }

运行结果：

    .. code-block:: c

        0000, 498
        0001, 502

.. note:: 这个量子程序的运行结果是不确定的，但其 ``0000`` 和 ``0001`` 对应的值都应该在500左右。

实例2
------------------

    .. code-block:: c

        #include <QPanda.h>
        USING_QPANDA

        int main(void)
        {
            init();
            auto qubits = qAllocMany(4);
            auto cbits = cAllocMany(4);

            //构建量子程序
            QProg prog;
            prog << H(qubits[0])
                << CNOT(qubits[0], qubits[1])
                << CNOT(qubits[1], qubits[2])
                << CNOT(qubits[2], qubits[3])
                << Measure(qubits[0], cbits[0]);

            auto result = directlyRun(prog);
            for (auto &val : result)
            {
                std::cout << val.first << ", " << val.second << std::endl;
            }

            finalize();
            return 0;
        }

运行结果：

    .. code-block:: c

        c0, 1
