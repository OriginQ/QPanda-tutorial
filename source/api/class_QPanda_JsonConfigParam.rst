.. index:: pair: class; QPanda::JsonConfigParam
.. _doxid-class_q_panda_1_1_json_config_param:

class QPanda::JsonConfigParam
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

json configuration parameter :ref:`More...<details-class_q_panda_1_1_json_config_param>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <JsonConfigParam.h>
	
	class JsonConfigParam
	{
	public:
		// methods
	
		bool :ref:`load_config<doxid-group___utilities_1ga67e19e97887a059cdff2bd39e5e51dc7>`(const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`);
		rapidjson::Document& :target:`get_root_element<doxid-class_q_panda_1_1_json_config_param_1a51429c7f168c6c47df0397d4ee6c4dac>`();
	
		bool :target:`getMetadataConfig<doxid-class_q_panda_1_1_json_config_param_1a1a105fcff2aab204ec57d307c16c2e85>`(
			int& qubit_num,
			std::vector<std::vector<double>>& qubit_matrix
			);
	
		bool :target:`getClassNameConfig<doxid-class_q_panda_1_1_json_config_param_1a3846f68e78279009ba70199d357a87c2>`(std::map<std::string, std::string>& class_names);
		bool :target:`getQuantumCloudConfig<doxid-class_q_panda_1_1_json_config_param_1ad362949cab101a06463d6da61dd47524>`(std::map<std::string, std::string>& cloud_config);
	
		bool :target:`getQGateConfig<doxid-class_q_panda_1_1_json_config_param_1a8c33bcd7b7ebbba85a3dbdd7f134e325>`(
			std::vector<std::string>& single_gates,
			std::vector<std::string>& double_gates
			);
	
		bool :target:`getQGateTimeConfig<doxid-class_q_panda_1_1_json_config_param_1a4ccab661f2618e936bce3fae0a05980a>`(std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t>& gate_time);
		bool :target:`getInstructionConfig<doxid-class_q_panda_1_1_json_config_param_1a220b9c21a3bb5ef5cf6981615118c3c6>`(std::map<std::string, std::map<std::string, uint32_t>>&);
	
		static bool :ref:`readAdjacentMatrix<doxid-group___utilities_1ga7e179045bbde3f080538907729fb51c1>`(
			const rapidjson::Value& AdjacentMatrixElement,
			int& qubit_num,
			std::vector<std::vector<double>>& qubit_matrix
			);
	
		static bool :ref:`loadQuantumTopoStructure<doxid-class_q_panda_1_1_json_config_param_1af6bcc59ff38732f3f147cb22e9f6015e>`(
			const std::string& xmlStr,
			const std::string& dataElementStr,
			int& qubitsCnt,
			std::vector<std::vector<double>>& vec,
			const std::string configFile = ""
			);
	};
.. _details-class_q_panda_1_1_json_config_param:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

json configuration parameter

Methods
-------

.. index:: pair: function; load_config
.. _doxid-group___utilities_1ga67e19e97887a059cdff2bd39e5e51dc7:

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

.. index:: pair: function; readAdjacentMatrix
.. _doxid-group___utilities_1ga7e179045bbde3f080538907729fb51c1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool readAdjacentMatrix(
		const rapidjson::Value& AdjacentMatrixElement,
		int& qubit_num,
		std::vector<std::vector<double>>& qubit_matrix
		)

read topological structure from json config file



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- rapidjson::Value& json value

	*
		- int&

		- qubit number

	*
		- std::vector<std::vector<int>>

		- qubit matrix



.. rubric:: Returns:

bool

.. index:: pair: function; loadQuantumTopoStructure
.. _doxid-class_q_panda_1_1_json_config_param_1af6bcc59ff38732f3f147cb22e9f6015e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool loadQuantumTopoStructure(
		const std::string& xmlStr,
		const std::string& dataElementStr,
		int& qubitsCnt,
		std::vector<std::vector<double>>& vec,
		const std::string configFile = ""
		)

load quantum circuit topological structure

