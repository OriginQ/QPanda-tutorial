.. index:: pair: struct; QPanda::JsonBackendParser<WeightedGraph<T>>
.. _doxid-struct_q_panda_1_1_json_backend_parser_3_01_weighted_graph_3_01_t_01_4_01_4:

template struct QPanda::JsonBackendParser<WeightedGraph<T>>
===========================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Graph.h>
	
	template <class T>
	struct JsonBackendParser<WeightedGraph<T>>
	{
		// methods
	
		static :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` :target:`ParseWeight<doxid-struct_q_panda_1_1_json_backend_parser_3_01_weighted_graph_3_01_t_01_4_01_4_1a5f98ba13b45838bbb5cb584a38dc2f4b>`(const rapidjson::Value& v);
		static std::unique_ptr<:ref:`WeightedGraph<doxid-class_q_panda_1_1_weighted_graph>`<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>> :target:`Parse<doxid-struct_q_panda_1_1_json_backend_parser_3_01_weighted_graph_3_01_t_01_4_01_4_1ac71a7795e1bfce4e04619b758cbd3ce5>`(const rapidjson::Value& root);
	};
