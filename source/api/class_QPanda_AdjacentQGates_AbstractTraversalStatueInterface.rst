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
	
		virtual void :target:`handle_QGate<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a04cd7c37c97ce1289fdc9c1a62282f27>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handle_QMeasure<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1aa6751e6ce014db528e90ef5a847f03c5>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handle_QReset<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a044bef399034ecea3b923a9861124f5e>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`on_enter_QIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a94e7809b8749e81cd70d475d7ed7a6d9>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`on_leave_QIf<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a91e61b3ca17777771e4a7698ec9fefd1>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`on_enter_QWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a33aefb74c697184576bc50ae7edc3237>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`on_leave_QWhile<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1ade0e632e10ccaa895fbe7e9428428c0f>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handle_classical_prog<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1a03cbeed0f6d6d126ae54b4324f08162f>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual TraversalStatue :target:`get_statue<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface_1ad6102a5b2ce7649f490e0dc7f39e4370>`() const = 0;
	};
