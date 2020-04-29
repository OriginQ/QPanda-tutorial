.. index:: pair: class; QPanda::SingleGateTypeValidator
.. _doxid-class_q_panda_1_1_single_gate_type_validator:

class QPanda::SingleGateTypeValidator
=====================================

.. toctree::
	:hidden:

Get single gate metadata Validator type.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <MetadataValidity.h>
	
	class SingleGateTypeValidator
	{
	public:
		// fields
	
		:ref:`MetadataValidity<doxid-class_q_panda_1_1_metadata_validity>` :target:`m_metadata_validity_functions<doxid-class_q_panda_1_1_single_gate_type_validator_1a08edbd91199ce9c9fb41d656478417b0>`;

		// methods
	
		static int :target:`GateType<doxid-class_q_panda_1_1_single_gate_type_validator_1a7a0104db56114defa997ecf8bcfaedeb>`(
			std::vector<std::string>& gates,
			std::vector<std::string>& valid_gates
			);
	};
