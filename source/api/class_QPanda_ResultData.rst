.. index:: pair: class; QPanda::ResultData
.. _doxid-class_q_panda_1_1_result_data:

class QPanda::ResultData
========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CutQC.h>
	
	class ResultData
	{
	public:
		// fields
	
		std::vector<:ref:`PrepState<doxid-namespace_q_panda_1a54f0f73f8c66a656faa1b370508b60c1>`> :target:`m_prep_labels<doxid-class_q_panda_1_1_result_data_1aca0c5319e28cb3f7a4aa174a18e3d18b>`;
		std::vector<:ref:`MeasState<doxid-namespace_q_panda_1ab7992d9ff4516e91d26f7e9c50ed017e>`> :target:`m_meas_labels<doxid-class_q_panda_1_1_result_data_1a5f76e32b90c8332a615cf7e18c85ca19>`;

		// construction
	
		:target:`ResultData<doxid-class_q_panda_1_1_result_data_1a9c234a977dc1c11bf11b50f5e327399b>`(
			std::vector<:ref:`PrepState<doxid-namespace_q_panda_1a54f0f73f8c66a656faa1b370508b60c1>`> prep_labels,
			std::vector<:ref:`MeasState<doxid-namespace_q_panda_1ab7992d9ff4516e91d26f7e9c50ed017e>`> meas_labels
			);

		// methods
	
		bool :target:`operator <<doxid-class_q_panda_1_1_result_data_1a0efc0c9ea09840101333ea0853e9694a>` (const ResultData& data) const;
	};
