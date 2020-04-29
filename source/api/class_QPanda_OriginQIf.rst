.. index:: pair: class; QPanda::OriginQIf
.. _doxid-class_q_panda_1_1_origin_q_if:

class QPanda::OriginQIf
=======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>` :ref:`More...<details-class_q_panda_1_1_origin_q_if>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class OriginQIf:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`
	{
	public:
		// construction
	
		:target:`OriginQIf<doxid-class_q_panda_1_1_origin_q_if_1acc3e03a90303f510d083d523aeef7eec>`(
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` false_node
			);
	
		:target:`OriginQIf<doxid-class_q_panda_1_1_origin_q_if_1a7ebff805d431b49c97e42a950dcd4db4>`(
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node
			);

		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_q_if_1a0def277a60bff14551d62168bdb07cb3>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getTrueBranch<doxid-class_q_panda_1_1_origin_q_if_1a64a8ab6d43191b0c696930223ced2d10>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getFalseBranch<doxid-class_q_panda_1_1_origin_q_if_1a3fbf457e5a515fe1ca3b64d5f053cfc5>`() const;
		virtual void :ref:`setTrueBranch<doxid-class_q_panda_1_1_origin_q_if_1ab7dfc8455963c10a02880adffe86c594>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node);
		virtual void :ref:`setFalseBranch<doxid-class_q_panda_1_1_origin_q_if_1ae97db69862990127d18f018f6bd58052>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node);
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getCExpr<doxid-class_q_panda_1_1_origin_q_if_1a678f9b7b012367acc8e8d6e61c2ac14a>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getTrueBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1aea87b38dcb985d675b746500b505a1af>`() const = 0;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getFalseBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a59528733e2a86f89827d352a7c312b8c>`() const = 0;
		virtual void :ref:`setTrueBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a2039dfd9785c87c206112df71a56849c>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0;
		virtual void :ref:`setFalseBranch<doxid-class_q_panda_1_1_abstract_control_flow_node_1a094ab286d9cc78313f4b3d459618de44>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node) = 0;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getCExpr<doxid-class_q_panda_1_1_abstract_control_flow_node_1a67ca259afc5af2652184e4cc0e12e985>`() = 0;

.. _details-class_q_panda_1_1_origin_q_if:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QIfProg <doxid-class_q_panda_1_1_q_if_prog>`

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_q_if_1a0def277a60bff14551d62168bdb07cb3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; getTrueBranch
.. _doxid-class_q_panda_1_1_origin_q_if_1a64a8ab6d43191b0c696930223ced2d10:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getTrueBranch() const

Get true branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; getFalseBranch
.. _doxid-class_q_panda_1_1_origin_q_if_1a3fbf457e5a515fe1ca3b64d5f053cfc5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getFalseBranch() const

Get false branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; setTrueBranch
.. _doxid-class_q_panda_1_1_origin_q_if_1ab7dfc8455963c10a02880adffe86c594:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setTrueBranch(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node)

Set the True branch.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Node

		- True branch node

.. index:: pair: function; setFalseBranch
.. _doxid-class_q_panda_1_1_origin_q_if_1ae97db69862990127d18f018f6bd58052:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setFalseBranch(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node)

Set the False Branch object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Node

		- False branch node

.. index:: pair: function; getCExpr
.. _doxid-class_q_panda_1_1_origin_q_if_1a678f9b7b012367acc8e8d6e61c2ac14a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` getCExpr()

Get classical expr.



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` ptr

