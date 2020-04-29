.. index:: pair: class; QPanda::AdjacentQGates::AbstractTraversalStatueInterface
.. _doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface:

class QPanda::AdjacentQGates::AbstractTraversalStatueInterface
==============================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class AbstractTraversalStatueInterface
	{
	public:
		// methods
	
		virtual void :target:`handleQGate<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a6cc17f2de486aab00d5150eedb4a0d04>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handleQMeasure<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1afcbbf3dc2a3a77523fd1547787d7df9b>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handleQReset<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1af2a36ff2080bde1506b9b19194681f3d>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`onEnterQIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a9b1c56541260315cfba4247de807e151>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`onLeaveQIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a97bb83e1ccbbacb5e36f879afc7154c2>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`onEnterQWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a7d54e493f741e6afb1560421954a9c86>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`onLeaveQWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1addf469d026a5de73f158ac857a5d2693>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handleQClassicalProg<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a1f6fdb580cd11e3158e8fb356eef9910>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual TraversalStatue :target:`getStatue<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a5b18b5304028df4b6a88279c66fb1d72>`() const = 0;
	};
