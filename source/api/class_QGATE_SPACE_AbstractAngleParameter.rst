.. index:: pair: class; QGATE_SPACE::AbstractAngleParameter
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter:

class QGATE_SPACE::AbstractAngleParameter
=========================================

.. toctree::
	:hidden:

Quantum gate angle parameter basic abstract class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	class AbstractAngleParameter
	{
	public:
		// methods
	
		virtual double :target:`getAlpha<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a726b5732056952cab570ff925da28a30>`() const = 0;
		virtual double :target:`getBeta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a09bbf9d9bf02741965ed009d61153013>`() const = 0;
		virtual double :target:`getGamma<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1abd5096955f680570ef4077f5c58b4144>`() const = 0;
		virtual double :target:`getDelta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a2b2bb0cd10344829991a186617317362>`() const = 0;
	};

	// direct descendants

	class :ref:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u>`;
	class :ref:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4>`;
