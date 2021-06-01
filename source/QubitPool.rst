
量子比特池
==========================

简介
--------------
QPanda之前版本中量子比特和经典寄存器都是通过虚拟机进行申请，管理，控制。
现在提供独立于虚拟机的方法，即量子比特、经典寄存器不通过虚拟机管理，可以由提供的比特池直接申请、释放。
为了更好的使用量子比特和经典寄存器，我们进一步支持以物理地址代表相应比特使用。在 ``Measure``

接口说明
--------------
量子比特池：
- ``OriginQubitPool::get_instance()`` 获取单例的量子比特池， 通过该池对象申请释放量子比特。
``get_capacity`` 获取最大容量
``set_capacity`` 设置容量
``get_qubit_by_addr`` 通过物理地址获取量子比特

经典寄存器池：
``OriginCMem::get_instance()`` 获取单例的经典寄存器池，通过该池对象申请释放经典寄存器。
``get_capacity`` 获取最大容量
``set_capacity`` 设置容量
``get_cbit_by_addr`` 通过物理地址获取量子比特

由于申请释放方法均和虚拟机提供的方法相同。 在 :ref:`QuantumMachine` 中有详细介绍。

同时对于量子比特和经典寄存器的使用，现在也可以直接通过对应比特的地址传参。
例如 :
``H(1)`` 可以理解在物理地址为1的量子比特上作用H门。
``Measure(1, 1)`` 可以理解在物理地址为1的量子比特施加Meausre测量，并将结果保存在地址为1的经典寄存器上。


实例
--------------
.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA
    using namespace std;
    int main()
    {
        // 量子比特可以和虚拟机 脱离关系，获取对应池的单例
        auto qpool = OriginQubitPool::get_instance();
        auto cmem = OriginCMem::get_instance();

        //获取容器大小
        cout << "set qubit pool capacity  before: "<< qpool->get_capacity() << endl;
        // 设置最大容器
        qpool->set_capacity(20);
        cout << "set qubit pool capacity  after: " << qpool->get_capacity() << endl;

        // 通过比特池申请比特，由于是单例模式，要保证申请的比特数量不超过最大容量
        auto qv = qpool->qAllocMany(6);
        auto cv = cmem->cAllocMany(6);

        // 获取被申请的量子比特
        QVec used_qv;
        auto used_qv_size = qpool->get_allocate_qubits(used_qv);
        cout << "allocate qubits number: " << used_qv_size << endl;

        // 构建虚拟机
        auto qvm = new CPUQVM();
        qvm->init();
        auto prog = QProg();
        // 直接使用物理地址作为量子比特信息入参
        prog << H(0) << H(1)
            << H(2)
            << H(4)
            << X(5)
            << X1(2)
            << CZ(2, 3)
            << RX(3, PI / 4)
            << CR(4, 5, PI / 2)
            << SWAP(3, 5)
            << CU(1, 3, PI / 2, PI / 3, PI / 4, PI / 5)
            << U4(4, 2.1, 2.2, 2.3, 2.4)
            << BARRIER({0, 1,2,3,4,5})
            ;

        // 测量方法也可以使用比特物理地址 
        auto res_0 = qvm->probRunDict(prog, { 0,1,2,3,4,5 });
        // auto res_1 = qvm->probRunDict(prog, qv);  //同等上述方法
   

        // 同样经典比特地址也可以作为经典比特信息入参
        prog << Measure(0, 0)
            << Measure(1, 1)
            << Measure(2, 2)
            << Measure(3, 3)
            << Measure(4, 4)
            << Measure(5, 5)
            ;

        // 使用经典比特地址入参 
        vector<int> cbit_addrs = { 0,1,2,3,4,5 };
        auto res_2 = qvm->runWithConfiguration(prog, cbit_addrs, 5000);
        // auto res_3 = qvm->runWithConfiguration(prog, cv, 5000); //同等上述方法
        qvm->finalize();
        delete(qvm);

        
        // 同时我们还可以再次利用这里申请的qv，避免多次使用虚拟机多次申请比特的问题发生
        auto qvm_noise = new NoiseQVM();
        qvm_noise->init();
        auto res_4 = qvm_noise->runWithConfiguration(prog, cbit_addrs, 5000);
        qvm_noise->finalize();
        delete(qvm_noise);
        
        return 0;
    }
    
运行结果：
::

    set qubit pool capacity  before: 29
    set qubit pool capacity  after: 20
    allocate qubits number: 6

