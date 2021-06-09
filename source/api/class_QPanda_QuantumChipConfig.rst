.. index:: pair: class; QPanda::QuantumChipConfig
.. _doxid-class_q_panda_1_1_quantum_chip_config:

class QPanda::QuantumChipConfig
===============================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <JsonConfigParam.h>
	
	class QuantumChipConfig
	{
	public:
		// methods
	
		bool :ref:`load_config<doxid-group___utilities_1ga98c94cb9fb11e2b999839427de8903e8>`(const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`);
	
		bool :target:`read_adjacent_matrix<doxid-class_q_panda_1_1_quantum_chip_config_1a18a47b000e78a29a6a8de6d1b25177a9>`(
			size_t& qubit_num,
			std::vector<std::vector<int>>& qubit_matrix
			);
	
		std::vector<int> :target:`read_high_frequency_qubit<doxid-class_q_panda_1_1_quantum_chip_config_1afae2c47f0316282d3c7aa986ca16918f>`();
		std::vector<double> :target:`read_compensate_angle<doxid-class_q_panda_1_1_quantum_chip_config_1a6d176c382aff748a1770d7b380a69fc7>`();
		void :target:`read_compensate_angle<doxid-class_q_panda_1_1_quantum_chip_config_1ae9aa5abae311ce7f29daf9c9d3a80dd4>`(std::map<std::pair<int, int>, std::vector<double>>&);
		size_t :target:`get_double_gate_clock<doxid-class_q_panda_1_1_quantum_chip_config_1a336fe04288d92b4c99667a9e787d8e32>`(const size_t default_val = 3);
		size_t :target:`get_single_gate_clock<doxid-class_q_panda_1_1_quantum_chip_config_1aff3a73ddda5a20435fabb4b62cc787c6>`(const size_t default_val = 1);
	};
.. _details-class_q_panda_1_1_quantum_chip_config:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; load_config
.. _doxid-group___utilities_1ga98c94cb9fb11e2b999839427de8903e8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool load_config(const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`)

Load config data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- std::string It can be configuration file or configuration data, which can be distinguished by file suffix, so the configuration file must be end with ".json", default is CONFIG_PATH



.. rubric:: Returns:

Return false if any error occurs, otherwise return true

