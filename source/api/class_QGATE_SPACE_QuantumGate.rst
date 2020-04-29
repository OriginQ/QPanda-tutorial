.. index:: pair: class; QGATE_SPACE::QuantumGate
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate:

class QGATE_SPACE::QuantumGate
==============================

.. toctree::
	:hidden:

Quantum gate basic abstract class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	class QuantumGate
	{
	public:
		// methods
	
		virtual int :target:`getOperationNum<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate_1ae84f0c5af3aa9db49358e3dbd6f8fd40>`() const = 0;
		virtual void :target:`getMatrix<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate_1aa22f882bf37503ce15b4fb423389ecee>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix) const = 0;
		virtual int :target:`getGateType<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate_1a5f478d9bc1ffa9d7d9785314f4230327>`() const;
	};

	// direct descendants

	class :ref:`OracularGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate>`;
	class :ref:`QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate>`;
	class :ref:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4>`;
