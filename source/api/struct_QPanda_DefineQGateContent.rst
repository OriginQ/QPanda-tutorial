.. index:: pair: struct; QPanda::DefineQGateContent
.. _doxid-struct_q_panda_1_1_define_q_gate_content:

struct QPanda::DefineQGateContent
=================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginIRToQProg.h>
	
	struct DefineQGateContent
	{
		// fields
	
		std::string :target:`define_name<doxid-struct_q_panda_1_1_define_q_gate_content_1adb897b2729b4841f2279528c08a89a06>`;
		std::vector<std::string> :target:`formal_qubits<doxid-struct_q_panda_1_1_define_q_gate_content_1ad811c42ab582957d65f1e1dd7e657a56>`;
		std::vector<std::string> :target:`formal_angles<doxid-struct_q_panda_1_1_define_q_gate_content_1ab7a2920df1c12c4df88311852ad10668>`;
		std::vector<:ref:`CallGateInfo<doxid-struct_q_panda_1_1_call_gate_info>`> :target:`gate_bodys<doxid-struct_q_panda_1_1_define_q_gate_content_1ad35e83178f3609795be746f39aa0cedd>`;
	};
