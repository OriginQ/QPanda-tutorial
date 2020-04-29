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
	
		virtual void :target:`handleQGate<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a964cb19c7481b132a6d73548eaa979e3>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handleQMeasure<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a7215663a19c0f1482b5efdb31a532c87>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`handleQReset<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a2132cff8afc7e95c2f6c5210a0da5720>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`onEnterFlowCtrlNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a96b9c56123f007ecf0515e13257bf52b>`();
		virtual void :target:`onLeaveFlowCtrlNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a5511333628843598ff0199f94561e93d>`();
	
		virtual void :target:`onEnterCircuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a7875c0ed682cc8de8b7051c7c42bd3d6>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		virtual void :target:`onLeaveCircuit<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a6560f6fd788c3b61f1ddff591a21b0cf>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		virtual void :target:`onTraversalEnd<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a2c273461f71b117f84cb6b64ee0c0984>`();
		virtual ResultStatue :target:`getStatue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface_1a32b91e7c61c936de14bfe40f3da112bf>`() const = 0;
	};
