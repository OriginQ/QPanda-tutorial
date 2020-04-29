.. index:: pair: class; QGATE_SPACE::U4
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4:

class QGATE_SPACE::U4
=====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	class U4:
	    public :ref:`QGATE_SPACE::QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`,
	    public :ref:`QGATE_SPACE::AbstractAngleParameter<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`,
	    public :ref:`QGATE_SPACE::DynamicCreator<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator>`
	{
	public:
		// construction
	
		:target:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1a4eb573ccef0525a8a7d3a9f45e79ffa9>`();
		:target:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1a3fbe341141c46e652daab28ac6948472>`(U4&);
	
		:target:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1a481f852987700e12d368e4ea4bfd4112>`(
			double,
			double,
			double,
			double
			);
	
		:target:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1aef578557c48c9c135d9a29a33880e5ef>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix);
		:target:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1aff79bd58432ee1901325e8105f7f51d4>`(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*);

		// methods
	
		virtual double :target:`getAlpha<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1afc24874c7454f88ec6d849fd6587e866>`() const;
		virtual double :target:`getBeta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1a8efe95a4d09780f5500ff2f8f068ea8c>`() const;
		virtual double :target:`getGamma<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1af13e07e9e78ec1dfb64bc7ca02730d16>`() const;
		virtual double :target:`getDelta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1a89aa1e18c56fa2af55052183dfeb25f1>`() const;
		virtual int :target:`getOperationNum<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1a7849b9280ece4194b04d396d590f2004>`() const;
		virtual void :target:`getMatrix<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4_1ade92942339a947bab2995e3bfb7f931f>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix) const;
	};

	// direct descendants

	class :ref:`H<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_h>`;
	class :ref:`I<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i>`;
	class :ref:`RX<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_x>`;
	class :ref:`RY<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_y>`;
	class :ref:`RZ<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_z>`;
	class :ref:`S<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s>`;
	class :ref:`T<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_t>`;
	class :ref:`U1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u1>`;
	class :ref:`U2<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u2>`;
	class :ref:`U3<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u3>`;
	class :ref:`X<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_x>`;
	class :ref:`X1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_x1>`;
	class :ref:`Y<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_y>`;
	class :ref:`Y1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_y1>`;
	class :ref:`Z<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_z>`;
	class :ref:`Z1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_z1>`;

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
		virtual double :ref:`getAlpha<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a726b5732056952cab570ff925da28a30>`() const = 0;
		virtual double :ref:`getBeta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a09bbf9d9bf02741965ed009d61153013>`() const = 0;
		virtual double :ref:`getGamma<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1abd5096955f680570ef4077f5c58b4144>`() const = 0;
		virtual double :ref:`getDelta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_abstract_angle_parameter_1a2b2bb0cd10344829991a186617317362>`() const = 0;
		static :ref:`T<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_t>`* :ref:`CreateObject<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1a0fcbddf75bfd66e35b71d1917e06cbe9>`(Targs&&... args);

