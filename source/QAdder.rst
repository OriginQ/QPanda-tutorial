量子加法器
====================
量子加法器（QAdder）是在量子线路中实现量子态加法的运算器。

接口介绍
---------
在QPanda中我们实现了上述算法，使用该算法必须包含QPanda命名空间 ``QPanda``，详见 ``ArithmeticUnit.h`` 。
主要接口包括量子加法器 ``QAdder`` 、判断最终结果是否有进位项 ``isCarry`` 以及忽略最终进位项的加法器 ``QAdderIgnoreCarry`` 。

在量子线路中实现加法功能的接口 ``QAdder`` 如下：

    .. code-block:: c

        prog << QAdder(a, b, c, is_carry);

可以看出,QAdder接受4个参数，a为加数1（多量子比特）、b为加数2（多量子比特）、c为辅助比特，用于保存运算过程中的进位项、
is_carry为辅助比特，用于保存最终结果的进位项；返回值为量子线路（QCircuit）。

除此之外，还有判断最终结果是否有进位项的接口  ``isCarry``：

    .. code-block:: c

        prog << isCarry(a, b, c, is_carry);

``isCarry`` 也是接受4个参数，a为加数1（多量子比特）、b为加数2（多量子比特）、c为辅助比特，用于保存运算过程中的进位项、
is_carry为辅助比特，用于保存最终结果的进位项；返回值为量子线路（QCircuit）。

还有忽略最终进位项的加法器 ``QAdderIgnoreCarry`` 的接口：

    .. code-block:: c

        prog << QAdderIgnoreCarry(a, b, c);

``QAdderIgnoreCarry`` 接受3个参数，a为加数1（多量子比特）、b为加数2（多量子比特）、c为辅助比特，用于保存运算过程中的进位项；返回值为量子线路（QCircuit）。



实例
--------
    \|a\> = \|011\>, \|b\> = \|111\>

    - QAdder: \|a\> + \|b\> -> \|1010\>;
    - isCarry: \|a\> + \|b\> -> \|1\>;
    - QAdderIgnoreCarry: \|a\> + \|b\> -> \|010\>;

实例代码如下：

运用接口量子加法器的示例代码

.. code-block:: c

    #include "QPanda.h"
    #include "Components/ArithmeticUnit/ArithmeticUnit.h"
    using namespace std;

    int main(int argc, char **argv) {

        auto qvm = initQuantumMachine();

        auto a = qvm->allocateQubits(3);
        auto b = qvm->allocateQubits(3);
        Qubit *c = qvm->allocateQubit();
        Qubit *is_carry = qvm->allocateQubit();
        QProg prog;
        prog << X(a[0]) << X(a[1])
            << X(b[0]) << X(b[1]) << X(b[2])
            << QAdder(a, b, c, is_carry);
            //<< isCarry(a, b, c, is_carry);
            //<< QAdderIgnoreCarry(a, b, c);

        qvm->directlyRun(prog);
        auto temp = dynamic_cast<IdealMachineInterface *>(qvm);

        //auto result = temp->quickMeasure(b , 1000);
        //auto result = temp->quickMeasure({ is_carry }, 1000);
        auto result = temp->quickMeasure(a, 1000);
        for (auto &val : result)
        {
            std::cout << val.first << ", " << val.second << std::endl;
        }

        destroyQuantumMachine(qvm);

        system("pause");
        return 0;
    }

计算结果：

    .. code-block:: c

        010, 1000

.. note:: 由于量子加法器QAdder是可逆线路，最后除去进位项（如果有）的结果保存在加数1（adder1）对应的比特上面，加数2（adder2）保持不变，辅助比特is_carry用于保存最终结果的进位项。

