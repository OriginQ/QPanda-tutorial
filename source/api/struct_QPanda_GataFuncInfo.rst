.. index:: pair: struct; QPanda::GataFuncInfo
.. _doxid-struct_q_panda_1_1_gata_func_info:

struct QPanda::GataFuncInfo
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QASMToQProg.h>
	
	struct GataFuncInfo
	{
		// fields
	
		std::string :target:`func_name<doxid-struct_q_panda_1_1_gata_func_info_1aff5155c74190ae5433c36ce55d4b346b>`;
		std::vector<std::string> :target:`angle_names_vec<doxid-struct_q_panda_1_1_gata_func_info_1ac50751e1880b75fa2b1e6827f9b7e772>`;
		std::vector<std::string> :target:`reg_names_vec<doxid-struct_q_panda_1_1_gata_func_info_1abb28f48d38de50ff577475dfdf0bb623>`;
		std::vector<:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>`> :target:`ops_vec<doxid-struct_q_panda_1_1_gata_func_info_1a37a1299a1085689a7a08c9f351303240>`;
	};
