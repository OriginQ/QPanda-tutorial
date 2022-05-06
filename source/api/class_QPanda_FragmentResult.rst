.. index:: pair: class; QPanda::FragmentResult
.. _doxid-class_q_panda_1_1_fragment_result:

class QPanda::FragmentResult
============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CutQC.h>
	
	class FragmentResult
	{
	public:
		// fields
	
		std::vector<:ref:`PrepState<doxid-namespace_q_panda_1a54f0f73f8c66a656faa1b370508b60c1>`> :target:`m_prep_state<doxid-class_q_panda_1_1_fragment_result_1a59357ed77905075bef45adf4073dfaed>`;
		std::vector<:ref:`MeasBasis<doxid-namespace_q_panda_1ae12275c7a0d612f247bef65709e6304d>`> :target:`m_meas_basis<doxid-class_q_panda_1_1_fragment_result_1afc7c412e0c5ea7f2206867e78236497e>`;
		std::map<std::string, size_t> :target:`m_result<doxid-class_q_panda_1_1_fragment_result_1a2fe19dfb1e24df7cee717c935641a439>`;

		// construction
	
		:target:`FragmentResult<doxid-class_q_panda_1_1_fragment_result_1a7e6c935288cc1c23ce82094906a12aaf>`(
			size_t prep_num,
			size_t meas_num
			);

		// methods
	
		void :target:`set_meas_label<doxid-class_q_panda_1_1_fragment_result_1acf194ec0baf9a8fd1f754cbb23381459>`(
			size_t meas_qubit,
			:ref:`MeasBasis<doxid-namespace_q_panda_1ae12275c7a0d612f247bef65709e6304d>` basis
			);
	
		void :target:`set_prep_label<doxid-class_q_panda_1_1_fragment_result_1a1030d22bec2f8eb58ac2d3d8519e4721>`(
			size_t prep_qubit,
			:ref:`PrepState<doxid-namespace_q_panda_1a54f0f73f8c66a656faa1b370508b60c1>` state
			);
	};
