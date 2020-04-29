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
	
		void :target:`handleQGate<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1ade32761772dae60afec630570089df3d>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQMeasure<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1ac827db889e03e082fddb2b008ff570e5>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`handleQReset<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1a2b2e796e0e7b979c4f239590e99887cf>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		void :target:`onEnterFlowCtrlNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1ab1ca16d599e2f064f933e911e1e6cb08>`();
		void :target:`onLeaveFlowCtrlNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1ae874dc8247417d3de18e7839a2df468f>`();
	
		void :target:`onEnterCircuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1ae5f14a0b5ebb4f9180ba2c2fbe4889d3>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`onLeaveCircuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1a35eeb887f534fd8e8ff67c5aeccfe867>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		ResultStatue :target:`getStatue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue_1a8a7bf2b0ce80fbbe55b04710efdf8e39>`() const;
	};
