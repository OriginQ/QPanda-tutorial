.. index:: pair: class; QGATE_SPACE::DynamicCreator
.. _doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator:

template class QGATE_SPACE::DynamicCreator
==========================================

.. toctree::
	:hidden:

	struct_QGATE_SPACE_DynamicCreator_Register.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumGate.h>
	
	template <typename T, typename ... Targs>
	class DynamicCreator
	{
	public:
		// structs
	
		struct :ref:`Register<doxid-struct_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1_1_register>`;

		// fields
	
		static :ref:`Register<doxid-struct_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1_1_register>` :target:`m_register<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1a48cae5de9a4b327c059bf7591974f47e>`;

		// methods
	
		static :ref:`T<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_t>`* :target:`CreateObject<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_dynamic_creator_1a0fcbddf75bfd66e35b71d1917e06cbe9>`(Targs&&... args);
	};

	// direct descendants

	class :ref:`CNOT<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_n_o_t>`;
	class :ref:`CNOT<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_n_o_t>`;
	class :ref:`CPHASE<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_p_h_a_s_e>`;
	class :ref:`CPHASE<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_p_h_a_s_e>`;
	class :ref:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u>`;
	class :ref:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u>`;
	class :ref:`CU<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_u>`;
	class :ref:`CZ<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_z>`;
	class :ref:`CZ<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_c_z>`;
	class :ref:`H<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_h>`;
	class :ref:`H<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_h>`;
	class :ref:`I<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i>`;
	class :ref:`I<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i>`;
	class :ref:`ISWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p>`;
	class :ref:`ISWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p>`;
	class :ref:`ISWAPTheta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p_theta>`;
	class :ref:`ISWAPTheta<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_i_s_w_a_p_theta>`;
	class :ref:`OracularGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate>`;
	class :ref:`OracularGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_oracular_gate>`;
	class :ref:`QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate>`;
	class :ref:`QDoubleGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_q_double_gate>`;
	class :ref:`RX<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_x>`;
	class :ref:`RX<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_x>`;
	class :ref:`RY<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_y>`;
	class :ref:`RY<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_y>`;
	class :ref:`RZ<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_z>`;
	class :ref:`RZ<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_r_z>`;
	class :ref:`S<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s>`;
	class :ref:`S<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s>`;
	class :ref:`SQISWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_q_i_s_w_a_p>`;
	class :ref:`SQISWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_q_i_s_w_a_p>`;
	class :ref:`SWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_w_a_p>`;
	class :ref:`SWAP<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_s_w_a_p>`;
	class :ref:`T<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_t>`;
	class :ref:`T<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_t>`;
	class :ref:`U1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u1>`;
	class :ref:`U1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u1>`;
	class :ref:`U2<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u2>`;
	class :ref:`U2<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u2>`;
	class :ref:`U3<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u3>`;
	class :ref:`U3<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u3>`;
	class :ref:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4>`;
	class :ref:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4>`;
	class :ref:`U4<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_u4>`;
	class :ref:`X<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_x>`;
	class :ref:`X<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_x>`;
	class :ref:`X1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_x1>`;
	class :ref:`X1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_x1>`;
	class :ref:`Y<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_y>`;
	class :ref:`Y<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_y>`;
	class :ref:`Y1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_y1>`;
	class :ref:`Y1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_y1>`;
	class :ref:`Z<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_z>`;
	class :ref:`Z<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_z>`;
	class :ref:`Z1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_z1>`;
	class :ref:`Z1<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_z1>`;
