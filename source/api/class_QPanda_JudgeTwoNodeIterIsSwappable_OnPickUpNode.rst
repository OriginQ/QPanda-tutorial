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
	
		void :target:`handle_QGate<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a36b50b68634cefb66cb7adf0596b7909>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QMeasure<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1abf9ef88a12a8abc97cb9b31647eb5e62>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QReset<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a3bfa833f04aa947ee7cbe464924d959e>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`enter_flow_ctrl_node<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a024a54065fd76db5afbb17fe4e2fe265>`();
		void :target:`leave_flow_ctrl_node<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a803053cb1f9e549b155055c224adeb89>`();
	
		void :target:`on_enter_circuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a7df53eb305edfbfa017f70695718651b>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`on_leave_circuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a32acad2590100951cb8b6089e108d703>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`on_enter_prog<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1ab7a1947e53af3d75a5a4d7d2aed8ff16>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`on_leave_prog<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1acf27bb1d3ff5c36bd39a979f16218d5e>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		ResultStatue :target:`get_statue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node_1a25056551e063c97fa8d7fde227280f21>`() const;
	};
