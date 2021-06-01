.. index:: pair: struct; QPanda::JsonBackendParser<ArchGraph>
.. _doxid-struct_q_panda_1_1_json_backend_parser_3_01_arch_graph_01_4:

template struct QPanda::JsonBackendParser<ArchGraph>
====================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ArchGraph.h>
	
	template <>
	struct JsonBackendParser<ArchGraph>
	{
		// methods
	
		static std::unique_ptr<:ref:`ArchGraph<doxid-class_q_panda_1_1_arch_graph>`> :target:`Parse<doxid-struct_q_panda_1_1_json_backend_parser_3_01_arch_graph_01_4_1ad0bc7a92c98161277a796c79c1d3e664>`(const rapidjson::Value& root);
	};
