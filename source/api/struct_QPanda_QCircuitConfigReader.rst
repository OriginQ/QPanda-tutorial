.. index:: pair: struct; QPanda::QCircuitConfigReader
.. _doxid-struct_q_panda_1_1_q_circuit_config_reader:

struct QPanda::QCircuitConfigReader
===================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <JsonConfigParam.h>
	
	struct QCircuitConfigReader
	{
		// fields
	
		const rapidjson::Value& :target:`m_circuit_config<doxid-struct_q_panda_1_1_q_circuit_config_reader_1ae6d6774a5a0d00b5c01d0315be698615>`;
		:ref:`QCircuitGenerator<doxid-class_q_panda_1_1_q_circuit_generator>`& :target:`m_cir_generator<doxid-struct_q_panda_1_1_q_circuit_config_reader_1a7f6fbacf5a51ee679e1f134a0020f062>`;

		// construction
	
		:target:`QCircuitConfigReader<doxid-struct_q_panda_1_1_q_circuit_config_reader_1acd0e8d7b50762919ff820c40d0f8df96>`(
			const rapidjson::Value& circuit_config,
			:ref:`QCircuitGenerator<doxid-class_q_panda_1_1_q_circuit_generator>`& cir_generator
			);

		// methods
	
		void :target:`read_cir<doxid-struct_q_panda_1_1_q_circuit_config_reader_1a67171e17bcee28ac43b22a44a52c6361>`();
	};
