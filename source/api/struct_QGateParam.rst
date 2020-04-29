.. index:: pair: struct; QGateParam
.. _doxid-struct_q_gate_param:

struct QGateParam
=================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGateParameter.h>
	
	struct QGateParam
	{
		// fields
	
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` :target:`qVec<doxid-struct_q_gate_param_1a9aaaeb284b1d1692da717a0a5da38d1a>`;
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`qstate<doxid-struct_q_gate_param_1a4af9f6f534b3bc2ed0142f8200edb2de>`;
		int :target:`qubitnumber<doxid-struct_q_gate_param_1a970712a176cbd7a2ea149f11c7dc0e7c>`;
		bool :target:`enable<doxid-struct_q_gate_param_1a7662c2c4c530f9f46b3ae05ebd2edbfb>`;

		// construction
	
		:target:`QGateParam<doxid-struct_q_gate_param_1ae1d826660003a40c99539073f2753668>`();
		:target:`QGateParam<doxid-struct_q_gate_param_1a71bb5aa92a1589a5fd976842100e4986>`(int qn);
	
		:target:`QGateParam<doxid-struct_q_gate_param_1af9618f174641a6abd95953512a33585f>`(
			int qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` num
			);
	};
