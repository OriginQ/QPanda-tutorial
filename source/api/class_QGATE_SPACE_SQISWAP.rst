.. index:: pair: class; QGATE_SPACE::SQISWAP
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_q_i_s_w_a_p:

class QGATE_SPACE::SQISWAP
==========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	class SQISWAP:
	    public :ref:`QGATE_SPACE::ISWAPTheta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p_theta>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`
	{
	public:
		// construction
	
		:target:`SQISWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_q_i_s_w_a_p_1aa3c40745e8ac332f7ef3c8574fb5c02a>`(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* gate_old);
		:target:`SQISWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_q_i_s_w_a_p_1aa7bac6f464b5ebfe87d88498c62a33d4>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// structs
	
		struct :ref:`Register<doxid-struct_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1_1_register>`;

		// fields
	
		static :ref:`Register<doxid-struct_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1_1_register>` :ref:`m_register<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1a48cae5de9a4b327c059bf7591974f47e>`;

		// methods
	
		virtual int :ref:`getOperationNum<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate_1ae84f0c5af3aa9db49358e3dbd6f8fd40>`() const = 0;
		virtual void :ref:`getMatrix<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate_1aa22f882bf37503ce15b4fb423389ecee>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix) const = 0;
		virtual int :ref:`getGateType<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate_1a5f478d9bc1ffa9d7d9785314f4230327>`() const;
		static :ref:`T<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_t>`* :ref:`CreateObject<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1a0fcbddf75bfd66e35b71d1917e06cbe9>`(Targs&&... args);
		virtual int :ref:`getOperationNum<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1a973d1bfbb4ff2a88d99af47fad1b2f84>`() const;
		virtual void :ref:`getMatrix<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1ad9c2e8d8e079179022d4624333d9b81e>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`&) const;
		virtual double :ref:`getParameter<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_single_angle_parameter_1a5ff797e26bd6933d2c58eeb3937d848a>`() const = 0;
		virtual double :ref:`getParameter<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p_theta_1a83b676d191c4e3aa0da782ffce306575>`() const;

