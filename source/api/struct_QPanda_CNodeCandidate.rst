.. index:: pair: struct; QPanda::CNodeCandidate
.. _doxid-struct_q_panda_1_1_c_node_candidate:

template struct QPanda::CNodeCandidate
======================================

.. toctree::
	:hidden:

Composition of each candidate in phase 1.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OBMTQMapping.h>
	
	template <typename T>
	struct CNodeCandidate
	{
		// fields
	
		:ref:`Dep<doxid-struct_q_panda_1_1_dep>` :target:`dep<doxid-struct_q_panda_1_1_c_node_candidate_1a7b3661c1874c0d2624ec0b90bd24b758>`;
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` :target:`cNode<doxid-struct_q_panda_1_1_c_node_candidate_1a94bef281a561477e443f52c6142f140e>`;
		uint32_t :target:`weight<doxid-struct_q_panda_1_1_c_node_candidate_1a740d80ee5f6e6ed4adac8e2c9bc3cf28>`;

		// methods
	
		bool :target:`operator ><doxid-struct_q_panda_1_1_c_node_candidate_1a7f78358e370e96cce26355ce9e46513f>` (const CNodeCandidate& rhs) const;
	};
