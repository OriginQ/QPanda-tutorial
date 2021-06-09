.. index:: pair: class; QPanda::QCircuitOptimizerConfig
.. _doxid-class_q_panda_1_1_q_circuit_optimizer_config:

class QPanda::QCircuitOptimizerConfig
=====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <JsonConfigParam.h>
	
	class QCircuitOptimizerConfig
	{
	public:
		// construction
	
		:target:`QCircuitOptimizerConfig<doxid-class_q_panda_1_1_q_circuit_optimizer_config_1ade0b4d66293fe23032fce04391329978>`(const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`);

		// methods
	
		bool :target:`get_replace_cir<doxid-class_q_panda_1_1_q_circuit_optimizer_config_1acbf07b7a2562e47520016cf3d235a53e>`(
			std::vector<std::pair<:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`>>& replace_cir_vec,
			std::string key_name = :ref:`QCIRCUIT_OPTIMIZER<doxid-_json_config_param_8h_1a90c1173bac3e0c194a52b65b22382c66>`
			);
	
		bool :target:`get_u3_replace_cir<doxid-class_q_panda_1_1_q_circuit_optimizer_config_1a6788bc0599d44182804df35aebdd0d6a>`(std::vector<std::pair<:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`>>& replace_cir_vec);
	};
