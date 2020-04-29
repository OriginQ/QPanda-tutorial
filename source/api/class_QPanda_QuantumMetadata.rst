.. index:: pair: class; QPanda::QuantumMetadata
.. _doxid-class_q_panda_1_1_quantum_metadata:

class QPanda::QuantumMetadata
=============================

.. toctree::
	:hidden:

Parse xml config and get metadata.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMetadata.h>
	
	class QuantumMetadata
	{
	public:
		// construction
	
		:target:`QuantumMetadata<doxid-class_q_panda_1_1_quantum_metadata_1aa9905b0bffe0e1abfccdd0731ee5600d>`(const std::string& filename = :ref:`CONFIG_PATH<doxid-_x_m_l_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`);

		// methods
	
		QuantumMetadata& :target:`operator =<doxid-class_q_panda_1_1_quantum_metadata_1aa5b73cb1b6ffad81333abb098f65c91c>` (const QuantumMetadata&);
	
		bool :target:`getMetadata<doxid-class_q_panda_1_1_quantum_metadata_1ae7ebd876b66430e515f2064471739c88>`(
			int& qubit_num,
			std::vector<std::vector<int>>& matrix
			);
	
		bool :target:`getQGate<doxid-class_q_panda_1_1_quantum_metadata_1a24ba457ae8c8c058b0f51fa984ee8b08>`(
			std::vector<std::string>& single_gates,
			std::vector<std::string>& double_gates
			);
	
		bool :target:`getGateTime<doxid-class_q_panda_1_1_quantum_metadata_1a61259949c41b23bf6ec4d041610565d0>`(std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t>& gate_time_map);
	};
