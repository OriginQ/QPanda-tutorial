.. index:: pair: class; QGATE_SPACE::QDoubleGate
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate:

class QGATE_SPACE::QDoubleGate
==============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	class QDoubleGate:
	    public :ref:`QGATE_SPACE::QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`
	{
	public:
		// construction
	
		:target:`QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1a7747dac203f2428ef23137fb12b8b679>`(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* gate_old);
		:target:`QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1a77cd850df596a47fbfb883c7dd89a7f9>`();
		:target:`QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1aac8760c20a05093073ccf13a4f93b54e>`(const QDoubleGate& oldDouble);
		:target:`QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1a3b932fb5184004f64a6c543952731dba>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix);

		// methods
	
		virtual int :target:`getOperationNum<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1a973d1bfbb4ff2a88d99af47fad1b2f84>`() const;
		virtual void :target:`getMatrix<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate_1ad9c2e8d8e079179022d4624333d9b81e>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`&) const;
	};

	// direct descendants

	class :ref:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u>`;
	class :ref:`ISWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p>`;
	class :ref:`ISWAPTheta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p_theta>`;
	class :ref:`SWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_w_a_p>`;

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

