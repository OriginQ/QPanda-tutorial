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
	
		void :target:`handleQGate<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1afc5cd0c6c26aa7e7711083ccc3df478a>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQMeasure<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1aac22bd38352e29c33a6a3fa12ff69186>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQReset<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a8df9c124e783f728f5b77e856e15de37>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onEnterQIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a3f0b080cba48f0facad891b507c77738>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onLeaveQIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a1e24e51da9eb8734a68023cc3fe98d30>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onEnterQWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a7825b595767da6589edfb0be900457dc>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onLeaveQWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a9ed4381b50e97f0dcd2ed153cc731b0c>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQClassicalProg<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1ae4a1e3e1479e8df0d75c21553366391d>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		TraversalStatue :target:`getStatue<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node_1a22c4bdb093219bbc908e9cc2fc882d88>`() const;
	};
