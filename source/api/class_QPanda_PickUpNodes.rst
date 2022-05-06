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
	
		:ref:`PickUpNodes<doxid-class_q_panda_1_1_pick_up_nodes_1ab19d5ec65100e71af105d96146fd1157>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& output_prog,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` src_prog,
			const std::vector<:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`>& reject_node_types,
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& node_itr_start,
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& node_itr_end
			);

		// methods
	
		virtual void :target:`traverse_qprog<doxid-class_q_panda_1_1_pick_up_nodes_1a5c15d719416011042f10e3aa0fc287a5>`();
	
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
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab298ca4e8835cb14518f8b83c87d6287>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);

.. _details-class_q_panda_1_1_pick_up_nodes:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Pick Up all the Nodes between the two NodeIters.

Construction
------------

.. index:: pair: function; PickUpNodes
.. _doxid-class_q_panda_1_1_pick_up_nodes_1ab19d5ec65100e71af105d96146fd1157:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PickUpNodes(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& output_prog,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` src_prog,
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

