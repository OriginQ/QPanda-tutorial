.. index:: pair: class; QPanda::DeleteUnitQNode
.. _doxid-class_q_panda_1_1_delete_unit_q_node:

class QPanda::DeleteUnitQNode
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TransformDecomposition.h>
	
	class DeleteUnitQNode: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		void :ref:`execute<doxid-class_q_panda_1_1_delete_unit_q_node_1ad0ddf5e461cd7f9d9eac6574bbecb6a7>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_delete_unit_q_node_1a343d4cfda1be9c9f36785fdb64c591d2>`(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_delete_unit_q_node_1aafd619238e7fa19f54170f3d3c5f39f4>`(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_delete_unit_q_node_1aade3299ff15f93683c29fd0bf9701bad>`(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_delete_unit_q_node_1aff5c2cf70e7c9598e8e617b5dba8c044>`(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_delete_unit_q_node_1a3de9010ff5f7b76bb8a8f4c1a63853af>`(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_delete_unit_q_node_1a62d9dad127e5ddab09d8c841f105c4f6>`(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
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

.. _details-class_q_panda_1_1_delete_unit_q_node:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_delete_unit_q_node_1ad0ddf5e461cd7f9d9eac6574bbecb6a7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void execute(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qgatenode.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQGateNode\*

		- quantum gate

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_delete_unit_q_node_1a343d4cfda1be9c9f36785fdb64c591d2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal measure node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumMeasure\*

		- measure node

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_delete_unit_q_node_1aafd619238e7fa19f54170f3d3c5f39f4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal reset node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumReset\*

		- reset node

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_delete_unit_q_node_1aade3299ff15f93683c29fd0bf9701bad:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal control flow node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractControlFlowNode\*

		- control flow node

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_delete_unit_q_node_1aff5c2cf70e7c9598e8e617b5dba8c044:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qcircuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumCircuit\*

		- quantum circuit

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_delete_unit_q_node_1a3de9010ff5f7b76bb8a8f4c1a63853af:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qprog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumProgram\*

		- quantum prog

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_delete_unit_q_node_1a62d9dad127e5ddab09d8c841f105c4f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qprog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractClassicalProg\*

		- quantum prog

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

