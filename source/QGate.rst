量子逻辑门
====================
----

经典计算中，最基本的单元是比特，而最基本的控制模式是逻辑门。我们可以通过逻辑门的组合来达到我们控制电路的目的。类似地，处理量子比特的方式就是量子逻辑门。
使用量子逻辑门，我们有意识的使量子态发生演化。所以量子逻辑门是构成量子算法的基础。

量子逻辑门由酉矩阵表示。最常见的量子门在一个或两个量子位的空间上工作，就像常见的经典逻辑门在一个或两个位上操作一样。

常见量子逻辑门矩阵形式
--------------------------------------

.. |I| image:: images/QGate_I.png
   :width: 50px
   :height: 50px

.. |H| image:: images/QGate_H.png
   :width: 50px
   :height: 50px

.. |T| image:: images/QGate_T.png
   :width: 50px
   :height: 50px

.. |S| image:: images/QGate_S.png
   :width: 50px
   :height: 50px

.. |X| image:: images/QGate_X.png
   :width: 50px
   :height: 50px

.. |Y| image:: images/QGate_Y.png
   :width: 50px
   :height: 50px
   
.. |Z| image:: images/QGate_Z.png
   :width: 50px
   :height: 50px

.. |X1| image:: images/QGate_X1.png
   :width: 50px
   :height: 50px

.. |Y1| image:: images/QGate_Y1.png
   :width: 50px
   :height: 50px
   
.. |Z1| image:: images/QGate_Z1.png
   :width: 50px
   :height: 50px

.. |RX| image:: images/QGate_RX.png
   :width: 50px
   :height: 50px

.. |RY| image:: images/QGate_RY.png
   :width: 50px
   :height: 50px

.. |RZ| image:: images/QGate_RZ.png
   :width: 50px
   :height: 50px

.. |U1| image:: images/QGate_U1.png
   :width: 50px
   :height: 50px

.. |U2| image:: images/QGate_U2.png
   :width: 50px
   :height: 50px

.. |U3| image:: images/QGate_U3.png
   :width: 50px
   :height: 50px

.. |U4| image:: images/QGate_U4.png
   :width: 50px
   :height: 50px

.. |CNOT| image:: images/QGate_CNOT.png
   :width: 50px
   :height: 50px

.. |CR| image:: images/QGate_CR.png
   :width: 50px
   :height: 50px

.. |iSWAP| image:: images/QGate_iSWAP.png
   :width: 50px
   :height: 50px

.. |SWAP| image:: images/QGate_SWAP.png
   :width: 50px
   :height: 50px

.. |CZ| image:: images/QGate_CZ.png
   :width: 50px
   :height: 50px

.. |CU| image:: images/QGate_CU.png
   :width: 50px
   :height: 50px

.. |RXX| image:: images/QGate_RXX.png
   :width: 50px
   :height: 50px

.. |RYY| image:: images/QGate_RYY.png
   :width: 50px
   :height: 50px

.. |RZZ| image:: images/QGate_RZZ.png
   :width: 50px
   :height: 50px

.. |RZX| image:: images/QGate_RZX.png
   :width: 50px
   :height: 50px

.. |Toffoli| image:: images/QGate_Toff.png
   :width: 50px
   :height: 50px

