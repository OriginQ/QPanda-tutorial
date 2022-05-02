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
	
		void :target:`handle_QGate<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a535d10cf9ae9c694e396ff32d3d7d7d8>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QMeasure<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1ac5c56758e2c75eb98e715102b5af3d5b>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QReset<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a45443f3c66a2f73914cc078ea3f9d3f6>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_enter_QIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a2e8e620b42054055c5d4abd703a79c5e>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_leave_QIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a58d71761f72141944076f3e8549f37bd>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_enter_QWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a21138a389f4d4c4b02193f28fc0aa26a>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`on_leave_QWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1ab4885161e9088d3ffe29f4daff3ae53c>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_classical_prog<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1ace0bbaeb9e35d067134440b926563e17>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		TraversalStatue :target:`get_statue<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node_1a8815b693223408838a586ebd204f7d15>`() const;
	};
