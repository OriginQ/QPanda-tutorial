.. index:: pair: class; QPanda::DoubleGateTypeValidator
.. _doxid-class_q_panda_1_1_double_gate_type_validator:

class QPanda::DoubleGateTypeValidator
=====================================

.. toctree::
	:hidden:

Get double gate metadata Validator type.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <MetadataValidity.h>
	
	class DoubleGateTypeValidator
	{
	public:
		// fields
	
		:ref:`MetadataValidity<doxid-class_q_panda_1_1_metadata_validity>` :target:`m_metadata_validity_functions<doxid-class_q_panda_1_1_double_gate_type_validator_1a53c0ac80188f9b110e4702c860a9333a>`;

		// methods
	
		static int :target:`GateType<doxid-class_q_panda_1_1_double_gate_type_validator_1ac56eb51512673122c418a4783a393ebc>`(
			std::vector<std::string>& gates,
			std::vector<std::string>& valid_gates
			);
	};
