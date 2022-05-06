.. index:: pair: struct; QPanda::CandidateSelector
.. _doxid-struct_q_panda_1_1_candidate_selector:

struct QPanda::CandidateSelector
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Interface for selecting candidates (if they are greater than a max) in phase 1. :ref:`More...<details-struct_q_panda_1_1_candidate_selector>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OBMTQMapping.h>
	
	struct CandidateSelector
	{
		// typedefs
	
		typedef CandidateSelector* :target:`Ref<doxid-struct_q_panda_1_1_candidate_selector_1a22f491f4f9971e858653eb772e943ee0>`;
		typedef std::unique_ptr<CandidateSelector> :target:`uRef<doxid-struct_q_panda_1_1_candidate_selector_1af31ad9af8ccee7de624d1482d3b69ef7>`;

		// methods
	
		virtual std::vector<:ref:`MappingCandidate<doxid-struct_q_panda_1_1_mapping_candidate>`> :ref:`select<doxid-struct_q_panda_1_1_candidate_selector_1af612716d32cfe7b564bc638aff776e6a>`(uint32_t maxCandidates, const std::vector<:ref:`MappingCandidate<doxid-struct_q_panda_1_1_mapping_candidate>`>& candidates) = 0;
	};
.. _details-struct_q_panda_1_1_candidate_selector:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Interface for selecting candidates (if they are greater than a max) in phase 1.

Methods
-------

.. index:: pair: function; select
.. _doxid-struct_q_panda_1_1_candidate_selector_1af612716d32cfe7b564bc638aff776e6a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`MappingCandidate<doxid-struct_q_panda_1_1_mapping_candidate>`> select(
		uint32_t maxCandidates,
		const std::vector<:ref:`MappingCandidate<doxid-struct_q_panda_1_1_mapping_candidate>`>& candidates
		) = 0

Selects *maxCandidates* from *candidates*.

