.. index:: pair: class; QPanda::JudgeTwoNodeIterIsSwappable::AbstractJudgeStatueInterface
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface:

class QPanda::JudgeTwoNodeIterIsSwappable::AbstractJudgeStatueInterface
=======================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class AbstractJudgeStatueInterface
	{
	public:
		// methods
	
		virtual void :target:`handle_QGate<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1ac2a9a122ba5ebe6ef7a4bf54cdebbf11>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handle_QMeasure<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a5b700b7ac794ad8604a55a2050158594>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handle_QReset<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1ac19f549e773648f20f9ac08e392e1646>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`enter_flow_ctrl_node<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1afe7b190b3ceeef716940ff6a229491a8>`();
		virtual void :target:`leave_flow_ctrl_node<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a388467558598aea35282b0c12d86453c>`();
	
		virtual void :target:`on_enter_circuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a37270a288de42323965a3cb98928ecc1>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		virtual void :target:`on_leave_circuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a31c04e5fe5b622886ef80127b273e9d6>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		virtual void :target:`on_enter_prog<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1aaf3704ed71aaf9a1b887765b9368c8a7>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		virtual void :target:`on_leave_prog<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a0b5b8a0a8a288750f7cf4d6d8ff75383>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		virtual void :target:`on_traversal_end<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1abc0d2c35cd2e2a14b124f0abb7d35b3f>`();
		virtual ResultStatue :target:`get_statue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a7c8884c5795c7f53de3c910bfbb7d7c3>`() const = 0;
	};
