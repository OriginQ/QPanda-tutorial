.. index:: pair: struct; QPanda::GateInfo
.. _doxid-struct_q_panda_1_1_gate_info:

struct QPanda::GateInfo
=======================

.. toctree::
	:hidden:

Save the parsed logical gate information.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QScheduler.h>
	
	struct GateInfo
	{
		// fields
	
		int :target:`target<doxid-struct_q_panda_1_1_gate_info_1af59b2beca19273ba2ac4cb0a0d87d021>`;
		int :target:`control<doxid-struct_q_panda_1_1_gate_info_1a8e16854a54aaf57e1cb8c2a06887d93b>`;
		int :target:`type<doxid-struct_q_panda_1_1_gate_info_1a24494399e63338da9c7e9316ddd84fff>`;
		bool :target:`is_dagger<doxid-struct_q_panda_1_1_gate_info_1a162f68e785eaec8d3b91e9e20bad5a01>`;
		std::vector<double> :target:`param<doxid-struct_q_panda_1_1_gate_info_1ace67ee382a8d6ee63440821fbd6dba9c>`;
		std::string :target:`gate_name<doxid-struct_q_panda_1_1_gate_info_1aa8228b8852f57fb9300593d7d60c5582>`;
		int :target:`barrier_id<doxid-struct_q_panda_1_1_gate_info_1ad4f4251cb1bcba59971b479b7e70cbce>`;
	};
