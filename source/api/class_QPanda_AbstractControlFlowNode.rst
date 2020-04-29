.. index:: pair: class; QPanda::AbstractControlFlowNode
.. _doxid-class_q_panda_1_1_abstract_control_flow_node:

class QPanda::AbstractControlFlowNode
=====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Superclass for QIfProg/QWhileProg. :ref:`More...<details-class_q_panda_1_1_abstract_control_flow_node>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class AbstractControlFlowNode
	{
	public:
		// methods
	
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getTrueBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1aea87b38dcb985d675b746500b505a1af>`() const = 0;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getFalseBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a59528733e2a86f89827d352a7c312b8c>`() const = 0;
		virtual void :ref:`setTrueBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a2039dfd9785c87c206112df71a56849c>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0;
		virtual void :ref:`setFalseBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a094ab286d9cc78313f4b3d459618de44>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getCExpr<doxid-class_q_panda_1_1_abstract_control_flow_node_1a67ca259afc5af2652184e4cc0e12e985>`() = 0;
	};

	// direct descendants

	class :ref:`OriginQIf<doxid-class_q_panda_1_1_origin_q_if>`;
	class :ref:`OriginQWhile<doxid-class_q_panda_1_1_origin_q_while>`;
	class :ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog>`;
	class :ref:`QWhileProg<doxid-class_q_panda_1_1_q_while_prog>`;
.. _details-class_q_panda_1_1_abstract_control_flow_node:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Superclass for QIfProg/QWhileProg.

Methods
-------

.. index:: pair: function; getTrueBranch
.. _doxid-class_q_panda_1_1_abstract_control_flow_node_1aea87b38dcb985d675b746500b505a1af:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getTrueBranch() const = 0

Get true branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; getFalseBranch
.. _doxid-class_q_panda_1_1_abstract_control_flow_node_1a59528733e2a86f89827d352a7c312b8c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getFalseBranch() const = 0

Get false branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; setTrueBranch
.. _doxid-class_q_panda_1_1_abstract_control_flow_node_1a2039dfd9785c87c206112df71a56849c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setTrueBranch(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0

Set the True branch.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Node

		- True branch node

.. index:: pair: function; setFalseBranch
.. _doxid-class_q_panda_1_1_abstract_control_flow_node_1a094ab286d9cc78313f4b3d459618de44:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setFalseBranch(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0

Set the False Branch object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Node

		- False branch node

.. index:: pair: function; getCExpr
.. _doxid-class_q_panda_1_1_abstract_control_flow_node_1a67ca259afc5af2652184e4cc0e12e985:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` getCExpr() = 0

Get classical expr.



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` ptr

