.. index:: pair: struct; QPanda::CallGateInfo
.. _doxid-struct_q_panda_1_1_call_gate_info:

struct QPanda::CallGateInfo
===========================

.. toctree::
	:hidden:

define :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` function info


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginIRToQProg.h>
	
	struct CallGateInfo
	{
		// fields
	
		std::string :target:`gate_name<doxid-struct_q_panda_1_1_call_gate_info_1aafa89c4ab07dcc83a1c048a625fab920>`;
		std::vector<std::string> :target:`qubits<doxid-struct_q_panda_1_1_call_gate_info_1a9ec932052810f569771433580b852c9f>`;
		std::vector<std::shared_ptr<:ref:`Exp<doxid-class_q_panda_1_1_exp>`>> :target:`angles<doxid-struct_q_panda_1_1_call_gate_info_1afb76b30e1ba62fcbba1b842545296a9f>`;
	};
