.. index:: pair: class; QPanda::TraverseByNodeIter
.. _doxid-class_q_panda_1_1_traverse_by_node_iter:

class QPanda::TraverseByNodeIter
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Traverse :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` By :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`. :ref:`More...<details-class_q_panda_1_1_traverse_by_node_iter>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitInfo.h>
	
	class TraverseByNodeIter: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab322f1c7e3734cf25d22c57c1dfe6e98>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a73c8f60de984e2aa5705211b361d98e1>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1aeea9c768792ed69bccd8cd9418fa9180>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1af01742419980d7fc620f085fffcc319b>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a95859495e9b97db265dc1a0932836366>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1adadb977d5747ba2f307f6f8d7bf49742>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab5039119411bc0f91236fac876fc606f>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab298ca4e8835cb14518f8b83c87d6287>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);
	};

	// direct descendants

	class :ref:`AdjacentQGates<doxid-class_q_panda_1_1_adjacent_q_gates>`;
	class :ref:`GetAllNodeType<doxid-class_q_panda_1_1_get_all_node_type>`;
	class :ref:`GetAllUsedQubitAndCBit<doxid-class_q_panda_1_1_get_all_used_qubit_and_c_bit>`;
	class :ref:`JudgeTwoNodeIterIsSwappable<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable>`;
	class :ref:`PickUpNodes<doxid-class_q_panda_1_1_pick_up_nodes>`;
	class :ref:`ProcessOnTraversing<doxid-class_q_panda_1_1_process_on_traversing>`;
	class :ref:`QProgToDAG<doxid-class_q_panda_1_1_q_prog_to_d_a_g>`;
	class :ref:`QProgToQASM<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m>`;
	class :ref:`RemapQProg<doxid-class_q_panda_1_1_remap_q_prog>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1adb53e4c20d48a0efd6e377680d7f0988>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aed584073b781c9a5c6441b08b14afc3d>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aadbf69a810033196de1790d3f362ef7a>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aab65fda71b8e1f719bc4b7bdd70a10e7>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1ab452f71d25eb3354d46346694ff82db7>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a4e97902dc8b42d5f5f50d790d11f1517>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aa311fe1c6abc46d84d90d6f412be063a>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);

.. _details-class_q_panda_1_1_traverse_by_node_iter:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Traverse :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` By :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.

Methods
-------

.. index:: pair: function; traverse_qprog
.. _doxid-class_q_panda_1_1_traverse_by_node_iter_1ab298ca4e8835cb14518f8b83c87d6287:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void traverse_qprog(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog)

start traverse a quantum prog

