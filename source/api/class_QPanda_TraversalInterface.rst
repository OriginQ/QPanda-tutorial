.. index:: pair: class; QPanda::TraversalInterface
.. _doxid-class_q_panda_1_1_traversal_interface:

template class QPanda::TraversalInterface
=========================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

All objects that want to use the class :ref:`Traversal <doxid-class_q_panda_1_1_traversal>` need to integrate this class. :ref:`More...<details-class_q_panda_1_1_traversal_interface>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Traversal.h>
	
	template <typename... Args>
	class TraversalInterface
	{
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
	};

	// direct descendants

	class :ref:`CancelControlQubitVector<doxid-class_q_panda_1_1_cancel_control_qubit_vector>`;
	class :ref:`DecomposeControlSingleQGateIntoMetadataDoubleQGate<doxid-class_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate>`;
	class :ref:`DecomposeControlUnitarySingleQGate<doxid-class_q_panda_1_1_decompose_control_unitary_single_q_gate>`;
	class :ref:`DecomposeDoubleQGate<doxid-class_q_panda_1_1_decompose_double_q_gate>`;
	class :ref:`DecomposeMultipleControlQGate<doxid-class_q_panda_1_1_decompose_multiple_control_q_gate>`;
	class :ref:`DecomposeUnitarySingleQGateIntoMetadataSingleQGate<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate>`;
	class :ref:`DeleteUnitQNode<doxid-class_q_panda_1_1_delete_unit_q_node>`;
	class :ref:`MergeSingleGate<doxid-class_q_panda_1_1_merge_single_gate>`;
	class :ref:`PartialAmplitudeQVM<doxid-class_q_panda_1_1_partial_amplitude_q_v_m>`;
	class :ref:`QGateCompare<doxid-class_q_panda_1_1_q_gate_compare>`;
	class :ref:`QGateCounter<doxid-class_q_panda_1_1_q_gate_counter>`;
	class :ref:`QNodeDeepCopy<doxid-class_q_panda_1_1_q_node_deep_copy>`;
	class :ref:`QProgFlattening<doxid-class_q_panda_1_1_q_prog_flattening>`;
	class :ref:`QProgStored<doxid-class_q_panda_1_1_q_prog_stored>`;
	class :ref:`QProgToOriginIR<doxid-class_q_panda_1_1_q_prog_to_origin_i_r>`;
	class :ref:`QProgToQASM<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m>`;
	class :ref:`QProgToQCircuit<doxid-class_q_panda_1_1_q_prog_to_q_circuit>`;
	class :ref:`QProgToQGate<doxid-class_q_panda_1_1_q_prog_to_q_gate>`;
	class :ref:`QProgToQMeasure<doxid-class_q_panda_1_1_q_prog_to_q_measure>`;
	class :ref:`QProgToQuil<doxid-class_q_panda_1_1_q_prog_to_quil>`;
	class :ref:`SingleAmplitudeQVM<doxid-class_q_panda_1_1_single_amplitude_q_v_m>`;
	class :ref:`TopologyMatch<doxid-class_q_panda_1_1_topology_match>`;
	class :ref:`TraverseByNodeIter<doxid-class_q_panda_1_1_traverse_by_node_iter>`;
.. _details-class_q_panda_1_1_traversal_interface:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

All objects that want to use the class :ref:`Traversal <doxid-class_q_panda_1_1_traversal>` need to integrate this class.

Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_traversal_interface_1a1cb0c50abcd626b8c45b8aa389cb3541:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		Args&&... func_args
		) = 0

Execution traversal qgatenode.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQGateNode\*

		- quantum gate

	*
		- QNode\*

		- parent Node



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_traversal_interface_1a6916170c055781c5ed5a615407390e1c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		Args&&... func_args
		) = 0

Execution traversal measure node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumMeasure\*

		- measure node

	*
		- QNode\*

		- parent Node



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_traversal_interface_1aa3389601eef27921246507d9bcd60e8f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		Args&&... func_args
		) = 0

Execution traversal reset node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumReset\*

		- reset node

	*
		- QNode\*

		- parent Node



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_traversal_interface_1a2196c7ad5525e519cfedad3d0285d712:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		Args&&... func_args
		) = 0

Execution traversal control flow node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractControlFlowNode\*

		- control flow node

	*
		- QNode\*

		- parent Node



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_traversal_interface_1a34a63b4019719d77711fcf6efbb6400c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		Args&&... func_args
		) = 0

Execution traversal qcircuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumCircuit\*

		- quantum circuit

	*
		- QNode\*

		- parent Node



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_traversal_interface_1a310247426bda77a52b81c7654fa4b848:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		Args&&... func_args
		) = 0

Execution traversal qprog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumProgram\*

		- quantum prog

	*
		- QNode\*

		- parent Node



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_traversal_interface_1a7d2fb53e43f56cc2f57cf0d025585146:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		Args&&... func_args
		) = 0

Execution traversal qprog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractClassicalProg\*

		- classical prog

	*
		- QNode\*

		- parent Node



.. rubric:: Returns:

void