单比特量子逻辑门：
`````````````````````````````````````````````````
.. tabularcolumns:: |m{0.06\textwidth}<{\centering}|c|c|

.. list-table:: 
   :align: center
   :class: longtable 

   * - |I|                                                     
     - ``I``                     
     - :math:`\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}\quad`
   * - |H|                                                      
     - ``Hadamard``              
     - :math:`\begin{bmatrix} 1/\sqrt {2} & 1/\sqrt {2} \\ 1/\sqrt {2} & -1/\sqrt {2} \end{bmatrix}\quad`
   * - |T|                                                     
     - ``T``                     
     - :math:`\begin{bmatrix} 1 & 0 \\ 0 & \exp(i\pi / 4) \end{bmatrix}\quad`
   * - |S|                                                     
     - ``S``                      
     - :math:`\begin{bmatrix} 1 & 0 \\ 0 & 1i \end{bmatrix}\quad`
   * - |X|                                                     
     - ``Pauli-X``               
     - :math:`\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}\quad`
   * - |Y|                                                     
     - ``Pauli-Y``               
     - :math:`\begin{bmatrix} 0 & -1i \\ 1i & 0 \end{bmatrix}\quad`
   * - |Z|                                                     
     - ``Pauli-Z``               
     - :math:`\begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}\quad`
   * - |X1|                                                    
     - ``X1``                    
     - :math:`\begin{bmatrix} 1/\sqrt {2} & -1i/\sqrt {2} \\ -1i/\sqrt {2} & 1/\sqrt {2} \end{bmatrix}\quad`
   * - |Y1|                                                    
     - ``Y1``                    
     - :math:`\begin{bmatrix} 1/\sqrt {2} & -1/\sqrt {2} \\ 1/\sqrt {2} & 1/\sqrt {2} \end{bmatrix}\quad`
   * - |Z1|                                                    
     - ``Z1``                    
     - :math:`\begin{bmatrix} \exp(-i\pi/4) & 0 \\ 0 & \exp(i\pi/4) \end{bmatrix}\quad`
   * - |RX|                                                    
     - ``RX``                    
     - :math:`\begin{bmatrix} \cos(\theta/2) & -1i×\sin(\theta/2) \\ -1i×\sin(\theta/2) & \cos(\theta/2) \end{bmatrix}\quad`
   * - |RY|                                                    
     - ``RY``                    
     - :math:`\begin{bmatrix} \cos(\theta/2) & -\sin(\theta/2) \\ \sin(\theta/2) & \cos(\theta/2) \end{bmatrix}\quad`
   * - |RZ|                                                    
     - ``RZ``                    
     - :math:`\begin{bmatrix} \exp(-i\theta/2) & 0 \\ 0 & \exp(i\theta/2) \end{bmatrix}\quad`
   * - |U1|                                                    
     - ``U1``                    
     - :math:`\begin{bmatrix} 1 & 0 \\ 0 & \exp(i\theta) \end{bmatrix}\quad`
   * - |U2|                                                    
     - ``U2``                    
     - :math:`\begin{bmatrix} 1/\sqrt {2} & -\exp(i\lambda)/\sqrt {2} \\ \exp(i\phi)/\sqrt {2} & \exp(i\lambda+i\phi)/\sqrt {2} \end{bmatrix}\quad`
   * - |U3|                                                    
     - ``U3``                    
     - :math:`\begin{bmatrix} \cos(\theta/2) & -\exp(i\lambda)×\sin(\theta/2) \\ \exp(i\phi)×\sin(\theta/2) & \exp(i\lambda+i\phi)×\cos(\theta/2) \end{bmatrix}\quad`
   * - |U4|                                                    
     - ``U4``                    
     - :math:`\begin{bmatrix} u0 & u1 \\ u2 & u3 \end{bmatrix}\quad`


多比特量子逻辑门：
`````````````````````````````````````````````````
.. tabularcolumns:: |m{0.1\linewidth}<{\centering}|c|c|

.. list-table:: 
   :widths: auto
   :align: center
   :class: longtable 

   * - |CNOT|                                                      
     - ``CNOT``                  
     - :math:`\begin{bmatrix} 1 & 0 & 0 & 0  \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 \\ 0 & 0 & 1 & 0 \end{bmatrix}\quad`
   * - |CR|                                                        
     - ``CR``                    
     - :math:`\begin{bmatrix} 1 & 0 & 0 & 0  \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & \exp(i\theta) \end{bmatrix}\quad`
   * - |iSWAP|                                                      
     - ``iSWAP``                 
     - :math:`\begin{bmatrix} 1 & 0 & 0 & 0  \\ 0 & \cos(\theta) & i×\sin(\theta) & 0 \\ 0 & i×\sin(\theta) & \cos(\theta) & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix}\quad`
   * - |SWAP|                                                      
     - ``SWAP``                  
     - :math:`\begin{bmatrix} 1 & 0 & 0 & 0  \\ 0 & 0 & 1 & 0 \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 1 \end{bmatrix}\quad`
   * - |CZ|                                                        
     - ``CZ``                    
     - :math:`\begin{bmatrix} 1 & 0 & 0 & 0  \\ 0 & 1 & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & -1 \end{bmatrix}\quad`
   * - |CU|                                                        
     - ``CU``                    
     - :math:`\begin{bmatrix} 1 & 0 & 0 & 0  \\ 0 & 1 & 0 & 0 \\ 0 & 0 & u0 & u1 \\ 0 & 0 & u2 & u3 \end{bmatrix}\quad`
   * - |RXX|                                                        
     - ``RXX``
     - :math:`\begin{bmatrix} \cos(\theta/2) & 0 & 0 & -i\sin(\theta/2)  \\ 0 & \cos(\theta/2) & -i\sin(\theta/2) & 0 \\ 0 & -i\sin(\theta/2) & \cos(\theta/2) & 0 \\ -i\sin(\theta/2) & 0 & 0 & \cos(\theta/2) \end{bmatrix}\quad`
   * - |RYY|                                                        
     - ``RYY``
     - :math:`\begin{bmatrix} \cos(\theta/2) & 0 & 0 & i\sin(\theta/2)  \\ 0 & \cos(\theta/2) & -i\sin(\theta/2) & 0 \\ 0 & -i\sin(\theta/2) & \cos(\theta/2) & 0 \\ i\sin(\theta/2) & 0 & 0 & \cos(\theta/2) \end{bmatrix}\quad`
   * - |RZZ|                                                        
     - ``RZZ``
     - :math:`\begin{bmatrix} \exp(-i\theta/2) & 0 & 0 & 0  \\ 0 & \exp(i\theta/2) & 0 & 0 \\ 0 & 0 & \exp(i\theta/2) & 0 \\ 0 & 0 & 0 & \exp(-i\theta/2) \end{bmatrix}\quad`
   * - |RZX|                                                        
     - ``RZX``
     - :math:`\begin{bmatrix} \cos(\theta/2) & 0 & -i\sin(\theta/2) & 0  \\ 0 & \cos(\theta/2) & 0 & i\sin(\theta/2) \\ -i\sin(\theta/2) & 0 & \cos(\theta/2) & 0 \\ 0 & i\sin(\theta/2) & 0 & \cos(\theta/2) \end{bmatrix}\quad`
   * - |Toffoli|                                                    
     - ``Toffoli``               
     - :math:`\begin{bmatrix} 1 & 0 & 0 & 0 & 0 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 & 0 & 0 & 0 & 0 \\ 0 & 0 & 1 & 0 & 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 1 & 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 & 1 & 0 & 0 & 0  \\ 0 & 0 & 0 & 0 & 0 & 1 & 0 & 0 \\ 0 & 0 & 0 & 0 & 0 & 0 & 0 & 1  \\ 0 & 0 & 0 & 0 & 0 & 0 & 1 & 0 \\ \end{bmatrix}\quad`

