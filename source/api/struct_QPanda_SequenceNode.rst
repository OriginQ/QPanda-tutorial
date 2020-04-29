.. index:: pair: struct; QPanda::SequenceNode
.. _doxid-struct_q_panda_1_1_sequence_node:

struct QPanda::SequenceNode
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	struct SequenceNode
	{
		// fields
	
		int :target:`m_node_type<doxid-struct_q_panda_1_1_sequence_node_1aa94a4f520ee2a396619f20dd87e5612e>`;
		size_t :target:`m_vertex_num<doxid-struct_q_panda_1_1_sequence_node_1ab1a95d92a56bf2ca3088a2215b0c7c72>`;

		// methods
	
		bool :target:`operator ==<doxid-struct_q_panda_1_1_sequence_node_1a74f611c7422581af76549d3123c343cf>` (const SequenceNode& node) const;
		bool :target:`operator <<doxid-struct_q_panda_1_1_sequence_node_1ae03ac78a111c877cc3b2008e8d3ebc6e>` (const SequenceNode& node) const;
		bool :target:`operator ><doxid-struct_q_panda_1_1_sequence_node_1a605d6b0906bd65d9cd4a8d3939490386>` (const SequenceNode& node) const;
	};
