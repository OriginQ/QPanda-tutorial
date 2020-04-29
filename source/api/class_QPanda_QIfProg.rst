.. index:: pair: class; QPanda::QIfProg
.. _doxid-class_q_panda_1_1_q_if_prog:

class QPanda::QIfProg
=====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Proxy class of quantum if program. :ref:`More...<details-class_q_panda_1_1_q_if_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class QIfProg: public :ref:`QPanda::AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`
	{
	public:
		// construction
	
		:ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog_1ada312e015f39b310009a30c0d471ee93>`(const QIfProg& old);
		:target:`QIfProg<doxid-class_q_panda_1_1_q_if_prog_1af750aa151e8e8cfd63b1c537fadc760b>`(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> qif);
		:ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog_1afa43a5f22a6606ca16f04958f08cdda9>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` false_node);
		:ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog_1a1a7068eeb07872b3297b2d7c1fb24a6f>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node);

		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_if_prog_1aa13300162fd43ef082beaa0101ce006d>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getTrueBranch<doxid-class_q_panda_1_1_q_if_prog_1a4b452df0d35b1bc3df770a1a46c52539>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getFalseBranch<doxid-class_q_panda_1_1_q_if_prog_1af294988fe99a5d80ae401730db6344c7>`() const;
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_q_if_prog_1a9fc18dfd79f052efb866f17818b2b1dd>`();
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getCExpr<doxid-class_q_panda_1_1_q_if_prog_1a168a97e52f650876cba557eb84da9865>`();
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getClassicalCondition<doxid-class_q_panda_1_1_q_if_prog_1a3e4489612cf90457837bf4823dfc44e3>`();
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

.. _details-class_q_panda_1_1_q_if_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Proxy class of quantum if program.

Construction
------------

.. index:: pair: function; QIfProg
.. _doxid-class_q_panda_1_1_q_if_prog_1ada312e015f39b310009a30c0d471ee93:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QIfProg(const QIfProg& old)

Construct a new :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- old

		- Target :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>`

.. index:: pair: function; QIfProg
.. _doxid-class_q_panda_1_1_q_if_prog_1afa43a5f22a6606ca16f04958f08cdda9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QIfProg(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` false_node)

Construct a new :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- classical_condition

		- this :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>` classical condition

	*
		- true_node

		- true branch node

	*
		- false_node

		- false branch node

.. index:: pair: function; QIfProg
.. _doxid-class_q_panda_1_1_q_if_prog_1a1a7068eeb07872b3297b2d7c1fb24a6f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QIfProg(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node)

Construct a new :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>` object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- classical_condition

		- this :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>` classical condition

	*
		- node

		- true branch node

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_q_if_prog_1aa13300162fd43ef082beaa0101ce006d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get the current node type.



.. rubric:: Returns:

NodeType

.. index:: pair: function; getTrueBranch
.. _doxid-class_q_panda_1_1_q_if_prog_1a4b452df0d35b1bc3df770a1a46c52539:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getTrueBranch() const

Get the True Branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; getFalseBranch
.. _doxid-class_q_panda_1_1_q_if_prog_1af294988fe99a5d80ae401730db6344c7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getFalseBranch() const

Get the False Branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; getCExpr
.. _doxid-class_q_panda_1_1_q_if_prog_1a168a97e52f650876cba557eb84da9865:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` getCExpr()

Get classical expr.



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` ptr

.. index:: pair: function; getClassicalCondition
.. _doxid-class_q_panda_1_1_q_if_prog_1a3e4489612cf90457837bf4823dfc44e3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` getClassicalCondition()

get a classical condition



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

