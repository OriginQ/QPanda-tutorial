.. index:: pair: class; QPanda::OriginQWhile
.. _doxid-class_q_panda_1_1_origin_q_while:

class QPanda::OriginQWhile
==========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QWhileProg <doxid-class_q_panda_1_1_q_while_prog>`. :ref:`More...<details-class_q_panda_1_1_origin_q_while>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class OriginQWhile:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`
	{
	public:
		// construction
	
		:target:`OriginQWhile<doxid-class_q_panda_1_1_origin_q_while_1a414c9ae37ae0ffd4069fe9e84d41f18b>`(
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` ccCon,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node
			);

		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_q_while_1ae04adcc7d926c55c89ad978ffe58149c>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getTrueBranch<doxid-class_q_panda_1_1_origin_q_while_1ac3a0eb8b9eadb9587411239d0ce2844d>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getFalseBranch<doxid-class_q_panda_1_1_origin_q_while_1ad5f4e9fa2205d20ac16fbbcf36de4fb2>`() const;
		virtual void :ref:`setTrueBranch<doxid-class_q_panda_1_1_origin_q_while_1acf16723f488d5e715091d526898a308d>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node);
		virtual void :ref:`setFalseBranch<doxid-class_q_panda_1_1_origin_q_while_1a74547eb6766cf7bac0544cd33622446d>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node);
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`getCExpr<doxid-class_q_panda_1_1_origin_q_while_1a9efb38f77ed3cf4ef5b13e87a79faa05>`();
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

.. _details-class_q_panda_1_1_origin_q_while:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QWhileProg <doxid-class_q_panda_1_1_q_while_prog>`.

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_q_while_1ae04adcc7d926c55c89ad978ffe58149c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; getTrueBranch
.. _doxid-class_q_panda_1_1_origin_q_while_1ac3a0eb8b9eadb9587411239d0ce2844d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getTrueBranch() const

Get true branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; getFalseBranch
.. _doxid-class_q_panda_1_1_origin_q_while_1ad5f4e9fa2205d20ac16fbbcf36de4fb2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> getFalseBranch() const

Get false branch.



.. rubric:: Returns:

std::shared_ptr<QNode>

.. index:: pair: function; setTrueBranch
.. _doxid-class_q_panda_1_1_origin_q_while_1acf16723f488d5e715091d526898a308d:

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
.. _doxid-class_q_panda_1_1_origin_q_while_1a74547eb6766cf7bac0544cd33622446d:

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
.. _doxid-class_q_panda_1_1_origin_q_while_1a9efb38f77ed3cf4ef5b13e87a79faa05:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` getCExpr()

Get classical expr.



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` ptr

