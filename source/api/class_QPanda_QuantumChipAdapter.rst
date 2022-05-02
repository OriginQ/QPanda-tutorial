.. index:: pair: class; QPanda::QuantumChipAdapter
.. _doxid-class_q_panda_1_1_quantum_chip_adapter:

class QPanda::QuantumChipAdapter
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumChipAdapter.h>
	
	class QuantumChipAdapter
	{
	public:
		// construction
	
		:target:`QuantumChipAdapter<doxid-class_q_panda_1_1_quantum_chip_adapter_1a3dff3645c39212ffff4c200ac85b1892>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine,
			bool b_mapping = true,
			const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`
			);

		// methods
	
		void :target:`init<doxid-class_q_panda_1_1_quantum_chip_adapter_1aadd18c8a9c24097627260e425c7035be>`();
	
		void :target:`adapter_conversion<doxid-class_q_panda_1_1_quantum_chip_adapter_1a116b020160bf4334582e6794e5bae5d5>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& new_qvec
			);
	
		void :target:`mapping<doxid-class_q_panda_1_1_quantum_chip_adapter_1a905e646b69463dec34edfe2e9bbe3901>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	};
