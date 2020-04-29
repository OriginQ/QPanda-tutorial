.. index:: pair: class; CPUImplQPU
.. _doxid-class_c_p_u_impl_q_p_u:

class CPUImplQPU
================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QPU implementation by CPU model. :ref:`More...<details-class_c_p_u_impl_q_p_u>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CPUImplQPU.h>
	
	class CPUImplQPU: public :ref:`QPUImpl<doxid-class_q_p_u_impl>`
	{
	public:
		// fields
	
		:ref:`vQParam<doxid-_q_p_u_impl_8h_1a902a178b3747917bdcc89bca8c9ccda5>` :target:`qubit2stat<doxid-class_c_p_u_impl_q_p_u_1aa4d533bad6ce676cd8769e7906b54d7a>`;

		// construction
	
		:target:`CPUImplQPU<doxid-class_c_p_u_impl_q_p_u_1aed275b188855a312323bf11a952f80ae>`();
		:target:`CPUImplQPU<doxid-class_c_p_u_impl_q_p_u_1ada8c102613dbf54f25c8d7eae667a9e5>`(size_t);

		// methods
	
		:ref:`QGateParam<doxid-struct_q_gate_param>`& :target:`findgroup<doxid-class_c_p_u_impl_q_p_u_1ae7015495d327ac3febcaa6c587d01c1d>`(size_t qn);
	
		bool :target:`TensorProduct<doxid-class_c_p_u_impl_q_p_u_1a5b1359f6aae369d905ae7ee4823d7c6e>`(
			:ref:`QGateParam<doxid-struct_q_gate_param>`& qgroup0,
			:ref:`QGateParam<doxid-struct_q_gate_param>`& qgroup1
			);
	
		template <
			const qcomplex_t & U00,
			const qcomplex_t & U01,
			const qcomplex_t & U10,
			const qcomplex_t & U11
			>
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`single_gate<doxid-class_c_p_u_impl_q_p_u_1a62224a27171c1233629d02e5cd73ff42>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`U1_GATE<doxid-class_c_p_u_impl_q_p_u_1a0dfcb12a2aac13ae2db3ec16b0025ebf>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		template <const double & Nx, const double & Ny, const double & Nz>
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`single_angle_gate<doxid-class_c_p_u_impl_q_p_u_1a1d8445fe7482fb105969c93e9a32db40>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		template <const double & Nx, const double & Ny, const double & Nz>
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`control_single_angle_gate<doxid-class_c_p_u_impl_q_p_u_1a16ed4373f09945e81b6602ee34c6dc31>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		template <
			const qcomplex_t & U00,
			const qcomplex_t & U01,
			const qcomplex_t & U10,
			const qcomplex_t & U11
			>
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`control_single_gate<doxid-class_c_p_u_impl_q_p_u_1a1d3bbaaa19d83a25bb75cba7776fbc52>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a36bdabba21dc0aae2c7e4342926a21c2>`(P0);
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a2e00cd324e4f5d4de9dcc3416902e47e>`(P1);
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a78ee1bba0d66a4217bec32328c65807d>`(X);
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a3f88c75d5474e9f5bb39244e995da2c3>`(Y);
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a6d8e9970146130e9ef3974e9b16e9973>`(Z);
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1adbe2ac2015d2a9a16e0f6ba62398348f>`(Hadamard);
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a15b3f5e6478c74bab29cd3faae00fee0>`(T);
		:target:`CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a18297463bcbbc3b124fff82a4c4e4fde>`(S);
		:target:`SINGLE_ANGLE_GATE<doxid-class_c_p_u_impl_q_p_u_1a399a3a98fec8815859e2556f411e10c2>`(:ref:`RX_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca0ef81629f054170a8bb71f850820bc3f>`);
		:target:`SINGLE_ANGLE_GATE<doxid-class_c_p_u_impl_q_p_u_1a164b37fa8a6359121365e341e1081337>`(:ref:`RY_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca7dc7565fd56d69ad24931133d0374267>`);
		:target:`SINGLE_ANGLE_GATE<doxid-class_c_p_u_impl_q_p_u_1acce440f35ed844ab7565a1882ad81163>`(:ref:`RZ_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca74648a1b57818d818c5f32770dde8fce>`);
		:target:`CONTROL_SINGLE_ANGLE_GATE<doxid-class_c_p_u_impl_q_p_u_1a751a38f122d52997884b5ebb8fe29d09>`(:ref:`RX_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca0ef81629f054170a8bb71f850820bc3f>`);
		:target:`CONTROL_SINGLE_ANGLE_GATE<doxid-class_c_p_u_impl_q_p_u_1a4cc3ae653d1f7b39f75c53fcc1e7e85f>`(:ref:`RY_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca7dc7565fd56d69ad24931133d0374267>`);
		:target:`CONTROL_SINGLE_ANGLE_GATE<doxid-class_c_p_u_impl_q_p_u_1a43ab74faec5e4c6c484577356952c1fa>`(:ref:`RZ_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca74648a1b57818d818c5f32770dde8fce>`);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a88d1744d47eaf11efae4e5e16d15a92f>`(Hadamard);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a26ebf3ec56f9c7dbb90f8b3febee3e38>`(X);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1aa1d86df8c3bdb112e5c92cec322b2a8f>`(Y);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1ab61bdb93cfe44242f4235f93c88ec1d4>`(Z);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a298d2f409e6e378b4b1f071df47c6bef>`(T);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1a01624fa85fdb503887da76d8b90bdbfe>`(S);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1af101b88564e785b447ca296cd2f2c3ae>`(P0);
		:target:`CONTROL_CONST_GATE<doxid-class_c_p_u_impl_q_p_u_1aa3c0fabc85e9a4e8b7c4d0547f7ecd14>`(P1);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CNOT<doxid-class_c_p_u_impl_q_p_u_1a2c988f60209e88780427eadb9bd453ad>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CNOT<doxid-class_c_p_u_impl_q_p_u_1a866c8c98b7a432345dd3ff4d86cd5b41>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_c_p_u_impl_q_p_u_1a9e62485830f28b32c91ec46978f0d505>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_c_p_u_impl_q_p_u_1ac766ca5f08cb9763db12c9c65963fcb8>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_c_p_u_impl_q_p_u_1a4226df2a6527cfc76c52c216fb1b1844>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_c_p_u_impl_q_p_u_1af378f2b4b2b6f02fa099f611d9e20461>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`SqiSWAP<doxid-class_c_p_u_impl_q_p_u_1a7bc9ae60fb97d6ca1e49e62b17eccc24>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`SqiSWAP<doxid-class_c_p_u_impl_q_p_u_1a505b48dcfa083e4ab86b910235de4e00>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CR<doxid-class_c_p_u_impl_q_p_u_1a3bb8d717f854ebfcbc07e7cb746fce1c>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CR<doxid-class_c_p_u_impl_q_p_u_1a5ef36b67cb18ed24678ef9963f705740>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CZ<doxid-class_c_p_u_impl_q_p_u_1acde237e9020151f62c92b3fa47b29f3b>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CZ<doxid-class_c_p_u_impl_q_p_u_1a897f9d455142499649059da91d0d3fef>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_c_p_u_impl_q_p_u_1a99f6be394fb9ed6d42f75fa787fbbec1>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_c_p_u_impl_q_p_u_1ac5ba6b2a6b1f868ecdd132a46633528b>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_c_p_u_impl_q_p_u_1a3bad44eb20d61666aab7c4f5df088bbc>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_c_p_u_impl_q_p_u_1ae6ef9236a4921e75aba1f59fd05cb7e9>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`DiagonalGate<doxid-class_c_p_u_impl_q_p_u_1a8a5887c193fe9b04bb2dd729c1fad649>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`controlDiagonalGate<doxid-class_c_p_u_impl_q_p_u_1a7fff3c97da4ea58161f73ba4fe24de36>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_c_p_u_impl_q_p_u_1ae39eb6921904abc0a22172ae91b35689>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_c_p_u_impl_q_p_u_1acf218e97f2b7186e0462ac59d8fa6c05>`(size_t qn);
		virtual bool :target:`qubitMeasure<doxid-class_c_p_u_impl_q_p_u_1a552868a3bfc1eef7b3216acb1ee22794>`(size_t qn);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`pMeasure<doxid-class_c_p_u_impl_q_p_u_1a6f36ed7b448a26c0b87118ba6cf9cd65>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>`& mResult,
			int select_max = -1
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`pMeasure<doxid-class_c_p_u_impl_q_p_u_1aa1b3116624d1fef768f08f5207b6e3fe>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`initState<doxid-class_c_p_u_impl_q_p_u_1a54e07ff0ab1b0a09ccf47e9ffb8e2078>`(
			size_t head_rank,
			size_t rank_size,
			size_t qubit_num
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P00<doxid-class_c_p_u_impl_q_p_u_1afff31187b87e15170be053652150cf0d>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P11<doxid-class_c_p_u_impl_q_p_u_1a40f8e01f96879373f4e59c26a1746410>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	};

	// direct descendants

	class :ref:`CPUImplQPUWithOracle<doxid-class_c_p_u_impl_q_p_u_with_oracle>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual bool :ref:`qubitMeasure<doxid-class_q_p_u_impl_1a8231dac2a0406c20032c871de6f45df3>`(size_t qn) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`pMeasure<doxid-class_q_p_u_impl_1a7b81f6f6dd6e1d3e56b812335cd26e5f>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`initState<doxid-class_q_p_u_impl_1a2fb637028cde700f9b415a9f0770eb02>`(size_t head_rank, size_t rank_size, size_t qubit_num) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_q_p_u_impl_1a5d4651b69e9ddcf7f3180b577a80ea22>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_q_p_u_impl_1ad1d0629c91a42e06e079d6d6c215c0a9>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ad5f00e8ccf36ca66f48f4c63b3650e61>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ac164d4305076d2d34f61997ef63a1f34>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_p_u_impl_1aa4152648b4001296305ee546a1136abc>`() = 0;
		virtual void :ref:`set_random_engine<doxid-class_q_p_u_impl_1ae8d102f1acac09f453c26f096d0e62ea>`(:ref:`RandomEngine<doxid-class_random_engine>`* rng);
		virtual double :ref:`get_random_double<doxid-class_q_p_u_impl_1a25c1af43b633e913810831a5bfd7c90d>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_q_p_u_impl_1a9087cb5109b90f3215093165b11b4218>`(size_t qn) = 0;

.. _details-class_c_p_u_impl_q_p_u:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPU implementation by CPU model.

Methods
-------

.. index:: pair: function; unitarySingleQubitGate
.. _doxid-class_c_p_u_impl_q_p_u_1a99f6be394fb9ed6d42f75fa787fbbec1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitarySingleQubitGate(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`)

