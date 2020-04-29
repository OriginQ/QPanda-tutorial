.. index:: pair: struct; QPanda::GateOperationInfo
.. _doxid-struct_q_panda_1_1_gate_operation_info:

struct QPanda::GateOperationInfo
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QASMToQProg.h>
	
	struct GateOperationInfo
	{
		// fields
	
		std::string :target:`op_id<doxid-struct_q_panda_1_1_gate_operation_info_1a24c293aea2619c31edaa1940f138585a>`;
		std::vector<:ref:`RegParamInfo<doxid-struct_q_panda_1_1_reg_param_info>`> :target:`regs_vec<doxid-struct_q_panda_1_1_gate_operation_info_1a246f29a680f557e9644159f9e5347304>`;
		std::vector<std::shared_ptr<:ref:`Exp<doxid-class_q_panda_1_1_exp>`>> :target:`angles_vec<doxid-struct_q_panda_1_1_gate_operation_info_1ac8031fadcbba3f3935eab14522c62ed5>`;
	};
