用I门填充QProg
===============

接口 ``fill_qprog_by_I`` 实现用I门填充QProg(量子程序)的功能。

实例
---------------

.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA

	int main()
	{
		auto qvm = initQuantumMachine(QMachineType::CPU);
		auto q = qvm->qAllocMany(4);
		auto c = qvm->cAllocMany(4);

		QCircuit cir;
		QProg prog;

		// 构建量子程序
		cir << CNOT(q[2], q[3]) 
			<< CU(1, 2, 3, 4, q[1], q[0])
			<< (H(q[1]))
			<< X(q[2]) 
			<< RZ(q[1], PI / 2)
			<< Y(q[2])
			<< (CR(q[0], q[3], PI / 2)) 
			<< (S(q[2]))
			<< S(q[1]) 
			<< RZ(q[1], PI / 2)
			<< Y(q[0]) 
			<< SWAP(q[3], q[1]);

		prog << cir << MeasureAll(q, c);

		// 输出原量子程序
		cout << "The source QProg:" << endl;
		cout << prog << endl;

		// 量子程序填充 I 门
		auto filled_prog = fill_qprog_by_I(prog);

		// 输出填充 I 门的量子程序
		cout << "The filled QProg:" << endl;
		cout << filled_prog << endl;

		destroyQuantumMachine(qvm);
		return 0;
	}
		
以上示例程序演示了 ``fill_qprog_by_I`` 接口的使用方法，我们可以看到只需要传入一个QProg类型的参数即可，该接口返回一个填充后的新QProg，输入QProg保持不变。
以上示例程序的字符画展示输出结果如下：

.. figure:: ./images/Filled_by_I.png
   :alt:
