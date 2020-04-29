.. index:: pair: class; QPanda::XmlConfigParam
.. _doxid-class_q_panda_1_1_xml_config_param:

class QPanda::XmlConfigParam
============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Xml configuration parameter. :ref:`More...<details-class_q_panda_1_1_xml_config_param>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <XMLConfigParam.h>
	
	class XmlConfigParam
	{
	public:
		// methods
	
		bool :target:`loadFile<doxid-class_q_panda_1_1_xml_config_param_1ab1f94b0314d2a7f7c3120146a742c04d>`(const std::string& filename);
	
		bool :target:`getMetadataConfig<doxid-class_q_panda_1_1_xml_config_param_1af4ce4b82f841c19b8922fe8193c4906a>`(
			int& qubit_num,
			std::vector<std::vector<int>>& qubit_matrix
			);
	
		bool :target:`getClassNameConfig<doxid-class_q_panda_1_1_xml_config_param_1a93d73b8933fff65b986566a03def9be3>`(std::map<std::string, std::string>& class_names);
		bool :target:`getQuantumCloudConfig<doxid-class_q_panda_1_1_xml_config_param_1a074ff8bbc874df953e269d506e1d2b7e>`(std::map<std::string, std::string>& cloud_config);
	
		bool :target:`getQGateConfig<doxid-class_q_panda_1_1_xml_config_param_1a7a294e06dce068c6f843d5e87c238168>`(
			std::vector<std::string>& single_gates,
			std::vector<std::string>& double_gates
			);
	
		bool :target:`getQGateTimeConfig<doxid-class_q_panda_1_1_xml_config_param_1a869519d7ebc7f76f423c2e202672e955>`(std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t>& gate_time);
		bool :target:`getInstructionConfig<doxid-class_q_panda_1_1_xml_config_param_1a5fc8efd5d40d7e58c3162be24f8d003c>`(std::map<std::string, std::map<std::string, uint32_t>>&);
		TiXmlElement* :target:`get_root_element<doxid-class_q_panda_1_1_xml_config_param_1a30cee037e1597d255e9fecef2cb79174>`();
	
		static bool :ref:`readAdjacentMatrix<doxid-group___utilities_1ga4e141809ff97965ba3dee77eb8e198fa>`(
			TiXmlElement* AdjacentMatrixElement,
			int& qubit_num,
			std::vector<std::vector<int>>& qubit_matrix
			);
	
		static bool :ref:`loadQuantumTopoStructure<doxid-class_q_panda_1_1_xml_config_param_1ace3fc704df32857ac8e9ee1fb729afb8>`(
			const std::string& xmlStr,
			const std::string& dataElementStr,
			int& qubitsCnt,
			std::vector<std::vector<int>>& vec,
			const std::string configFile = ""
			);
	};
.. _details-class_q_panda_1_1_xml_config_param:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Xml configuration parameter.

Methods
-------

.. index:: pair: function; readAdjacentMatrix
.. _doxid-group___utilities_1ga4e141809ff97965ba3dee77eb8e198fa:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool readAdjacentMatrix(
		TiXmlElement* AdjacentMatrixElement,
		int& qubit_num,
		std::vector<std::vector<int>>& qubit_matrix
		)

read topological structure from xml config file



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- TiXmlElement\*

		- qubit vector

	*
		- int&

		- qubit number

	*
		- std::vector<std::vector<int>>

		- qubit matrix



.. rubric:: Returns:

bool

.. index:: pair: function; loadQuantumTopoStructure
.. _doxid-class_q_panda_1_1_xml_config_param_1ace3fc704df32857ac8e9ee1fb729afb8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool loadQuantumTopoStructure(
		const std::string& xmlStr,
		const std::string& dataElementStr,
		int& qubitsCnt,
		std::vector<std::vector<int>>& vec,
		const std::string configFile = ""
		)

load quantum circuit topological structure

