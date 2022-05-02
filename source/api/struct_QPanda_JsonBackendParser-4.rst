.. index:: pair: struct; QPanda::JsonBackendParser<Graph>
.. _doxid-struct_q_panda_1_1_json_backend_parser_3_01_graph_01_4:

template struct QPanda::JsonBackendParser<Graph>
================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Graph.h>
	
	template <>
	struct JsonBackendParser<Graph>
	{
		// methods
	
		static std::unique_ptr<:ref:`Graph<doxid-class_q_panda_1_1_graph>`> :target:`Parse<doxid-struct_q_panda_1_1_json_backend_parser_3_01_graph_01_4_1ab6ccf62664456977105effae0e4d6eee>`(const rapidjson::Value& root);
	};
