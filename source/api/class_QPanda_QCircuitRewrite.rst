.. index:: pair: class; QPanda::QCircuitRewrite
.. _doxid-class_q_panda_1_1_q_circuit_rewrite:

class QPanda::QCircuitRewrite
=============================

.. toctree::
	:hidden:

	struct_QPanda_QCircuitRewrite_SemMatch.rst
	struct_QPanda_QCircuitRewrite_StructMatch.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitRewrite.h>
	
	class QCircuitRewrite
	{
	public:
		// structs
	
		struct :ref:`SemMatch<doxid-struct_q_panda_1_1_q_circuit_rewrite_1_1_sem_match>`;
		struct :ref:`StructMatch<doxid-struct_q_panda_1_1_q_circuit_rewrite_1_1_struct_match>`;

		// fields
	
		:ref:`StructMatch<doxid-struct_q_panda_1_1_q_circuit_rewrite_1_1_struct_match>` :target:`m_struct<doxid-class_q_panda_1_1_q_circuit_rewrite_1ad07a37dfe0b7a1891a5b63910dc9a06e>`;
		:ref:`SemMatch<doxid-struct_q_panda_1_1_q_circuit_rewrite_1_1_sem_match>` :target:`m_sem<doxid-class_q_panda_1_1_q_circuit_rewrite_1a5b21fc786ac88ed56e17b65b201aea9a>`;
		std::set<int> :target:`matched<doxid-class_q_panda_1_1_q_circuit_rewrite_1a730eb7f48d0a06dcf492d456fadb8387>`;
		std::vector<std::map<int, int>> :target:`match_vertex_list<doxid-class_q_panda_1_1_q_circuit_rewrite_1adba62a315ba49498f69c143ddb1d3713>`;
		std::vector<std::map<int, int>> :target:`match_qubit_list<doxid-class_q_panda_1_1_q_circuit_rewrite_1aa920978f58f8773eccaf63154f0c3f28>`;
		std::vector<std::map<int, double>> :target:`match_angle_list<doxid-class_q_panda_1_1_q_circuit_rewrite_1a7e263db6b048e0545fdfd1360115eb8d>`;

		// methods
	
		std::shared_ptr<:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`> :target:`generator_to_dag<doxid-class_q_panda_1_1_q_circuit_rewrite_1a668c21007a7b8dd62c6a50e7787155a3>`(:ref:`QCircuitGenerator<doxid-class_q_panda_1_1_q_circuit_generator>`& cir_gen);
	
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`replace_subgraph<doxid-class_q_panda_1_1_q_circuit_rewrite_1afe710f2ada6864b20a82bcddde0718a9>`(
			std::shared_ptr<:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`> g,
			:ref:`QCircuitGenerator::Ref<doxid-class_q_panda_1_1_q_circuit_generator_1a27882a6e598c32bafffa9ea630a31d32>` cir_gen
			);
	
		void :target:`recursiveMatch<doxid-class_q_panda_1_1_q_circuit_rewrite_1af73d7ab6ab8f45d399fde5eb393d560e>`(
			std::shared_ptr<:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`> pattern,
			std::shared_ptr<:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`> graph,
			int i = 0
			);
	
		bool :target:`feasibilityRules<doxid-class_q_panda_1_1_q_circuit_rewrite_1a5aa1dc143d6094a34ca5d72ce811c26a>`(
			std::shared_ptr<:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`> pattern,
			std::shared_ptr<:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`> graph,
			int n,
			int m,
			:ref:`StructMatch<doxid-struct_q_panda_1_1_q_circuit_rewrite_1_1_struct_match>`& match
			);
	
		std::shared_ptr<:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`> :target:`circuitRewrite<doxid-class_q_panda_1_1_q_circuit_rewrite_1ad47093d96373ba1047cd7daf17bd14a0>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog,
			const std::string& config_data
			);
	
		static double :target:`angle_str_to_double<doxid-class_q_panda_1_1_q_circuit_rewrite_1a93b8617493ccf059b47a83f3ed9493dd>`(const std::string angle_str);
	};
