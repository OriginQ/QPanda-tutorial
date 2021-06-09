.. index:: pair: struct; QPanda::MappingSwapSequence
.. _doxid-struct_q_panda_1_1_mapping_swap_sequence:

struct QPanda::MappingSwapSequence
==================================

.. toctree::
	:hidden:

Holds the sequence of ``Mapping`` s and ``Swaps`` to be executed.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OBMTQMapping.h>
	
	struct MappingSwapSequence
	{
		// fields
	
		std::vector<:ref:`Mapping<doxid-namespace_q_panda_1a7b5fe6d8f00345359e7ae23d05af5e24>`> :target:`mappings<doxid-struct_q_panda_1_1_mapping_swap_sequence_1a6a4ef9934a64bd6cb160228c7d500aed>`;
		std::vector<:ref:`SwapSeq<doxid-namespace_q_panda_1a4e66c639211525c3cf74a597216fb6a3>`> :target:`swapSeqs<doxid-struct_q_panda_1_1_mapping_swap_sequence_1a3420cb0108cf1caff699a246c769f08c>`;
		uint32_t :target:`cost<doxid-struct_q_panda_1_1_mapping_swap_sequence_1a2a6c22ffcda40849446e8a187f538d84>`;
		double :target:`reliability<doxid-struct_q_panda_1_1_mapping_swap_sequence_1a33d5bf1b3cde8a8a2727b6458ebbe12d>`;
	};
