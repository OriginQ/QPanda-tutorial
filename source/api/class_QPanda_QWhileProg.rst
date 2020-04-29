.. index:: pair: class; QPanda::QWhileProg
.. _doxid-class_q_panda_1_1_q_while_prog:

class QPanda::QWhileProg
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Proxy class of quantum while program. :ref:`More...<details-class_q_panda_1_1_q_while_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class QWhileProg: public :ref:`QPanda::AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`
	{
	public:
		// construction
	
		:target:`QWhileProg<doxid-class_q_panda_1_1_q_while_prog_1a5172cbcc883a48e912b6864ff3256934>`(const QWhileProg&);
		:target:`QWhileProg<doxid-class_q_panda_1_1_q_while_prog_1a4d2e576909b32801741c022fd62ee4c8>`(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> qwhile);
	
		:target:`QWhileProg<doxid-class_q_panda_1_1_q_while_prog_1a0c73a79659981e1f3852acc981193003>`(
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`
			);

		// methods
	
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_q_while_prog_1a81e44fc83e4271985fdd82cec8ccd712>`();
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :target:`getNodeType<doxid-class_q_panda_1_1_q_while_prog_1a9310981a55b161784ae91bdd25244426>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getTrueBranch<doxid-class_q_panda_1_1_q_while_prog_1a042e7133285464f8fa6c1e707a0b6d1c>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getFalseBranch<doxid-class_q_panda_1_1_q_while_prog_1a1b77b6d34a1ec94426fdbfc8ed289ce6>`() const;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getCExpr<doxid-class_q_panda_1_1_q_while_prog_1a9174f0fdac303628a93c8bbc5c45b8b0>`();
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :target:`getClassicalCondition<doxid-class_q_panda_1_1_q_while_prog_1a67aec1f5d12cd103f09fd244ba92bff7>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getTrueBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1aea87b38dcb985d675b746500b505a1af>`() const = 0;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getFalseBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a59528733e2a86f89827d352a7c312b8c>`() const = 0;
		virtual void :ref:`setTrueBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a2039dfd9785c87c206112df71a56849c>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0;
		virtual void :ref:`setFalseBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a094ab286d9cc78313f4b3d459618de44>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getCExpr<doxid-class_q_panda_1_1_abstract_control_flow_node_1a67ca259afc5af2652184e4cc0e12e985>`() = 0;

.. _details-class_q_panda_1_1_q_while_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Proxy class of quantum while program.

Methods
-------

.. index:: pair: function; getTrueBranch
.. _doxid-class_q_panda_1_1_q_while_prog_1a042e7133285464f8fa6c1e707a0b6d1c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getTrueBranch() const

Get true branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; getFalseBranch
.. _doxid-class_q_panda_1_1_q_while_prog_1a1b77b6d34a1ec94426fdbfc8ed289ce6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getFalseBranch() const

Get false branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; getCExpr
.. _doxid-class_q_panda_1_1_q_while_prog_1a9174f0fdac303628a93c8bbc5c45b8b0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` getCExpr()

Get classical expr.



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` ptr

