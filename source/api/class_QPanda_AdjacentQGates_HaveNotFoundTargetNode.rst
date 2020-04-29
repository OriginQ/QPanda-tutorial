.. index:: pair: class; QPanda::AdjacentQGates::HaveNotFoundTargetNode
.. _doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node:

class QPanda::AdjacentQGates::HaveNotFoundTargetNode
====================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class HaveNotFoundTargetNode: public QPanda::AdjacentQGates::AbstractTraversalStatueInterface
	{
	public:
		// construction
	
		:target:`HaveNotFoundTargetNode<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a255e513395e052eacf40ee2cc5209e93>`(
			:ref:`AdjacentQGates<doxid-class_q_panda_1_1_adjacent_q_gates>`& parent,
			TraversalStatue s
			);

		// methods
	
		void :target:`handleQGate<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1acea9ab3a6c66a6b7c562d61334ec3cc0>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQMeasure<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a4bceb4ea60aeaeda45fd885a5d964f8c>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQReset<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a2b8d4ec2f788d5a3a6c2b45460bcbe4e>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onEnterQIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a452c565d815f0f3bb757d238e28be0a2>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onLeaveQIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a78453cd6c89b31db96e81e9ae53729c4>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onEnterQWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1ab029a3aab92ff77a1b77a21beda0dbe1>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onLeaveQWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1adef095f38fff080c5b2653834d4ac07c>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQClassicalProg<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a8568084649eac989c3c46ee2c40bc5a8>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		TraversalStatue :target:`getStatue<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a8cfe179ecb4ae13a3d5f37e94a3228e0>`() const;
	};
