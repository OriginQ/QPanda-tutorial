.. index:: pair: class; QPanda::JudgeTwoNodeIterIsSwappable::OnInitStatue
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue:

class QPanda::JudgeTwoNodeIterIsSwappable::OnInitStatue
=======================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class OnInitStatue: public QPanda::JudgeTwoNodeIterIsSwappable::AbstractJudgeStatueInterface
	{
	public:
		// construction
	
		:target:`OnInitStatue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1a8a5c3616fbb813d8bd30da49c30c13ec>`(
			:ref:`JudgeTwoNodeIterIsSwappable<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable>`& parent,
			ResultStatue s
			);

		// methods
	
		void :target:`handle_QGate<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1abefafeddb6db2f91185c6927e19c59f1>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QMeasure<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1a317bcd273801aaec0440c3136d62bbf1>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handle_QReset<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1a4088fa16cd22b726f58dc766ee4db522>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		ResultStatue :target:`get_statue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1a6ddddfae53745d404e9c20b68b2ef824>`() const;
	};
