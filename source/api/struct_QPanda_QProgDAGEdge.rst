.. index:: pair: struct; QPanda::QProgDAGEdge
.. _doxid-struct_q_panda_1_1_q_prog_d_a_g_edge:

struct QPanda::QProgDAGEdge
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	struct QProgDAGEdge
	{
		// fields
	
		uint32_t :target:`m_from<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge_1aba66047b1cccc6137c99efb71efbb837>`;
		uint32_t :target:`m_to<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge_1a19df1b6388ed4f1cdec0498881e70a0c>`;
		uint32_t :target:`m_qubit<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge_1a5ebca6822d2b5b24da7f5826292c647e>`;

		// construction
	
		:target:`QProgDAGEdge<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge_1a4c707854f32c29da0a62b200b0615d5a>`(
			uint32_t from,
			uint32_t to,
			uint32_t qubit
			);

		// methods
	
		bool :target:`operator <<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge_1a36ee9817a449f893e5396d31e37c2278>` (const QProgDAGEdge& e) const;
		bool :target:`operator ==<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge_1ac8003576ae1b9df374c4097c69dea82e>` (const QProgDAGEdge& e) const;
	};
