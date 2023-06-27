量子线路字符画
===============

接口 ``draw_qprog()`` 可以将输入的量子程序转换为字符画并输出到控制台同时将字符画信息保存到文件（QCircuitTextPic.txt，该接口会在当前程序运行目录下创建该txt文件，该文件用utf8编码，并覆盖之前数据），
接口详细说明如下:

::

    /**
    * @brief output a quantum prog/circuit to console by text-picture(UTF-8 encode),
             and will save the text-picture in file named QCircuitTextPic.txt in the same time in current path.
    * @param[in] prog  the source prog
    * @param[in] itr_start The start pos, default is the first node of the prog
    * @param[in] itr_end The end pos, default is the end node of the prog
    * @return the output string
    * @ Note: All the output characters are UTF-8 code.
    */
    std::string draw_qprog(QProg &prog, const NodeIter itr_start = NodeIter(), const NodeIter itr_end = NodeIter());
    

实例
---------------

.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA

    int main(void)
    {
        auto qvm = CPUQVM();
		qvm.init();
        auto q = qvm.qAllocMany(3);
        auto c = qvm.cAllocMany(3);
        QProg prog;
        QCircuit cir1, cir2;

        // 构建量子程序
        auto gate = S(q[1]);
        gate.setDagger(true);
        cir1 << H(q[0]) << S(q[2]) << CNOT(q[0], q[1]) << CZ(q[1], q[2]) << gate;
        cir1.setDagger(true);
        cir2 << cir1 << CU(1, 2, 3, 4, q[0], q[2]) << S(q[2]) << CR(q[2], q[1], PI / 2);
        cir2.setDagger(true);
        prog << cir2 << MeasureAll(q, c);

        // 量子程序字符画
        std::string text_picture = draw_qprog(prog);

        #if defined(WIN32) || defined(_WIN32)
        text_picture = fit_to_gbk(text_picture);
        text_picture = Utf8ToGbkOnWin32(text_picture.c_str());
        #endif

        // 打印字符画
        std::cout << text_picture << std::endl;
        return 0;
    }

以上示例演示了draw_qprog这个接口的使用方法，上述代码的输出结果如下：

.. figure:: ./images/draw_prog.png
   :alt:

在实际使用过程中，为了方便调用，我们重载了标准输出std::cout，所以以下两部分代码是等价的：

::

    //普通方法打印字符画
    string text_picture = draw_qprog(prog);
    cout << text_picture << endl;
    
    //通过重载cout，进行字符画打印
    cout << prog << endl;