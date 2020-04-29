.. index:: pair: class; NoisyCPUImplQPU
.. _doxid-class_noisy_c_p_u_impl_q_p_u:

class NoisyCPUImplQPU
=====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QPU implementation by noisy CPU model. :ref:`More...<details-class_noisy_c_p_u_impl_q_p_u>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NoiseCPUImplQPU.h>
	
	class NoisyCPUImplQPU: public :ref:`QPUImpl<doxid-class_q_p_u_impl>`
	{
	public:
		// fields
	
		:ref:`vQParam<doxid-_q_p_u_impl_8h_1a902a178b3747917bdcc89bca8c9ccda5>` :target:`qubit2stat<doxid-class_noisy_c_p_u_impl_q_p_u_1a8780ae068f79675005ef2c6fe1bd7a9a>`;

		// construction
	
		:target:`NoisyCPUImplQPU<doxid-class_noisy_c_p_u_impl_q_p_u_1a68b1c2009f2e19da346be2de9bddd4e1>`();
		:target:`NoisyCPUImplQPU<doxid-class_noisy_c_p_u_impl_q_p_u_1a6c9b24b2c39fe708d0aa73a3d806eb9f>`(rapidjson::Document&);

		// methods
	
		:ref:`QGateParam<doxid-struct_q_gate_param>`& :target:`findgroup<doxid-class_noisy_c_p_u_impl_q_p_u_1aa45b26b73b0b1e4b7138007bf7f2d07d>`(size_t qn);
	
		bool :target:`TensorProduct<doxid-class_noisy_c_p_u_impl_q_p_u_1a6220c92fac3bea63de391bf9fd52f1c9>`(
			:ref:`QGateParam<doxid-struct_q_gate_param>`& qgroup0,
			:ref:`QGateParam<doxid-struct_q_gate_param>`& qgroup1
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_noisy_c_p_u_impl_q_p_u_1a78448b5b2cdda5bb69f667c7cfee489d>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`noisyUnitarySingleQubitGate<doxid-class_noisy_c_p_u_impl_q_p_u_1af73aa3dadab367fdf15eef27ae27e8ae>`(
			size_t qn,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			bool isConjugate,
			:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_noisy_c_p_u_impl_q_p_u_1accd016e153610a7640b2d3d517fc04f6>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_noisy_c_p_u_impl_q_p_u_1a35757829c542e307f625898e80eab3ce>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`noisyUnitaryDoubleQubitGate<doxid-class_noisy_c_p_u_impl_q_p_u_1acd2e135405c1692a2f21865b97134a8d>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			bool isConjugate,
			:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_noisy_c_p_u_impl_q_p_u_1a9f2f6b4eaeb39af69efd7ed5523db6b3>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Hadamard<doxid-class_noisy_c_p_u_impl_q_p_u_1ae2cbb3961a5c27adea620bffe48328a8>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Hadamard<doxid-class_noisy_c_p_u_impl_q_p_u_1aca74bf06232d619b43ff1f20bb9f0239>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`X<doxid-class_noisy_c_p_u_impl_q_p_u_1a86c429f74d1d95aa592e1965231d3827>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`X<doxid-class_noisy_c_p_u_impl_q_p_u_1a731f5767a7d36ffa81e2731ae8261bdd>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P0<doxid-class_noisy_c_p_u_impl_q_p_u_1abc934817a6e774e048c5cc94920b4abf>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P0<doxid-class_noisy_c_p_u_impl_q_p_u_1a5a6407acc394a8c7420cdc8da78a4b63>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P1<doxid-class_noisy_c_p_u_impl_q_p_u_1a566672891363eaa46383600e514e8751>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P1<doxid-class_noisy_c_p_u_impl_q_p_u_1a5b2458bd921b14299a0d37d48fab5d58>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Y<doxid-class_noisy_c_p_u_impl_q_p_u_1a30097a0be36ab4730297af0d3d35ea86>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Y<doxid-class_noisy_c_p_u_impl_q_p_u_1a1960604c6157c57fed49bfbfbd7a98d2>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Z<doxid-class_noisy_c_p_u_impl_q_p_u_1a2c86eca744dcd28f97b76e68fef9e15c>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Z<doxid-class_noisy_c_p_u_impl_q_p_u_1a64ec050520e7f761453d529dc7703c4d>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`T<doxid-class_noisy_c_p_u_impl_q_p_u_1a8a8bfeb75ef28aca6cc6807df820ce93>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`T<doxid-class_noisy_c_p_u_impl_q_p_u_1ac43772d0b4017500df92c11dc6db5be0>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`S<doxid-class_noisy_c_p_u_impl_q_p_u_1a7b1dbc33489d42ec173da28757d067d7>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`S<doxid-class_noisy_c_p_u_impl_q_p_u_1a6f216221b77ec022b2012e5c515b0a1e>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`U1_GATE<doxid-class_noisy_c_p_u_impl_q_p_u_1a3af6ee35ec5d1cb2b583db9ce649f194>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RX_GATE<doxid-class_noisy_c_p_u_impl_q_p_u_1a0eea86fee45759ef38e7d408d7610877>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RX_GATE<doxid-class_noisy_c_p_u_impl_q_p_u_1a8893723fef3f202e847663ec8724d869>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RY_GATE<doxid-class_noisy_c_p_u_impl_q_p_u_1a715806ca03ef3c18e96f28f8f75bbd91>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RY_GATE<doxid-class_noisy_c_p_u_impl_q_p_u_1aca31b380ddc9034f5d0ef9e6b27c5b97>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RZ_GATE<doxid-class_noisy_c_p_u_impl_q_p_u_1a11f871f4358a82dc0e0e1b9f0e78e027>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RZ_GATE<doxid-class_noisy_c_p_u_impl_q_p_u_1a0107bb749acead49dc8f847b078d7b48>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CNOT<doxid-class_noisy_c_p_u_impl_q_p_u_1a80f7b8721b7adf911dea473452f8cda7>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CNOT<doxid-class_noisy_c_p_u_impl_q_p_u_1afbe6c37b6451afc4cad86e01cc36b795>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CR<doxid-class_noisy_c_p_u_impl_q_p_u_1a1f1f65ceb628a95c4128b255acf77f31>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CR<doxid-class_noisy_c_p_u_impl_q_p_u_1a8f8451551a882067ebb6f22c1fc5895d>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CZ<doxid-class_noisy_c_p_u_impl_q_p_u_1a1341f2f141e39914e53e7f56bf398b45>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CZ<doxid-class_noisy_c_p_u_impl_q_p_u_1aca76b5abc8beedb45e190f3843cd5b2a>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_noisy_c_p_u_impl_q_p_u_1a1b14d6c17ebbbaef439d5a38f80feb58>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_noisy_c_p_u_impl_q_p_u_1a2922ded08bd1f828bf752a3e1bbb6e3d>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_noisy_c_p_u_impl_q_p_u_1a53db126fccea1d3cd917f79f91d8c65b>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_noisy_c_p_u_impl_q_p_u_1a0560da234dced02793b1849839a8d228>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`SqiSWAP<doxid-class_noisy_c_p_u_impl_q_p_u_1add11a5e00de9e0907b2b973188ae960c>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`SqiSWAP<doxid-class_noisy_c_p_u_impl_q_p_u_1a12ec36f0c28c51db10fb297382ea8374>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`DiagonalGate<doxid-class_noisy_c_p_u_impl_q_p_u_1a85ec5bf611955ce5e5babce44372c51a>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`controlDiagonalGate<doxid-class_noisy_c_p_u_impl_q_p_u_1a8c82d90ed3795898b4678d9307dc1cbd>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_noisy_c_p_u_impl_q_p_u_1a393c993a3adaeaac1152d0bcd7d57f21>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_noisy_c_p_u_impl_q_p_u_1af96e2226f95a6397094b5380c4326525>`(size_t qn);
		virtual bool :target:`qubitMeasure<doxid-class_noisy_c_p_u_impl_q_p_u_1a457f9dec967873c956dbd2b1ac7d2e6e>`(size_t qn);
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`pMeasure<doxid-class_noisy_c_p_u_impl_q_p_u_1ad2f922e3fa82d087b92fb73013fc95c8>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>`& mResult,
			int select_max = -1
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`pMeasure<doxid-class_noisy_c_p_u_impl_q_p_u_1a7e48eae5f75246ace1ccceae0c22f207>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`initState<doxid-class_noisy_c_p_u_impl_q_p_u_1a3ef67d735f6c3281c3079756d77703b3>`(
			size_t head_rank,
			size_t rank_size,
			size_t qubit_num
			);
	};

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

.. _details-class_noisy_c_p_u_impl_q_p_u:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPU implementation by noisy CPU model.

Methods
-------

.. index:: pair: function; unitarySingleQubitGate
.. _doxid-class_noisy_c_p_u_impl_q_p_u_1a78448b5b2cdda5bb69f667c7cfee489d:

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
.. _doxid-class_noisy_c_p_u_impl_q_p_u_1accd016e153610a7640b2d3d517fc04f6:

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
.. _doxid-class_noisy_c_p_u_impl_q_p_u_1a35757829c542e307f625898e80eab3ce:

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
.. _doxid-class_noisy_c_p_u_impl_q_p_u_1a9f2f6b4eaeb39af69efd7ed5523db6b3:

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
.. _doxid-class_noisy_c_p_u_impl_q_p_u_1a393c993a3adaeaac1152d0bcd7d57f21:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getQState()

get quantum states

.. index:: pair: function; Reset
.. _doxid-class_noisy_c_p_u_impl_q_p_u_1af96e2226f95a6397094b5380c4326525:

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

