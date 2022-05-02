.. index:: pair: struct; QPanda::JsonBackendParser
.. _doxid-struct_q_panda_1_1_json_backend_parser:

template struct QPanda::JsonBackendParser
=========================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Graph.h>
	
	template <class T>
	struct JsonBackendParser
	{
		// methods
	
		static std::unique_ptr<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> :target:`Parse<doxid-struct_q_panda_1_1_json_backend_parser_1aec705aed1be7758442272ccbed450c45>`(const rapidjson::Value& root);
		int32_t :target:`ParseWeight<doxid-struct_q_panda_1_1_json_backend_parser_1ac66f0e393fb6b9ac0814d0d96b3bb031>`(const rapidjson::Value& v);
		uint32_t :target:`ParseWeight<doxid-struct_q_panda_1_1_json_backend_parser_1a4df5cae295f33455efc245c8dca1d7ff>`(const rapidjson::Value& v);
		double :target:`ParseWeight<doxid-struct_q_panda_1_1_json_backend_parser_1a563adb630cd63f7826ae409fa3709343>`(const rapidjson::Value& v);
	};
