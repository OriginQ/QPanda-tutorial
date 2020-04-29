.. QPanda 2 documentation master file, created by
   sphinx-quickstart on Tue Jan 22 14:31:31 2019.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

QPanda 2
====================================
|build-status|

.. |build-status| image:: https://travis-ci.org/OriginQ/QPanda-2.svg?branch=master
    :alt: build status
    :scale: 100%
    :target: https://travis-ci.org/OriginQ/QPanda-2

**一种功能齐全，运行高效的量子软件开发工具包**

QPanda 2是由本源量子开发的开源量子计算框架，它可以用于构建、运行和优化量子算法。QPanda 2作为本源量子计算系列软件的基础库，为OriginIR、Qurator、量子计算服务提供核心部件。

为了方便用户使用，QPanda 2为用户提供了Python版本的pyQPanda,详情请参考 `pyQPanda使用文档 <https://pyqpanda-toturial.readthedocs.io/zh/latest/index.html>`_ 。

.. toctree::
    :maxdepth: 1
   
.. toctree::
    :caption: 基础介绍
    :maxdepth: 2

    Tutorial

.. toctree::
    :caption: 深入学习
    :maxdepth: 2

    QGate
    QCircuit
    BuildingModularQCircuit
    QWhile
    QIf
    QProg
    QuantumMachine
    Measure
    PMeasure
    
.. toctree::
    :caption: 量子程序信息
    :maxdepth: 2

    QGateValidity 
    QProgClockCycle  
    QGateCounter
    QCircuitInfo
    DrawQProg

.. toctree::
    :caption: 编译量子程序
    :maxdepth: 2
    
    QProgToQASM
    QASMToQProg
    QProgToQuil
    QProgStored
    QProgDataParse
    OriginIRToQProg
    QProgToOriginIR
    OriginIRToQProg
    QCodarMatch
    
.. toctree::
    :caption: 实用工具
    :maxdepth: 2
    
    GraphMatch
    FillQProgByI

.. toctree::
    :caption: 组件
    :maxdepth: 2

    PauliOperator
    FermionOperator
    Optimizer

.. toctree::
    :caption: VQNet
    :maxdepth: 2
    
    Var
    VarOperator
    VQG
    VQC
    GradientOptimizer
    VQNetExample

.. toctree::
    :caption: API Reference
    :maxdepth: 2

	api/index
