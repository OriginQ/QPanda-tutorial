.. index:: pair: class; QPanda::QNodeDeepCopy
.. _doxid-class_q_panda_1_1_q_node_deep_copy:

class QPanda::QNodeDeepCopy
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Deep copy interface for classess based on :ref:`QNode <doxid-class_q_panda_1_1_q_node>`. :ref:`More...<details-class_q_panda_1_1_q_node_deep_copy>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QNodeDeepCopy.h>
	
	class QNodeDeepCopy: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`executeQNode<doxid-class_q_panda_1_1_q_node_deep_copy_1aee69de6e692e742b7107592a3f156b83>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node);
		:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`copy_node<doxid-class_q_panda_1_1_q_node_deep_copy_1a134f4799ed71fb30f28df3d2b44ac5da>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`>);
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`copy_node<doxid-class_q_panda_1_1_q_node_deep_copy_1a1c50d05fbecefe3b501ae746667c0cd8>`(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`>);
		:ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` :ref:`copy_node<doxid-class_q_panda_1_1_q_node_deep_copy_1a68533c85304335408722fc2863b10c1c>`(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`>);
		:ref:`QReset<doxid-class_q_panda_1_1_q_reset>` :ref:`copy_node<doxid-class_q_panda_1_1_q_node_deep_copy_1a79a02a7004fd250b171ef3f66ba5ee2e>`(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`>);
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`copy_node<doxid-class_q_panda_1_1_q_node_deep_copy_1ae6295c34c5d352b07b5cdb46d5e30d85>`(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`>);
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> :ref:`copy_node<doxid-class_q_panda_1_1_q_node_deep_copy_1a080c042b1752d9ced31fc2837ae8232b>`(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`>);
		:ref:`ClassicalProg<doxid-class_q_panda_1_1_classical_prog>` :ref:`copy_node<doxid-class_q_panda_1_1_q_node_deep_copy_1a118bdb859514b48aa813a6908ee6e831>`(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`>);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_node_deep_copy_1a96645872eed144337fe7b9d95f9813a8>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_node_deep_copy_1a20e1cd18185b40c1a7d236360b5108d7>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_node_deep_copy_1af1eb120c7c8cbccd875bf02bd41ea6c8>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_node_deep_copy_1a702f05f3213b7af3e6bb522b743fdf66>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_node_deep_copy_1a803e31255fbbba4760e28cd00a8373df>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_node_deep_copy_1a36a25593f92f4b98f7613dfcb26a49d9>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_node_deep_copy_1acd259efee9d2419adf7473370692787b>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a1cb0c50abcd626b8c45b8aa389cb3541>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a6916170c055781c5ed5a615407390e1c>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aa3389601eef27921246507d9bcd60e8f>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a2196c7ad5525e519cfedad3d0285d712>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a34a63b4019719d77711fcf6efbb6400c>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a310247426bda77a52b81c7654fa4b848>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a7d2fb53e43f56cc2f57cf0d025585146>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;

.. _details-class_q_panda_1_1_q_node_deep_copy:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Deep copy interface for classess based on :ref:`QNode <doxid-class_q_panda_1_1_q_node>`.

Methods
-------

.. index:: pair: function; executeQNode
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1aee69de6e692e742b7107592a3f156b83:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> executeQNode(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node)

Execute :ref:`QNode <doxid-class_q_panda_1_1_q_node>` Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QNode\*

		- 



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new Node

.. index:: pair: function; copy_node
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1a134f4799ed71fb30f28df3d2b44ac5da:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` copy_node(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`>)

Execute Quantum Gate Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQGateNode\*

		- Quantum Gate Node



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new :ref:`QNode <doxid-class_q_panda_1_1_q_node>`

.. index:: pair: function; copy_node
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1a1c50d05fbecefe3b501ae746667c0cd8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` copy_node(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`>)

Execute Quantum :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumProgram\*

		- Quantum :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` Node



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new Node

.. index:: pair: function; copy_node
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1a68533c85304335408722fc2863b10c1c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` copy_node(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`>)

Execute Quantum Measure Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumMeasure\*

		- Quantum Measure Node



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new Node

.. index:: pair: function; copy_node
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1a79a02a7004fd250b171ef3f66ba5ee2e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QReset<doxid-class_q_panda_1_1_q_reset>` copy_node(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`>)

Execute Quantum Reset Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumReset\*

		- Quantum Reset Node



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new Node

.. index:: pair: function; copy_node
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1ae6295c34c5d352b07b5cdb46d5e30d85:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` copy_node(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`>)

Execute Quantum Circuit Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumCircuit\*

		- Quantum Circuit Node



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new Node

.. index:: pair: function; copy_node
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1a080c042b1752d9ced31fc2837ae8232b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> copy_node(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`>)

Execute ControlFlow Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractControlFlowNode\*

		- ControlFlow Node



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new Node

.. index:: pair: function; copy_node
.. _doxid-class_q_panda_1_1_q_node_deep_copy_1a118bdb859514b48aa813a6908ee6e831:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalProg<doxid-class_q_panda_1_1_classical_prog>` copy_node(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`>)

Execute :ref:`ClassicalProg <doxid-class_q_panda_1_1_classical_prog>` Node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractClassicalProg\*

		- :ref:`ClassicalProg <doxid-class_q_panda_1_1_classical_prog>` Node



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> new Node

