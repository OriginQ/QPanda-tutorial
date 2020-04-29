.. index:: pair: class; QPanda::QProgToDAG
.. _doxid-class_q_panda_1_1_q_prog_to_d_a_g:

class QPanda::QProgToDAG
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgToDAG.h>
	
	class QProgToDAG
	{
	public:
		// methods
	
		template <typename _Ty>
		void :ref:`traversal<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1acb391f6e1c112941badaef61593f4fa0>`(_Ty& node, :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& prog_dag);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1ac85a60923f8a286026b1862b409d9203>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`&,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`&,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1a8dcde5ddae5f7ecaa300058d0a4d5ca7>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`&,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`&,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1acccae3bb6d65655b9cf0c9f8f69d1340>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`&,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`&,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1a8c97b66d7a03dff3b8f6cfb56a218ab2>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`&,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`&,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1a37172d3430823c95a490c3e9cceb5675>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`&,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`&,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1a7c59f4cf5762859398118f2a569472e5>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`&,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`&,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1a83aa2ba212fd7d14754d78a993077828>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`&,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`&,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&
			);
	};
.. _details-class_q_panda_1_1_q_prog_to_d_a_g:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; traversal
.. _doxid-class_q_panda_1_1_q_prog_to_d_a_g_1acb391f6e1c112941badaef61593f4fa0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty>
	void traversal(_Ty& node, :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& prog_dag)

traversal :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty&

		- node

	*
		- QProgDAG&

		- prog_dag



.. rubric:: Returns:

void

