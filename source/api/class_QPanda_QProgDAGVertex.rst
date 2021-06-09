.. index:: pair: class; QPanda::QProgDAGVertex
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_vertex:

class QPanda::QProgDAGVertex
============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	class QProgDAGVertex
	{
	public:
		// fields
	
		std::shared_ptr<:ref:`QProgDAGNode<doxid-struct_q_panda_1_1_q_prog_d_a_g_node>`> :target:`m_node<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1afe6e70d56959d522393b2a9eb65339ad>`;
		uint32_t :target:`m_id<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1ae41b14830b77b1d6451a3ec049d402d6>`;
		:ref:`DAGNodeType<doxid-namespace_q_panda_1ab003414a5253d4a751cb89f052573337>` :target:`m_type<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1ad8ec70d10704d0c1f02ea49d64f61799>`;
		uint32_t :target:`m_layer<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1adfc79860e35b3b89208da9c9aa9873d2>`;
		bool :target:`m_invalid<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a3ca5f2e3720febe99c0491bc2ec73e06>`;
		std::vector<uint32_t> :target:`m_pre_node<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a156180b4b49fa46070c3c8100e54acfe>`;
		std::vector<uint32_t> :target:`m_succ_node<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a97f1ee98a2343815df79fd1190c16941>`;
		std::vector<:ref:`QProgDAGEdge<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge>`> :target:`m_pre_edges<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a41243b34ea85005a1a573cf8c5fd3b03>`;
		std::vector<:ref:`QProgDAGEdge<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge>`> :target:`m_succ_edges<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a5648fe72a80b0c9439b003f393935348>`;

		// methods
	
		bool :target:`is_pre_adjoin<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a450b306a3a075e78187e4f328847231f>`(const uint32_t& n);
		bool :target:`is_succ_adjoin<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1ac45f0f2af3bfd1aff855b51832cdfe1a>`(const uint32_t& n);
		void :target:`remove_pre_edge<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a38c5aadd4a54d4ef8936104a5d1270ac>`(const :ref:`QProgDAGEdge<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge>`& e);
		void :target:`remove_succ_edge<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex_1a0173960f4275d8d3392bfadfbe08bd8a>`(const :ref:`QProgDAGEdge<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge>`& e);
	};
