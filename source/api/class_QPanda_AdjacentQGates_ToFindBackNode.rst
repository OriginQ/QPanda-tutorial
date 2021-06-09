.. index:: pair: class; QPanda::AdjacentQGates::ToFindBackNode
.. _doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node:

class QPanda::AdjacentQGates::ToFindBackNode
============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class ToFindBackNode: public QPanda::AdjacentQGates::AbstractTraversalStatueInterface
	{
	public:
		// construction
	
		:target:`ToFindBackNode<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1af9dff3b07ad3a59db9e68f848653ffd0>`(
			:ref:`AdjacentQGates<doxid-class_q_panda_1_1_adjacent_q_gates>`& parent,
			TraversalStatue s
			);

		// methods
	
		void :target:`handle_QGate<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a2834090af5c915cb87e54b63e9a31e28>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QMeasure<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a8cbe68b6b66611f4f5882c95d377252a>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QReset<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a648ca59661252ec94363a5f432390b79>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_enter_QIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a250579efbb167c317576010f273146bf>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_leave_QIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1af0b73599f05e55c08ffea9af79f1d31c>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_enter_QWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1ae0e7e0e7051a57a2e0ee58ab6fb678b6>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_leave_QWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a1a31740985b6657739793b4a16df0edc>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_classical_prog<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1ad67ac9e287e0327eabbbfbf67f768f06>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		TraversalStatue :target:`get_statue<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a502bd7ec4ab628b4412eda45ca131bde>`() const;
	};
