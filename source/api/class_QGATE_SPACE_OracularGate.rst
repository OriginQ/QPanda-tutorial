.. index:: pair: class; QGATE_SPACE::OracularGate
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate:

class QGATE_SPACE::OracularGate
===============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	class OracularGate:
	    public :ref:`QGATE_SPACE::QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`
	{
	public:
		// construction
	
		:target:`OracularGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate_1a610143409be4b8a8041abfd32f918b25>`(std::string name);
		:target:`OracularGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate_1ae913b343f0b04c01b2ef0b4f39743174>`(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* qgate_old);

		// methods
	
		std::string :target:`get_name<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate_1a2c7bb96db0b77cfb26da153528e841d1>`() const;
		virtual int :target:`getOperationNum<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate_1a78d7040985504b8725e3e14b0651da02>`() const;
		virtual void :target:`getMatrix<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate_1a0cda00e88e6a1b989bb8843e2279c3a0>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix) const;
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

