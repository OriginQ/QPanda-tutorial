.. index:: pair: class; CPUImplQPUSingleThreadWithOracle
.. _doxid-class_c_p_u_impl_q_p_u_single_thread_with_oracle:

class CPUImplQPUSingleThreadWithOracle
======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CPUImplQPUSingleThread.h>
	
	class CPUImplQPUSingleThreadWithOracle: public :ref:`CPUImplQPUSingleThread<doxid-class_c_p_u_impl_q_p_u_single_thread>`
	{
	public:
		// methods
	
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`controlOracularGate<doxid-class_c_p_u_impl_q_p_u_single_thread_with_oracle_1acadad7c98309ecd36a9cc4a9bee129b2>`(
			std::vector<size_t> bits,
			std::vector<size_t> controlbits,
			bool is_dagger,
			std::string name
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// fields
	
		:ref:`vQParam<doxid-_q_p_u_impl_8h_1a902a178b3747917bdcc89bca8c9ccda5>` :ref:`qubit2stat<doxid-class_c_p_u_impl_q_p_u_single_thread_1ac6f9d1e0b5e2b446739a06435298d16f>`;

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
		:ref:`QGateParam<doxid-struct_q_gate_param>`& :ref:`findgroup<doxid-class_c_p_u_impl_q_p_u_single_thread_1ae0a179f07a503578e8011579fd8112b8>`(size_t qn);
		bool :ref:`TensorProduct<doxid-class_c_p_u_impl_q_p_u_single_thread_1a808fbf03e9cb4e65ab531bd72eb4f7ad>`(:ref:`QGateParam<doxid-struct_q_gate_param>`& qgroup0, :ref:`QGateParam<doxid-struct_q_gate_param>`& qgroup1);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_c_p_u_impl_q_p_u_single_thread_1a5ad2312e263c2c3b31d146e7897f6057>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_c_p_u_impl_q_p_u_single_thread_1a44abacfca1b382b2f48db02aa6246d99>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_c_p_u_impl_q_p_u_single_thread_1a89ad412af2f9c95906c6c0d448d31714>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_c_p_u_impl_q_p_u_single_thread_1a859a096b00f100ba58c4e57cca8688cb>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`P0<doxid-class_c_p_u_impl_q_p_u_single_thread_1ade2fabd7edcd24cfefee5d9845125cf6>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`P0<doxid-class_c_p_u_impl_q_p_u_single_thread_1aedbf9f7ea58caa40de9790cf69848f10>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`P1<doxid-class_c_p_u_impl_q_p_u_single_thread_1ac4a20655339a4beca74d6f9882289751>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`P1<doxid-class_c_p_u_impl_q_p_u_single_thread_1acd7ad7f8b630dd677a9e6b5d436281c4>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Hadamard<doxid-class_c_p_u_impl_q_p_u_single_thread_1a0754244bab7878ea8f3c104f51e24a91>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Hadamard<doxid-class_c_p_u_impl_q_p_u_single_thread_1a88d9e95d04c203e838cc98790d4bc370>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`X<doxid-class_c_p_u_impl_q_p_u_single_thread_1ac0ee94bd527596a0d5c232c00e24c531>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`X<doxid-class_c_p_u_impl_q_p_u_single_thread_1a19c8666a338f54d8ce97be78921cb77f>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Y<doxid-class_c_p_u_impl_q_p_u_single_thread_1a7d758ec914b25c1a52f26ae73527b753>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Y<doxid-class_c_p_u_impl_q_p_u_single_thread_1a8896f06559121d8e99da58f314aca73c>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Z<doxid-class_c_p_u_impl_q_p_u_single_thread_1a02eb4e704497d403a91a17ead45113de>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Z<doxid-class_c_p_u_impl_q_p_u_single_thread_1add5f999f0e94d6b7ce01c653d3777b30>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`T<doxid-class_c_p_u_impl_q_p_u_single_thread_1a8ea4fb7251d26edac734506f4b05fb03>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`T<doxid-class_c_p_u_impl_q_p_u_single_thread_1a5fb42de3396cb1d3d2d16ab60a8141d5>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`S<doxid-class_c_p_u_impl_q_p_u_single_thread_1a9271c8e73ed729702c2875e1fc23a461>`(size_t qn, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`S<doxid-class_c_p_u_impl_q_p_u_single_thread_1aa2c61d25401efc7c35ed41affc5fa7e4>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`U1_GATE<doxid-class_c_p_u_impl_q_p_u_single_thread_1a41bb6eb4c196d18fa192f6ddd094ea09>`(size_t qn, double theta, bool isConjugate, double error_rate);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`RX_GATE<doxid-class_c_p_u_impl_q_p_u_single_thread_1aa5568a4869013fdf9670585eb20d54c3>`(size_t qn, double theta, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`RX_GATE<doxid-class_c_p_u_impl_q_p_u_single_thread_1ae6b87b4ec1718334db89013e58a7eb94>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`RY_GATE<doxid-class_c_p_u_impl_q_p_u_single_thread_1a177d36d36e86ef722c7972d66d2d40ae>`(size_t qn, double theta, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`RY_GATE<doxid-class_c_p_u_impl_q_p_u_single_thread_1a3767073511f4717df3ed1eda1a54a919>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`RZ_GATE<doxid-class_c_p_u_impl_q_p_u_single_thread_1a5d5fcb29e97c79ebb1a62448a8443a73>`(size_t qn, double theta, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`RZ_GATE<doxid-class_c_p_u_impl_q_p_u_single_thread_1a215ae68884957ea7366b0e5fd0b97390>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`CNOT<doxid-class_c_p_u_impl_q_p_u_single_thread_1a060c550ab5c9395abd9ece46bc7ca77e>`(size_t qn_0, size_t qn_1, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`CNOT<doxid-class_c_p_u_impl_q_p_u_single_thread_1a03c47d3c7a3e9fd799cb1a309f68cb9a>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`CR<doxid-class_c_p_u_impl_q_p_u_single_thread_1a492d7b72338a1a8daee9d2247949ee3e>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`CR<doxid-class_c_p_u_impl_q_p_u_single_thread_1a21f3c7127a7fa3458af4f0621b66e9cd>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`CZ<doxid-class_c_p_u_impl_q_p_u_single_thread_1ad705f713886a617432d86af5412de8fb>`(size_t qn_0, size_t qn_1, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`CZ<doxid-class_c_p_u_impl_q_p_u_single_thread_1abf1df022ea3e796e8a7fc7047e2397b1>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`iSWAP<doxid-class_c_p_u_impl_q_p_u_single_thread_1a6b00908bce1832fd4b661fc48cda2cd9>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`iSWAP<doxid-class_c_p_u_impl_q_p_u_single_thread_1a50c4aa1294425fa82d162a55e013d01e>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`iSWAP<doxid-class_c_p_u_impl_q_p_u_single_thread_1ac98e3e307b38aa88fe6f64b0ae40efb2>`(size_t qn_0, size_t qn_1, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`iSWAP<doxid-class_c_p_u_impl_q_p_u_single_thread_1ac9784d2192406b6ce1b63fd0fa5d3bf6>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`SqiSWAP<doxid-class_c_p_u_impl_q_p_u_single_thread_1acd12530c19d6852dc70e8736bb18d8fc>`(size_t qn_0, size_t qn_1, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`SqiSWAP<doxid-class_c_p_u_impl_q_p_u_single_thread_1aa5fcb19a98df24f67a5bfc5b192fa913>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`DiagonalGate<doxid-class_c_p_u_impl_q_p_u_single_thread_1ab3f41b42c0a9474b58c3fdea93905abe>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, double error_rate);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlDiagonalGate<doxid-class_c_p_u_impl_q_p_u_single_thread_1a7df69cb42b99ce506dada1ddfebdb25a>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			);
	
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_c_p_u_impl_q_p_u_single_thread_1a4623d13103698b25ce2f857bacaccf8f>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_c_p_u_impl_q_p_u_single_thread_1ab2dcb7aeccdd64aa8397408e24b45678>`(size_t qn);
		virtual bool :ref:`qubitMeasure<doxid-class_c_p_u_impl_q_p_u_single_thread_1a1961d22bef2931f3ca57c7856830587f>`(size_t qn);
		:ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`pMeasure<doxid-class_c_p_u_impl_q_p_u_single_thread_1a9f3bf5a0e18ca75c5e7aba7696d4d1e3>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>`& mResult, int select_max = -1);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`pMeasure<doxid-class_c_p_u_impl_q_p_u_single_thread_1a22dab1f2f5f526ef86f27607076ef7e6>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`initState<doxid-class_c_p_u_impl_q_p_u_single_thread_1a96f9d128e05b60bdcc3b443cfe36bc00>`(size_t head_rank, size_t rank_size, size_t qubit_num);

