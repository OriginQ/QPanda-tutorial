.. index:: pair: class; QGATE_SPACE::QGateFactory
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_gate_factory:

template class QGATE_SPACE::QGateFactory
========================================

.. toctree::
	:hidden:

Quantum Gate Factory.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	template <typename ... Targs>
	class QGateFactory
	{
	public:
		// methods
	
		bool :target:`registClass<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_gate_factory_1ad1bba88f1d3ff9bd8e470bbc46874839>`(
			const std::string& type_name,
			std::function<:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*(Targs&&... args)> function
			);
	
		:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* :target:`getGateNode<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_gate_factory_1a0f59ae65cc18b3e6b0368233c6c3e21d>`(
			const std::string& type_name,
			Targs&&... args
			);
	
		static QGateFactory* :target:`getInstance<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_gate_factory_1ace3683d6c5a3944ed0fd8b0a3163feb6>`();
	};
