.. index:: pair: struct; QPanda::QProgDAGNode
.. _doxid-struct_q_panda_1_1_q_prog_d_a_g_node:

struct QPanda::QProgDAGNode
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	struct QProgDAGNode
	{
		// fields
	
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`m_itr<doxid-struct_q_panda_1_1_q_prog_d_a_g_node_1a662e8cb3b8b91c9612834b1b44a0d3f3>`;
		bool :target:`m_dagger<doxid-struct_q_panda_1_1_q_prog_d_a_g_node_1aa77c701b62ea3e9198a52973f24e02a1>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`m_qubits_vec<doxid-struct_q_panda_1_1_q_prog_d_a_g_node_1a3bca1eb2d8985c6832a25c766c0800c4>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`m_control_vec<doxid-struct_q_panda_1_1_q_prog_d_a_g_node_1a3ad910153c922f5e31608b8ae572094c>`;
		std::vector<double> :target:`m_angles<doxid-struct_q_panda_1_1_q_prog_d_a_g_node_1a1e0d0f1cecb56d19ec13ed9011ea158c>`;

		// methods
	
		void :target:`copy<doxid-struct_q_panda_1_1_q_prog_d_a_g_node_1a1ee5da94a467ca30a88b36f372498c84>`(std::shared_ptr<QProgDAGNode> node);
	};