.. _api_introduction:

QPanda-2把所有的量子逻辑门封装为API向用户提供使用，并可获得QGate类型的返回值。比如，您想要使用Hadamard门，就可以通过如下方式获得：

     .. code-block:: c
          
          QGate h = H(qubit);

可以看到，H函数只接收一个qubit，qubit如何申请会在 :ref:`QuantumMachine` 部分介绍。

再比如，您想要使用RX门，可以通过如下方式获得：

     .. code-block:: c
          
          QGate rx = RX(qubit, PI);

如上所示，RX门接收两个参数，第一个是目标量子比特，第二个偏转角度。您也可以通过相同的方式使用RY，RZ门。

两比特量子逻辑门的使用和单比特量子逻辑门的用法相似，只不过是输入的参数不同，举个使用CNOT的例子：

     .. code-block:: c
          
          QGate cnot = CNOT(control_qubit, target_qubit);

CNOT门接收两个参数，第一个是控制比特，第二个是目标比特。


接口介绍
----------------

在本章的开头介绍过，所有的量子逻辑门都是酉矩阵，那么您也可以对量子逻辑门做转置共轭操作。QGate类型有两个成员函数可以做转置共轭操作：
dagger、setDagger。

setDagger的作用是根据输入参数更新当前量子逻辑门的dagger标记，在计算时计算后端会根据dagger判断当前量子逻辑门是否需要执行转置共轭操作。举个列子：

     .. code-block:: c
          
          auto gate = H(qubit);
          gate.setDagger(true);

.. note:: setDagger有一个布尔类型参数，用来设置当前逻辑门是否需要转置共轭操作。

dagger的作用是复制一份当前的量子逻辑门，并更新复制的量子逻辑门的dagger标记。举个例子：

     .. code-block:: c
          
          QGate rx_dagger = RX(qubit,PI).dagger();

除了转置共轭操作，您也可以为量子逻辑门添加控制比特，添加控制比特后，当前量子逻辑门是否执行需要根据控制比特的量子态决定。如果控制比特的量子态为|1>态时，当前量子逻辑门可被执行，
如果控制比特的量子态为|0>时，当前量子逻辑门不会被执行。QGate类型有两个成员函数帮助您添加控制比特：control、setControl。

setControl的作用是给当前的量子逻辑门添加控制比特，例如：

     .. code-block:: c
          
          auto gate = RX(qubit,PI)
          gate.setControl(qvec);



control的作用是复制当前的量子逻辑门，并给复制的量子逻辑门添加控制比特，例如：

     .. code-block:: c
          
          QGate rx_control = RX(qubit,PI).control(qvec);


.. note:: setControl、control都需要接收一个参数，参数类型为QVec，QVec是qubit的vector。

实例
----------------

以下实例主要是向您展现QGate类型接口的使用方式，我们先使用CPUQVM()来创建一个虚拟机，再调用init接口初始化，向量子虚拟机申请3个量子比特，并把q[0],q[1]存放在一个量子比特容器中。
接着，调用QProg构建一个量子程序prog，然后我们可以通过 << 操作符把量子逻辑门插入到prog中。最后调用probRunTupleList概率测量运行接口，就可以得到计算结果了。

    .. code-block:: c
    
        #include "QPanda.h"
        using namespace QPanda;

        int main(void)
        {
            auto qvm = CPUQVM();
            qvm.init();
            auto q = qvm.qAllocMany(3);
            QVec qubits = {q[0],q[1]};
            
            // 构建量子程序
            auto prog = QProg();
            prog << H(q[0])
                 << H(q[1]) 
                 << H(q[0]).dagger()
                 << X(q[2]).control(qubits);
            
            // 概率测量，并返回目标量子比特的概率测量结果，下标为十进制
            auto result = qvm.probRunTupleList(prog, q);

            // 打印测量结果
            for(auto & aiter : result)
            {
                std::cout << aiter.first << " : " << aiter.second << std::endl;
            }

            return 0;
        }

计算结果如下：

    .. code-block:: c
        
        0 : 0.5
        2 : 0.5