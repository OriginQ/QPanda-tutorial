.. index:: pair: class; QPanda::JudgeTwoNodeIterIsSwappable::OnPickUpNode
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node:

class QPanda::JudgeTwoNodeIterIsSwappable::OnPickUpNode
=======================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class OnPickUpNode: public QPanda::JudgeTwoNodeIterIsSwappable::AbstractJudgeStatueInterface
	{
	public:
		// construction
	
		:target:`OnPickUpNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1ad5214624bf02f9dc7be1edf22daa240f>`(
			:ref:`JudgeTwoNodeIterIsSwappable<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable>`& parent,
			ResultStatue s
			);

		// methods
	
		void :target:`handleQGate<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a02fdfc192d86a6b59f3f4e1dda55e3a3>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQMeasure<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1aee9e59028d46d0579e76d7ba19efd1b7>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQReset<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a58df6838209b4a1b1d7879dfd70be427>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onEnterFlowCtrlNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1ad2f682257558958aefc1071604d20a2c>`();
		void :target:`onLeaveFlowCtrlNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a9cc570754691cea0c9519765b20af36a>`();
	
		void :target:`onEnterCircuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a4b3e3bd294e833dab5c963532d65c273>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`onLeaveCircuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a8a6327c898272bbd935f774f2178406c>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`onTraversalEnd<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1ac244da8edaaff0b51a5fcc04e91dc329>`();
		ResultStatue :target:`getStatue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1ad5381b3ca175279b1486f93b0430ff0a>`() const;
	};
