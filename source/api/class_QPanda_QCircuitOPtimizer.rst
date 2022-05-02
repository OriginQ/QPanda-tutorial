.. index:: pair: class; QPanda::QCircuitOPtimizer
.. _doxid-class_q_panda_1_1_q_circuit_o_ptimizer:

class QPanda::QCircuitOPtimizer
===============================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitOptimize.h>
	
	class QCircuitOPtimizer: public :ref:`QPanda::ProcessOnTraversing<doxid-class_q_panda_1_1_process_on_traversing>`
	{
	public:
		// fields
	
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`m_new_prog<doxid-class_q_panda_1_1_q_circuit_o_ptimizer_1a56db09f810e40db5de030b5f64654abd>`;

		// methods
	
		virtual void :target:`process<doxid-class_q_panda_1_1_q_circuit_o_ptimizer_1a428df37ff287319d577ab89543d4b833>`(const bool on_travel_end = false);
		void :target:`register_single_gate_optimizer<doxid-class_q_panda_1_1_q_circuit_o_ptimizer_1ae838c59980acdefe2215ceff28ad7dc9>`(const int mode);
	
		void :target:`register_optimize_sub_cir<doxid-class_q_panda_1_1_q_circuit_o_ptimizer_1aee1285f3cf9a520664c7e0aae6e1f6fb>`(
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` sub_cir,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` replase_to_cir
			);
	
		void :target:`run_optimize<doxid-class_q_panda_1_1_q_circuit_o_ptimizer_1af7c3214205bae7bb1a111cb7653ad15d>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` src_prog,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubits = {},
			bool b_enable_I = false
			);
	
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`replase_sub_cir<doxid-group___utilities_1ga7f0e3265cb94e76cbf4df636fead147a>`(std::function<:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`(const size_t)> get_cir_fun);
		void :target:`sub_cir_optimizer<doxid-class_q_panda_1_1_q_circuit_o_ptimizer_1aa181238eeb03a681b74dbe703adf4f19>`(const size_t optimizer_sub_cir_index);
		void :target:`do_optimizer<doxid-class_q_panda_1_1_q_circuit_o_ptimizer_1ad5d6652920c271dd47543a04220917cd>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`TopologSequence<doxid-class_q_panda_1_1_topolog_sequence>`<std::pair<size_t, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`>> :ref:`layer_iter_seq<doxid-class_q_panda_1_1_process_on_traversing_1ad6a349927045cbc436346695e18f1d56>`;

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
		virtual void :ref:`process<doxid-class_q_panda_1_1_process_on_traversing_1aadef9f4e91d8892f6463c170aa56ceec>`(const bool on_travel_end) = 0;
		virtual void :ref:`run_traversal<doxid-class_q_panda_1_1_process_on_traversing_1a04ce1680a7d63f570dbf16cc581ba3e0>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` src_prog, const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubits = {});
		virtual void :ref:`do_process<doxid-class_q_panda_1_1_process_on_traversing_1a985f65295ca64f9bb524444201db865b>`(const bool on_travel_end);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_process_on_traversing_1a93f7770cca93677cbe800c3a3cd6fd69>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_process_on_traversing_1a9c002c6a38e03274e85c43f4185a939d>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_process_on_traversing_1af842a89da8f0e00bc2e88c549e328498>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_process_on_traversing_1ab4d8c88c6c38420a42d19da4ee5fea9f>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_process_on_traversing_1a1b3e3c1dd612d3c7112bb5409800d50a>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_process_on_traversing_1a329176a4f3a1280167db9aa4d7b0707e>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_process_on_traversing_1a4d966a1a4ed67463b6b9603ab4750e86>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`gates_sink_to_topolog_sequence<doxid-class_q_panda_1_1_process_on_traversing_1aa00e5cc6ffef6e71486b0b3b87aba8f4>`(:ref:`OptimizerSink<doxid-namespace_q_panda_1a751da7aaa7cac46c55057a59f2285e73>`& gate_buf, :ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& seq, const size_t max_output_layer = :ref:`MAX_LAYER<doxid-_process_on_traversing_8h_1a912d8a5fc768baa70d250f6d8f0cf751>`);
		virtual void :ref:`clean_gate_buf_to_cir<doxid-group___utilities_1ga99094e26f15c8f0ab168a8e3de78c058>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& cir, bool b_clean_all_buf = false);
		virtual void :ref:`clean_gate_buf<doxid-class_q_panda_1_1_process_on_traversing_1a0dd88f0a33744e81ef40230d9fbf7095>`(bool b_clean_all_buf = false);
		virtual void :ref:`drop_gates<doxid-class_q_panda_1_1_process_on_traversing_1afbb09826e90c3121bdcb2620302ac7b2>`(const size_t max_drop_layer);
	
		virtual void :ref:`seq_to_cir<doxid-class_q_panda_1_1_process_on_traversing_1a5a8e2d5c3f0028d1155708016a7305b9>`(
			:ref:`layer_iter_seq<doxid-class_q_panda_1_1_process_on_traversing_1ad6a349927045cbc436346695e18f1d56>`& tmp_seq,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			const size_t start_layer_to_cir,
			const size_t max_output_layer
			);
	
		virtual void :ref:`seq_to_cir<doxid-class_q_panda_1_1_process_on_traversing_1aa09f04a2056b374789d470e26564c592>`(:ref:`layer_iter_seq<doxid-class_q_panda_1_1_process_on_traversing_1ad6a349927045cbc436346695e18f1d56>`& tmp_seq, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
		virtual void :ref:`add_node_to_seq<doxid-class_q_panda_1_1_process_on_traversing_1ad668c1561c3e448a244c6241e5094470>`(:ref:`layer_iter_seq<doxid-class_q_panda_1_1_process_on_traversing_1ad6a349927045cbc436346695e18f1d56>`& tmp_seq, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_iter, const size_t layer);

.. _details-class_q_panda_1_1_q_circuit_o_ptimizer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; replase_sub_cir
.. _doxid-group___utilities_1ga7f0e3265cb94e76cbf4df636fead147a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` replase_sub_cir(std::function<:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`(const size_t)> get_cir_fun)

replace sub circuit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::function<QCircuit(const

		- size_t)> the function to get a new quantum circuit



.. rubric:: Returns:

the new quantum prog

