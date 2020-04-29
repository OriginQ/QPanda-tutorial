.. index:: pair: struct; QPanda::QProgDAG::NodeInfo
.. _doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info:

struct QPanda::QProgDAG::NodeInfo
=================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	struct NodeInfo
	{
		// fields
	
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`m_itr<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info_1a3850613deb573033f78b194ffa9cc834>`;
		bool :target:`m_dagger<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info_1ab19770bcb70bb610589658b3df71f79e>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`m_qubits_vec<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info_1a763e35d65edb270ece70e97796c94c25>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`m_control_vec<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info_1a83d09941ced1f5a01236b128675df29a>`;

		// construction
	
		:target:`NodeInfo<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info_1a87cbb5d8068a0773bf2bc3ff3b11435c>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr);
	};