unitary single qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

	*
		- QStat&

		- matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; controlunitarySingleQubitGate
.. _doxid-class_c_p_u_impl_q_p_u_1ac5ba6b2a6b1f868ecdd132a46633528b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitarySingleQubitGate(
		size_t qn,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

controlunitary single qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

	*
		- Qnum&

		- control qubit addresses

	*
		- QStat

		- & matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; unitaryDoubleQubitGate
.. _doxid-class_c_p_u_impl_q_p_u_1a3bad44eb20d61666aab7c4f5df088bbc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

unitary double qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- first qubit address

	*
		- size_t

		- second qubit address

	*
		- QStat&

		- matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; controlunitaryDoubleQubitGate
.. _doxid-class_c_p_u_impl_q_p_u_1ae6ef9236a4921e75aba1f59fd05cb7e9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

controlunitary double qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- first qubit address

	*
		- size_t

		- second qubit address

	*
		- Qnum&

		- control qubit addresses

	*
		- QStat&

		- quantum states

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; getQState
.. _doxid-class_c_p_u_impl_q_p_u_1ae39eb6921904abc0a22172ae91b35689:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getQState()

get quantum states

.. index:: pair: function; Reset
.. _doxid-class_c_p_u_impl_q_p_u_1acf218e97f2b7186e0462ac59d8fa6c05:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` Reset(size_t qn)

reset qubit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

