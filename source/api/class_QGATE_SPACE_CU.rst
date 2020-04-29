.. index:: pair: class; QGATE_SPACE::CU
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u:

class QGATE_SPACE::CU
=====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	class CU:
	    public :ref:`QGATE_SPACE::QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate>`,
	    public :ref:`QGATE_SPACE::AbstractAngleParameter<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`
	{
	public:
		// construction
	
		:target:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1a1c00777e1280b76219b974a71afc4c02>`(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* gate_old);
		:target:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1a3d4acc91c7381e688675cce96f6d30d3>`();
		:target:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1af13a0c3e4e84f3218f470a2c7ec1b185>`(const CU&);
	
		:target:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1a953617fca67f1c400a10b32634e921fe>`(
			double,
			double,
			double,
			double
			);
	
		:target:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1a2a992c419b3b3753faaa6770845bd5c0>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix);

		// methods
	
		virtual double :target:`getAlpha<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1a804e8e00ac8f253353ba83cf31ab91b5>`() const;
		virtual double :target:`getBeta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1ae81694f5fe0333668755600d0bb8f733>`() const;
		virtual double :target:`getGamma<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1a095a429643b55cf42acf908304695fb7>`() const;
		virtual double :target:`getDelta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1aae03371d2d34cd6ce6c157ddf8cae942>`() const;
		virtual int :target:`getOperationNum<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u_1a5f1eb49512a6de16971ee84ed54a88e8>`() const;
	};

	// direct descendants

	class :ref:`CNOT<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_n_o_t>`;
	class :ref:`CPHASE<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_p_h_a_s_e>`;
	class :ref:`CZ<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_z>`;

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
		virtual double :ref:`getAlpha<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a726b5732056952cab570ff925da28a30>`() const = 0;
		virtual double :ref:`getBeta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a09bbf9d9bf02741965ed009d61153013>`() const = 0;
		virtual double :ref:`getGamma<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1abd5096955f680570ef4077f5c58b4144>`() const = 0;
		virtual double :ref:`getDelta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a2b2bb0cd10344829991a186617317362>`() const = 0;

