量子程序转化QASM
=====================
----

通过该功能模块，你可以解析通过QPanda2构建的量子程序，将其中包含的量子比特信息以及量子逻辑门操作信息提取出来，得到按固定格式存储的QASM指令集。

.. _QASM介绍:

QASM介绍
>>>>>>>>>>>>>>>
----

QASM(Quantum Assembly Language)是IBM公司提出的量子汇编语言，与 :ref:`OriginIR介绍` 中的语法规则类似，一段QASM代码如下所示：

    :: 

        OPENQASM 2.0;
        include "qelib1.inc";
        qreg q[10];
        creg c[10];

        x q[0];
        h q[1];
        tdg q[2];
        sdg q[2];
        cx q[0],q[2];
        cx q[1],q[4];
        u1(pi) q[0];
        u2(pi,pi) q[1];
        u3(pi,pi,pi) q[2];
        cz q[2],q[5];
        ccx q[3],q[4],q[6];
        cu3(pi,pi,pi) q[0],q[1];
        measure q[2] -> c[2];
        measure q[0] -> c[0];


需要注意的是，QASM的语法格式与OriginIR形相似而神不同，主要区别有以下几点:

 - OriginIR对于需要进行转置共轭操作的量子逻辑门与量子线路，需要将目标置于DAGGER与ENDAGGER语句之间，而QASM会直接进行转化。
 - OriginIR支持对量子逻辑门与量子线路施加控制操作，而QASM不支持，在对量子程序转化QASM指令集之前，会对其中包含的控制操作进行分解。


QPanda2提供了QASM转换工具接口 ``std::string convert_qprog_to_qasm(QProg &, QuantumMachine*)`` 该接口使用非常简单，具体可参考下方示例程序。

实例
>>>>>>>>>>>>>>
----

下面的例程通过简单的接口调用演示了量子程序转化QASM指令集的过程

    .. code-block:: c

        #include "QPanda.h"
        USING_QPANDA

        int main(void)
        {
            auto qvm = CPUQVM();
            qvm.init();

            auto prog = QProg();
            auto cir = QCircuit();

            auto q = qvm.qAllocMany(6);
            auto c = qvm.cAllocMany(6);

            // 构建量子程序
            cir << Y(q[2]) << H(q[2]);
            cir.setDagger(true);
            auto h1 = H(q[1]);
            h1.setDagger(true);
            prog << H(q[1]) 
                 << X(q[2]) 
                 << h1 
                 << RX(q[1], 2 / PI) 
                 << cir 
                 << CR(q[1], q[2], PI / 2)
                 <<MeasureAll(q,c);

            // 量子程序转换QASM，并打印QASM
            std::cout << convert_qprog_to_qasm(prog, &qvm);

            return 0;
        }

具体步骤如下:

 - 首先在主程序中用 ``CPUQVM()`` 初始化一个量子虚拟机对象，用于管理后续一系列行为

 - 然后调用init()函数来初始化虚拟机

 - 接着用 ``qAllocMany()`` 和 ``cAllocMany()`` 初始化量子比特与经典寄存器数目

 - 然后调用 ``QProg()`` 构建量子程序

 - 最后调用接口 ``convert_qprog_to_qasm`` 输出QASM指令集并用 ``destroyQuantumMachine`` 释放系统资源


运行结果如下：

    .. code-block:: c

        OPENQASM 2.0;
        include "qelib1.inc";
        qreg q[6];
        creg c[6];
        h q[1];
        x q[2];
        h q[1];
        rx(0.636620) q[1];
        h q[2];
        y q[2];
        rz(-0.785398) q[2];
        cx q[1],q[2];
        rz(-0.785398) q[2];
        cx q[1],q[2];
        rz(1.570796) q[2];
        rx(1.570796) q[1];
        ry(-0.785398) q[1];
        rx(-1.570796) q[1];
        measure q[0] -> c[0];
        measure q[1] -> c[1];
        measure q[2] -> c[2];
        measure q[3] -> c[3];
        measure q[4] -> c[4];
        measure q[5] -> c[5];
