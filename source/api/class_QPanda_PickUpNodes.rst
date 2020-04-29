.. index:: pair: class; QPanda::PickUpNodes
.. _doxid-class_q_panda_1_1_pick_up_nodes:

class QPanda::PickUpNodes
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Pick Up all the Nodes between the two NodeIters. :ref:`More...<details-class_q_panda_1_1_pick_up_nodes>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitInfo.h>
	
	class PickUpNodes: public :ref:`QPanda::TraverseByNodeIter<doxid-class_q_panda_1_1_traverse_by_node_iter>`
	{
	public:
		// construction
	
		:ref:`PickUpNodes<doxid-class_q_panda_1_1_pick_up_nodes_1ae8a58dc4c8e02b587f95c26bd77d3bbb>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& output_prog,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& src_prog,
			const std::vector<:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`>& reject_node_types,
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& node_itr_start,
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& node_itr_end
			);

		// methods
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_pick_up_nodes_1a41605f6d189b6cd266a5da20a7c98ead>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_pick_up_nodes_1ac9fbc2ea4f1cc4e4710d09a4b83ca554>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_pick_up_nodes_1a59e1d522efbafb8d5d7f980536007220>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_pick_up_nodes_1a796f8b54ceab2f85ab85350e14af5566>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_pick_up_nodes_1a76378308ee48cd585d9de2092a72da83>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_pick_up_nodes_1a59a1016399fecfe44cf6680afea479ff>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_pick_up_nodes_1a80d149f10e0d26e61ffe21b9b360c7f6>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :ref:`setDaggerFlag<doxid-class_q_panda_1_1_pick_up_nodes_1a67b85e8bd9365234b24902ac403be857>`(bool b);
		void :ref:`reverse_dagger_circuit<doxid-class_q_panda_1_1_pick_up_nodes_1a341abe0dead8124e77ea4812a5ab9b91>`();
		static bool :ref:`check_control_qubits<doxid-class_q_panda_1_1_pick_up_nodes_1a498c266d7f64300252dc97b020932546>`(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate);
		static void :ref:`no_dagger_gate<doxid-class_q_panda_1_1_pick_up_nodes_1a9ac6fbd7bf24d2265911dfad17afb9c5>`(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate);
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
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab322f1c7e3734cf25d22c57c1dfe6e98>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a73c8f60de984e2aa5705211b361d98e1>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1aeea9c768792ed69bccd8cd9418fa9180>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1af01742419980d7fc620f085fffcc319b>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a95859495e9b97db265dc1a0932836366>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1adadb977d5747ba2f307f6f8d7bf49742>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab5039119411bc0f91236fac876fc606f>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_traverse_by_node_iter_1a407bc9a3cc75874142fbfec69447e9e2>`();

.. _details-class_q_panda_1_1_pick_up_nodes:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Pick Up all the Nodes between the two NodeIters.

Construction
------------

.. index:: pair: function; PickUpNodes
.. _doxid-class_q_panda_1_1_pick_up_nodes_1ae8a58dc4c8e02b587f95c26bd77d3bbb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PickUpNodes(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& output_prog,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& src_prog,
		const std::vector<:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`>& reject_node_types,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& node_itr_start,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& node_itr_end
		)

Constructor of :ref:`PickUpNodes <doxid-class_q_panda_1_1_pick_up_nodes>`.

Methods
-------

.. index:: pair: function; setDaggerFlag
.. _doxid-class_q_panda_1_1_pick_up_nodes_1a67b85e8bd9365234b24902ac403be857:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDaggerFlag(bool b)

set dagger flag



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; reverse_dagger_circuit
.. _doxid-class_q_panda_1_1_pick_up_nodes_1a341abe0dead8124e77ea4812a5ab9b91:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void reverse_dagger_circuit()

reverse the dagger circuit

.. index:: pair: function; check_control_qubits
.. _doxid-class_q_panda_1_1_pick_up_nodes_1a498c266d7f64300252dc97b020932546:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool check_control_qubits(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate)

check whether the control qubit is same as the target qubit



.. rubric:: Returns:

bool return true if the control qubit is same as the target qubit, otherwise return false

.. index:: pair: function; no_dagger_gate
.. _doxid-class_q_panda_1_1_pick_up_nodes_1a9ac6fbd7bf24d2265911dfad17afb9c5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static void no_dagger_gate(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate)

check no dagger gate

