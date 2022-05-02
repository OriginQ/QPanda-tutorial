.. index:: pair: struct; QPanda::DAGSeqNode
.. _doxid-struct_q_panda_1_1_d_a_g_seq_node:

struct QPanda::DAGSeqNode
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	struct DAGSeqNode
	{
		// fields
	
		int :target:`m_node_type<doxid-struct_q_panda_1_1_d_a_g_seq_node_1aa9498c1b39ea265b00de1a24c0bd14ab>`;
		size_t :target:`m_vertex_num<doxid-struct_q_panda_1_1_d_a_g_seq_node_1a467bffebd21592189dd2f32f219d816b>`;

		// construction
	
		:ref:`DAGSeqNode<doxid-struct_q_panda_1_1_d_a_g_seq_node_1aa14fe10c2978907b6d85c46940ad0a4e>`();
		:target:`DAGSeqNode<doxid-struct_q_panda_1_1_d_a_g_seq_node_1a7940566245f6181f660d8ae6b4295ee5>`(const :ref:`QProgDAGVertex<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex>`& dag_vertex);

		// methods
	
		bool :target:`operator ==<doxid-struct_q_panda_1_1_d_a_g_seq_node_1ad759c416dc5468b5eba40ffb3c1abc40>` (const DAGSeqNode& node) const;
		bool :target:`operator <<doxid-struct_q_panda_1_1_d_a_g_seq_node_1aca04596b9b72d0f3ab7620d320004b78>` (const DAGSeqNode& node) const;
		bool :target:`operator ><doxid-struct_q_panda_1_1_d_a_g_seq_node_1af15fcbb9b5e79aeeb438638009a944e5>` (const DAGSeqNode& node) const;
	};
.. _details-struct_q_panda_1_1_d_a_g_seq_node:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Construction
------------

.. index:: pair: function; DAGSeqNode
.. _doxid-struct_q_panda_1_1_d_a_g_seq_node_1aa14fe10c2978907b6d85c46940ad0a4e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DAGSeqNode()

construct sequence node



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- vertex num



.. rubric:: Returns:

QPanda::SequenceNode

