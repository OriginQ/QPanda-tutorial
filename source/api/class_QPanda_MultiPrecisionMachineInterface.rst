.. index:: pair: class; QPanda::MultiPrecisionMachineInterface
.. _doxid-class_q_panda_1_1_multi_precision_machine_interface:

class QPanda::MultiPrecisionMachineInterface
============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMachineInterface.h>
	
	class MultiPrecisionMachineInterface
	{
	public:
		// methods
	
		virtual :ref:`stat_map<doxid-_q_panda_namespace_8h_1a5b1ec78da541eaa2f329249b544e0488>` :target:`getQState<doxid-class_q_panda_1_1_multi_precision_machine_interface_1afc7d04785262138464ef48b0b30016f5>`() = 0;
		virtual :ref:`qstate_type<doxid-_q_panda_namespace_8h_1aa3be5ca16b07cae5d6e1b07151ed01c0>` :target:`pMeasureBinIndex<doxid-class_q_panda_1_1_multi_precision_machine_interface_1a72d7e35e215d096d7e151933f6ff3aee>`(std::string) = 0;
		virtual :ref:`qstate_type<doxid-_q_panda_namespace_8h_1aa3be5ca16b07cae5d6e1b07151ed01c0>` :target:`pMeasureDecIndex<doxid-class_q_panda_1_1_multi_precision_machine_interface_1abf0fcd73b20d7593ebb8781393e3afdf>`(std::string) = 0;
		virtual :ref:`prob_map<doxid-_q_panda_namespace_8h_1a7f2845d06ff66a209709171dcb1f696a>` :target:`PMeasure<doxid-class_q_panda_1_1_multi_precision_machine_interface_1abfdd0ddde21e97f332f365faa20eb264>`(std::string) = 0;
	
		virtual :ref:`prob_map<doxid-_q_panda_namespace_8h_1a7f2845d06ff66a209709171dcb1f696a>` :target:`PMeasure<doxid-class_q_panda_1_1_multi_precision_machine_interface_1aaeb86584756932cea97c59b785f42f80>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			std::string
			) = 0;
	
		virtual :ref:`prob_map<doxid-_q_panda_namespace_8h_1a7f2845d06ff66a209709171dcb1f696a>` :target:`getProbDict<doxid-class_q_panda_1_1_multi_precision_machine_interface_1a2c763d4fa92291d1b8722bfb3515ac07>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			std::string
			) = 0;
	
		virtual :ref:`prob_map<doxid-_q_panda_namespace_8h_1a7f2845d06ff66a209709171dcb1f696a>` :target:`probRunDict<doxid-class_q_panda_1_1_multi_precision_machine_interface_1a883557b6243e00d335ba7c0544a55b1d>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			std::string
			) = 0;
	};

	// direct descendants

	class :ref:`PartialAmplitudeQVM<doxid-class_q_panda_1_1_partial_amplitude_q_v_m>`;
