.. index:: pair: struct; QPanda::MappingCandidate
.. _doxid-struct_q_panda_1_1_mapping_candidate:

struct QPanda::MappingCandidate
===============================

.. toctree::
	:hidden:

Composition of each candidate in phase 1.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OBMTQMapping.h>
	
	struct MappingCandidate
	{
		// fields
	
		:ref:`Mapping<doxid-namespace_q_panda_1a7b5fe6d8f00345359e7ae23d05af5e24>` :target:`m<doxid-struct_q_panda_1_1_mapping_candidate_1abc0eb4457ef4b3873c1a7f93b5afbdb4>`;
		uint32_t :target:`cost<doxid-struct_q_panda_1_1_mapping_candidate_1af684c5932268c0e10d01b1db48414dca>`;
		double :target:`reliability<doxid-struct_q_panda_1_1_mapping_candidate_1a17fc71705de72544058b52b71e02d54b>` = 1.0;
		uint32_t :target:`weight<doxid-struct_q_panda_1_1_mapping_candidate_1a971aecc7c0d9059b4003ab48bc9f91ed>`;

		// methods
	
		bool :target:`operator ><doxid-struct_q_panda_1_1_mapping_candidate_1ab48baa9b61a8962d6159beb9967dec7b>` (const MappingCandidate& rhs) const;
	};
