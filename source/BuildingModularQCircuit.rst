.. _构建模块化的量子线路:

构建模块化的量子线路
===================

在比特数量比较多，量子算法比较复杂的情况下，可能我们需要把多个比较小的量子线路组成成一整个大的量子程序。

QPanda-2可以以一种比较方便的模式去构建这种模块。


用于生成量子线路（量子程序）的函数
----------------------------------

QPanda中最常见的做法是用C++函数来定义一个量子线路模块。它通常具有一个QCircuit或者QProg类型的返回值。例如


     .. code-block:: c

            QCircuit foo(Qubit* qubit1, Qubit* qubit2)
            {
                QCircuit cir;
                cir << H(qubit2) << CNOT(qubit1, qubit2) << H(qubit2);
                return cir;
            }

这样的一个函数代表了一个模块（如图），当以不同的qubit1和qubit2作为输入的时候，它相当于把这个模块放置在了量子线路的不同位置


.. image:: images/QCircuit_cir.png
    :align: center   


Qubit分配（qAlloc）与映射
----------------------------------

QPanda-2中量子比特是用一个Qubit*的指针对象进行表示的。Qubit本身不包含任何和量子态相关的数据，它只是一个用于映射物理量子比特的对象。

qAlloc这个函数可以从量子芯片未用到的量子比特池中申请一个量子比特。qAllocMany则可以申请到一批。

示例：

     .. code-block:: c

            Qubit* q=qAlloc();
            QVec qs=qAllocMany(3);

如图：

.. image:: images/Qubit_Maping.png
    :align: center   

在任何时候Qubit * 类型的对象（或者Qvec容器中包含的每一个Qubit*）对象，都是映射到量子芯片上一个位置。
在一开始申请的时候，用户无需指定这种映射关系（通过allocateQubitThroughPhyAddress可以进行手动指定），程序后面可以通过自动的优化器来根据量子程序进行重新映射，以便得到最简的量子程序。

使用编写好的模块
-------------------

前面写好的foo，就可以被用于不同的量子比特上，以构建一个更大的量子程序。例如我们可以把这一段线路作用在q和qs上：

     .. code-block:: c

            QProg prog;
            prog << foo(q, qs[0]) << foo(qs[1],qs[2]) << foo(qs[2], q);


这样，这个量子程序对应了下面这个量子线路：

.. image:: images/QCircuit_cir_2.png
    :align: center   


利用QVec（vector<Qubit*>)构建模块的方式
------------------------------------------

QVec继承了vector<Qubit*>类，因此它可以覆盖所有vector所包含的功能（operator[]，size()，push_back，iterator……），当然也可以利用C++11的新式for循环。

下面这个程序利用了一组量子比特（数量不定）去构建一个量子线路，对这组量子比特中每一个，都作用一个Hadamard门。

     .. code-block:: c

            QCircuit foo2(QVec qs)
            {
                QCircuit cir;
                for (auto qubit: qs){
                    cir << H(q);
                }
                return cir;
            }

如果qs中只有一个量子比特，那这个线路就是：

.. image:: images/QVec_Example.png
    :align: center  

如果qs中有N个量子比特，那这个线路自然就是：

.. image:: images/QVec_Example_2.png
    :align: center  

请问：下面这个量子程序代表了一个什么样的模块呢？

     .. code-block:: c

            QCircuit foo2(QVec qs)
            {
                QCircuit cir;
                cir << H(q[0]);
                for (int i=1;i<qs.size();++i)
                {
                    cir << CNOT(q[i-1], q[i]);
                }
                return cir;
            }

答案是如图所示：

.. image:: images/QVec_Example_3.png
    :align: center  

