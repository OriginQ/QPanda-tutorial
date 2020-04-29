.. _global:
.. index:: pair: namespace; global

Global Namespace
================

.. toctree::
	:hidden:

	namespace_Base64.rst
	namespace_GATEGPU.rst
	namespace_QGATE_SPACE.rst
	namespace_QPanda.rst
	namespace_gpu.rst
	namespace_std.rst
	enum_GateType.rst
	enum_MetadataGateType.rst
	enum_NOISE_MODEL.rst
	enum_NodeType.rst
	enum_OperatorType.rst
	enum_Operatortype.rst
	enum_QError.rst
	struct_Complex.rst
	struct_Mask.rst
	struct_QGateParam.rst
	struct_QubitVertice.rst
	class_CPUImplQPUSingleThread.rst
	class_CPUImplQPUSingleThreadWithOracle.rst
	class_CPUImplQPUWithOracle.rst
	class_ComplexTensor.rst
	class_Edge.rst
	class_Instructions.rst
	class_QuantumProgMap.rst
	class_TensorEngine.rst
	class_Vertice.rst
	class_VerticeMatrix.rst
	class_originirBaseVisitor.rst
	class_originirLexer.rst
	class_originirListener.rst
	class_originirParser.rst
	class_originirVisitor.rst
	class_qasmBaseVisitor.rst
	class_qasmLexer.rst
	class_qasmListener.rst
	class_qasmParser.rst
	class_qasmVisitor.rst

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// namespaces

	namespace :ref:`Base64<doxid-namespace_base64>`;
	namespace :ref:`GATEGPU<doxid-namespace_g_a_t_e_g_p_u>`;
	namespace :ref:`QGATE_SPACE<doxid-namespace_q_g_a_t_e___s_p_a_c_e>`;
	namespace :ref:`QPanda<doxid-namespace_q_panda>`;
		namespace :ref:`QPanda::Variational<doxid-namespace_q_panda_1_1_variational>`;
	namespace :ref:`gpu<doxid-namespacegpu>`;
	namespace :ref:`std<doxid-namespacestd>`;

	// typedefs

	typedef std::map<std::string, std::map<std::string, uint32_t>> :target:`config_map<doxid-instructions_8h_1a55d4d0d6f7920946e3cd55c30e9496ed>`;
	typedef float :target:`qstate_type<doxid-_q_panda_namespace_8h_1aa3be5ca16b07cae5d6e1b07151ed01c0>`;
	typedef std::complex<:ref:`qstate_type<doxid-_q_panda_namespace_8h_1aa3be5ca16b07cae5d6e1b07151ed01c0>`> :target:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`;
	typedef std::vector<:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`> :target:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`;
	typedef std::vector<size_t> :target:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`;
	typedef std::vector<double> :target:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`;
	typedef std::unordered_map<std::string, double> :target:`prob_map<doxid-_q_panda_namespace_8h_1a7f2845d06ff66a209709171dcb1f696a>`;
	typedef std::unordered_map<std::string, :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`> :target:`stat_map<doxid-_q_panda_namespace_8h_1a5b1ec78da541eaa2f329249b544e0488>`;
	typedef std::map<std::string, double> :target:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>`;
	typedef std::vector<std::pair<size_t, double>> :target:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>`;
	typedef wide_integer::generic_template::uint128_t :target:`uint128_t<doxid-_uinteger_8h_1ab23ac3d00ef1e3d7eb9211efd03de4b7>`;
	typedef wide_integer::generic_template::uint256_t :target:`uint256_t<doxid-_uinteger_8h_1a8cabad6c8ce9a9be1ae043b0fac95305>`;
	typedef wide_integer::generic_template::uint512_t :target:`uint512_t<doxid-_uinteger_8h_1a77bce31435304312e956325954e5b6d2>`;
	typedef size_t :target:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>`;
	typedef float :target:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`;
	typedef std::complex<:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`> :target:`gpu_qcomplex_t<doxid-_g_p_u_struct_8h_1a5427351e226a0fe5f3d9c29058252f43>`;
	typedef std::pair<size_t, double> :target:`gpu_pair<doxid-_g_p_u_struct_8h_1ae6cc32a10a2499f5e108ac025a33f197>`;
	typedef std::vector<:ref:`gpu_pair<doxid-_g_p_u_struct_8h_1ae6cc32a10a2499f5e108ac025a33f197>`> :target:`touple_prob<doxid-_g_p_u_struct_8h_1a6f3c3b9b86a1c5f31c541051760b64fe>`;
	typedef std::vector<double> :target:`vec_prob<doxid-_g_p_u_struct_8h_1a9e7ff63ce19e8c10cc6912f1bbe27d6e>`;
	typedef std::vector<:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>`> :target:`Qnum<doxid-_g_p_u_struct_8h_1a30f8cb6d9e512132464141bcc6f313fd>`;

	typedef bool (*:target:`noise_mode_function<doxid-_noise_model_8h_1a23eefdad48b57ed970997f0938dcc4e3>`)(
		rapidjson::Value &,
		NoiseOp &
		);

	typedef std::vector<:ref:`QGateParam<doxid-struct_q_gate_param>`> :target:`vQParam<doxid-_q_p_u_impl_8h_1a902a178b3747917bdcc89bca8c9ccda5>`;
	typedef struct :ref:`QubitVertice<doxid-struct_qubit_vertice>` :target:`qubit_vertice_t<doxid-_tensor_engine_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`;
	typedef float :target:`qdata_t<doxid-_tensor_node_8h_1a32cbdf9f66e36c2fc6b54cf9e32230d3>`;
	typedef size_t :target:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`;
	typedef complex<:ref:`qdata_t<doxid-_tensor_node_8h_1a32cbdf9f66e36c2fc6b54cf9e32230d3>`> :target:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>`;
	typedef vector<:ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>`> :target:`qstate_t<doxid-_tensor_node_8h_1a3d31874fe5c5e054c8c3eb07f19aa84b>`;
	typedef vector<pair<:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`>> :target:`qubit_vector_t<doxid-_tensor_node_8h_1aac19cd0cea4e3958f3c9339902f4addc>`;
	typedef map<size_t, :ref:`Edge<doxid-class_edge>`> :target:`EdgeMap<doxid-_tensor_node_8h_1a6ae5033ce14f4186e6c7063d177d75e2>`;
	typedef struct :ref:`Mask<doxid-struct_mask>` :target:`mask_t<doxid-_tensor_node_8h_1a45eead51aadff750a958300659ff7afe>`;
	typedef map<:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`Vertice<doxid-class_vertice>`> :target:`vertice_map_t<doxid-_tensor_node_8h_1a33eef85cb234c4824d5e7d3052896e2c>`;
	typedef vector<:ref:`vertice_map_t<doxid-_tensor_node_8h_1a33eef85cb234c4824d5e7d3052896e2c>`> :target:`vertice_matrix_t<doxid-_tensor_node_8h_1a703ff574c41e601bbe50f48ee42ecd8b>`;

	// enums

	enum :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`;
	enum :ref:`MetadataGateType<doxid-_q_global_variable_8h_1a9a37c80c5a19aef6f365af1f5dc1f766>`;
	enum :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`;
	enum :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`;
	enum :ref:`OperatorType<doxid-_q_global_variable_8h_1a6a02b2d1d62293b20242e3dcfbdd0117>`;
	enum :ref:`Operatortype<doxid-_q_global_variable_8h_1aac90bf8209b1a1a01eb17974a1311649>`;
	enum :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>`;

	// structs

	struct :ref:`Complex<doxid-struct_complex>`;
	struct :ref:`Mask<doxid-struct_mask>`;
	struct :ref:`QGateParam<doxid-struct_q_gate_param>`;
	struct :ref:`QubitVertice<doxid-struct_qubit_vertice>`;

	// classes

	class :ref:`AbstractDistributedFullAmplitudeEngine<doxid-class_abstract_distributed_full_amplitude_engine>`;
	class :ref:`AbstractQuantumGates<doxid-class_abstract_quantum_gates>`;
	class :ref:`CPUImplQPU<doxid-class_c_p_u_impl_q_p_u>`;
	class :ref:`CPUImplQPUSingleThread<doxid-class_c_p_u_impl_q_p_u_single_thread>`;
	class :ref:`CPUImplQPUSingleThreadWithOracle<doxid-class_c_p_u_impl_q_p_u_single_thread_with_oracle>`;
	class :ref:`CPUImplQPUWithOracle<doxid-class_c_p_u_impl_q_p_u_with_oracle>`;
	class :ref:`ComplexTensor<doxid-class_complex_tensor>`;
	class :ref:`DefaultRandomEngine<doxid-class_default_random_engine>`;
	class :ref:`DeleteUnitQnode<doxid-class_delete_unit_qnode>`;
	class :ref:`DistributedFullAmplitudeEngine<doxid-class_distributed_full_amplitude_engine>`;
	class :ref:`DoubleGateNoiseModeMap<doxid-class_double_gate_noise_mode_map>`;
	class :ref:`Edge<doxid-class_edge>`;
	class :ref:`Instructions<doxid-class_instructions>`;
	class :ref:`NoisyCPUImplQPU<doxid-class_noisy_c_p_u_impl_q_p_u>`;
	class :ref:`QPUImpl<doxid-class_q_p_u_impl>`;
	class :ref:`QuantumProgMap<doxid-class_quantum_prog_map>`;
	class :ref:`RandomEngine<doxid-class_random_engine>`;
	class :ref:`ReadLock<doxid-class_read_lock>`;
	class :ref:`SharedMutex<doxid-class_shared_mutex>`;
	class :ref:`SingleGateNoiseModeMap<doxid-class_single_gate_noise_mode_map>`;
	class :ref:`TensorEngine<doxid-class_tensor_engine>`;
	class :ref:`Vertice<doxid-class_vertice>`;
	class :ref:`VerticeMatrix<doxid-class_vertice_matrix>`;
	class :ref:`WriteLock<doxid-class_write_lock>`;
	class :ref:`XC_RandomEngine16807<doxid-class_x_c___random_engine16807>`;
	class :ref:`originirBaseVisitor<doxid-classoriginir_base_visitor>`;
	class :ref:`originirLexer<doxid-classoriginir_lexer>`;
	class :ref:`originirListener<doxid-classoriginir_listener>`;
	class :ref:`originirParser<doxid-classoriginir_parser>`;
	class :ref:`originirVisitor<doxid-classoriginir_visitor>`;
	class :ref:`qasmBaseVisitor<doxid-classqasm_base_visitor>`;
	class :ref:`qasmLexer<doxid-classqasm_lexer>`;
	class :ref:`qasmListener<doxid-classqasm_listener>`;
	class :ref:`qasmParser<doxid-classqasm_parser>`;
	class :ref:`qasmVisitor<doxid-classqasm_visitor>`;

	// global variables

	const :ref:`qstate_type<doxid-_q_panda_namespace_8h_1aa3be5ca16b07cae5d6e1b07151ed01c0>` :ref:`PI<doxid-_q_global_variable_8h_1a4d5c20a533e37f77b0bcc6c5eb160b09>`;
	constexpr :ref:`qstate_type<doxid-_q_panda_namespace_8h_1aa3be5ca16b07cae5d6e1b07151ed01c0>` :target:`SQRT2<doxid-_q_global_variable_8h_1aa72a9c39cd34ac99b237647f7795f856>`;
	const :ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` :target:`kThreadDim<doxid-_g_p_u_struct_8h_1aeef7ee927cfb0dc21622a8e9c1fc9738>`;

	// global functions

	uint32_t :target:`LOAD<doxid-instructions_8h_1a946e393ea315fdb831b240fbe83fa557>`(
		uint32_t rs1,
		uint32_t rd,
		uint32_t imm
		);

	uint32_t :target:`STORE<doxid-instructions_8h_1ac28df6a68ded267477d4132d2cd9f05d>`(
		uint32_t rs1,
		uint32_t rd,
		uint32_t imm
		);

	uint32_t :target:`BEQ<doxid-instructions_8h_1a0cbd6349d5dac94ff14ed9e9d82576dc>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t imm
		);

	uint32_t :target:`BNE<doxid-instructions_8h_1a89a9a4d1e23c43e895cdd1a6effa3d09>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t imm
		);

	uint32_t :target:`BLT<doxid-instructions_8h_1a378861027bb729421056867f1c299b73>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t imm
		);

	uint32_t :target:`BGT<doxid-instructions_8h_1a556b5fe4555748c7a2299e9c0d2e9193>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t imm
		);

	uint32_t :target:`ADDI<doxid-instructions_8h_1a2d1d8ba34b07b373baa82615b6a4c441>`(
		uint32_t rs1,
		uint32_t rd,
		uint32_t imm
		);

	uint32_t :target:`ANDI<doxid-instructions_8h_1a45f4fc920771da440dead9f35441a7c2>`(
		uint32_t rs1,
		uint32_t rd,
		uint32_t imm
		);

	uint32_t :target:`XORI<doxid-instructions_8h_1a08f2126eccc746c4c4540d63359efdb5>`(
		uint32_t rs1,
		uint32_t rd,
		uint32_t imm
		);

	uint32_t :target:`ORI<doxid-instructions_8h_1a778d3b2ec90d976b55ce1fdcf3043bb2>`(
		uint32_t rs1,
		uint32_t rd,
		uint32_t imm
		);

	uint32_t :target:`ADD<doxid-instructions_8h_1a6ff5921cc2507fa25640f8a7dc1bb64f>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t rd
		);

	uint32_t :target:`AND<doxid-instructions_8h_1a272ba9aa1dbbda7d9a658356479e67eb>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t rd
		);

	uint32_t :target:`XOR<doxid-instructions_8h_1a33a5f1c049b44e3e8621569e75e53291>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t rd
		);

	uint32_t :target:`OR<doxid-instructions_8h_1a7ab1895f7c583461b916a7083ddc6157>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t rd
		);

	uint32_t :target:`QWAITI<doxid-instructions_8h_1a4ed374dcc9de20b8770194313ed5cd19>`(uint32_t imm);

	uint32_t :target:`FMR<doxid-instructions_8h_1a105fdd0468f7014b7e2f9f32793d097e>`(
		uint32_t rs1,
		uint32_t rd
		);

	uint32_t :target:`SMIS<doxid-instructions_8h_1a611e10775c55aab00a0c5ecb05cea8e7>`(
		uint32_t rd,
		uint32_t imm
		);

	uint32_t :target:`QI<doxid-instructions_8h_1a5fd2ccef133e01a6bc8a7ef2e770abd8>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t PI,
		uint32_t opcode1,
		uint32_t opcode2
		);

	uint32_t :target:`MEASURE<doxid-instructions_8h_1a849b8d8675111092e9c9195b2b3b7aab>`(
		uint32_t rs1,
		uint32_t PI
		);

	template <typename UnsignedIntegralType>
	std::string :ref:`integerToBinary<doxid-group___utilities_1gaa65528bba400afbe3456b569805c1275>`(
		const UnsignedIntegralType& number,
		int ret_len
		);

	template <typename UnsignedIntegralType>
	std::string :ref:`integerToString<doxid-group___utilities_1ga674c5935aa6e6b7f5fc63dab3b4376c2>`(const UnsignedIntegralType& number);

	template <typename UnsignedIntegralType>
	UnsignedIntegralType :ref:`getDecIndex<doxid-group___utilities_1gae427c07ca7652b1f831ccf1eda056393>`(
		const UnsignedIntegralType& num1,
		const UnsignedIntegralType& num2,
		std::vector<size_t> qvec,
		size_t len
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`matrix_multiply<doxid-_noise_c_p_u_impl_q_p_u_8h_1a088032038179110cd9540ccf2f6cfc3d>`(
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`matrix_tensor<doxid-_noise_model_8h_1a82f07f65d8f7b9d6814d9c8126cd4b5d>`(
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	bool :target:`damping_kraus_operator<doxid-_noise_model_8h_1afe0044f9b1b74dd7808c59337cd8f8da>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`dephasing_kraus_operator<doxid-_noise_model_8h_1a95f9961f2457b7a4d4baf4cdc1de1060>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`decoherence_kraus_operator<doxid-_noise_model_8h_1a10a56d0f95c5578dc8d902fbcef62786>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`double_damping_kraus_operator<doxid-_noise_model_8h_1aff1403e30ab6821043c2d6df250b8123>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`double_decoherence_kraus_operator<doxid-_noise_model_8h_1a01c1af1dcffaae3f34653baaa262f7fe>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`pauli_kraus_map<doxid-_noise_model_8h_1a045504bffe3877a5c8694bfee128431d>`(
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`decoherence_kraus_operator_p1_p2<doxid-_noise_model_8h_1aa96b30941223d1d9541e5037b8d1c851>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`bitflip_kraus_operator<doxid-_noise_model_8h_1a949bfb1ad80a62d5a40071fec9128103>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`depolarizing_kraus_operator<doxid-_noise_model_8h_1aa354ecc773d9eba253b55c89dbe3eba1>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :ref:`bit_phase_flip_operator<doxid-group___virtual_quantum_processor_1ga387b0f99344a6794da969d23de3a96b0>` (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);
	bool :ref:`phase_damping_oprator<doxid-group___virtual_quantum_processor_1gaec6e538178b20f1f902fcdf30ff9062d>`(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);

	bool :target:`double_decoherence_kraus_operator_p1_p2<doxid-_noise_model_8h_1aab737c8bea9726b06445a821c4a20dd7>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`double_bitflip_kraus_operator<doxid-_noise_model_8h_1abfa9d8790dddfa552432d775c86d2600>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :target:`double_depolarizing_kraus_operator<doxid-_noise_model_8h_1ae395fd30ea36d7174f721b8836813033>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise
		);

	bool :ref:`double_bit_phase_flip_operator<doxid-group___virtual_quantum_processor_1gacc4ff7b27f520f6fb21a41c8848cdc0d>` (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);
	bool :ref:`double_phase_damping_oprator<doxid-group___virtual_quantum_processor_1gaef3f3a9f7026dc7a790cb2e58448b5ae>`(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);
	double :target:`_default_random_generator<doxid-_random_engine_8h_1a76645e3b89b68e020526bda5352f3d54>`();

	void :target:`H_Gate<doxid-_quantum_gates_8h_1aa2489b5d134df7872855d13f7d6a611b>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`T_Gate<doxid-_quantum_gates_8h_1a00a9bab6481253fa716ead78826b04b0>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`S_Gate<doxid-_quantum_gates_8h_1a003f0e919c714c44ea97bee11c7704f9>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`X_Gate<doxid-_quantum_gates_8h_1ae0af9fc3819b2a80d9cfd8f2c3feb1aa>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`Y_Gate<doxid-_quantum_gates_8h_1a2e90077ce27d7a305a7d6272562d3554>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`Z_Gate<doxid-_quantum_gates_8h_1ae21a01e14b9df50ef2ca962becd2fad6>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`X1_Gate<doxid-_quantum_gates_8h_1abf8db03f82133ef2fcd5375669635dae>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`Y1_Gate<doxid-_quantum_gates_8h_1ad65af61d7ca7b8bbe0fc06645a6856b2>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`Z1_Gate<doxid-_quantum_gates_8h_1a7241d7f6c5ffe6dc3f0fb3c4c7e8a657>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		bool isDagger
		);

	void :target:`RX_Gate<doxid-_quantum_gates_8h_1aeece20df36dbaf6543fefa2d4744d452>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		double angle,
		bool isDagger
		);

	void :target:`RY_Gate<doxid-_quantum_gates_8h_1ac2423237f629cd0457109eeecbc36ebb>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		double angle,
		bool isDagger
		);

	void :target:`RZ_Gate<doxid-_quantum_gates_8h_1a8f284c8d0faa3c31fe03a7216fea4d69>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		double angle,
		bool isDagger
		);

	void :target:`U1_Gate<doxid-_quantum_gates_8h_1ae5100ec58eae1530b2221cfd30e51b1e>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
		double angle,
		bool isDagger
		);

	void :target:`CZ_Gate<doxid-_quantum_gates_8h_1a3d14d72be930f8ef7383ee4f37a270dc>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit1,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit2,
		bool isDagger
		);

	void :target:`CNOT_Gate<doxid-_quantum_gates_8h_1a5334ec0fd6f5b533104ea467113d9d89>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit1,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit2,
		bool isDagger
		);

	void :target:`ISWAP_Gate<doxid-_quantum_gates_8h_1a04a92bb7ebf5d9c9dc585066760664dc>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit1,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit2,
		bool isDagger
		);

	void :target:`SQISWAP_Gate<doxid-_quantum_gates_8h_1ac2d31ad36879d2136d8335ae071e7c14>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit1,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit2,
		bool isDagger
		);

	void :target:`CR_Gate<doxid-_quantum_gates_8h_1adfb315958b79d31bc0a9f8e156579f98>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit1,
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit2,
		double angle,
		bool isDagger
		);

	void :target:`split<doxid-_tensor_engine_8h_1a40a2cf9355b1284cd2b82881bef276dd>`(
		:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`* prog_map,
		:ref:`qubit_vertice_t<doxid-_tensor_engine_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`* qubit_vertice,
		:ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>`* result
		);

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* :ref:`initialize<doxid-_chemi_q_i_f_c_8h_1a54f4eda15dd20e82919fcc100fb101b1>`(char* dir);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`finalize<doxid-_chemi_q_i_f_c_8h_1a35c742ebb04759d05160c183573ab4bb>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setMolecule<doxid-_chemi_q_i_f_c_8h_1aff908db723c06f88faaaef4d80526cab>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecule);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setMolecules<doxid-_chemi_q_i_f_c_8h_1a62cbe512973d55ce78d1098c69f651b8>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecules);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setMultiplicity<doxid-_chemi_q_i_f_c_8h_1afa4616781c758abdd0e310cc583cc306>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int multiplicity);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setCharge<doxid-_chemi_q_i_f_c_8h_1a0937e49cf4c0ac3e114c6c2c449bfe40>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int charge);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setBasis<doxid-_chemi_q_i_f_c_8h_1a39356f40f231e4533f6225413d8b3901>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* basis);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setTransformType<doxid-_chemi_q_i_f_c_8h_1a57571abf529d58ef4d197eb838a0df97>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setUccType<doxid-_chemi_q_i_f_c_8h_1a345009bff8bc327845abc1717c1714a3>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setOptimizerType<doxid-_chemi_q_i_f_c_8h_1a05337011ecbc3cdaec08d1b03cecfd47>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setOptimizerIterNum<doxid-_chemi_q_i_f_c_8h_1ad864b5c29eacb4a7c6254a7ef20e0cb6>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setOptimizerFuncCallNum<doxid-_chemi_q_i_f_c_8h_1a561c06e5f054902e7cb65a8b242090f8>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setOptimizerXatol<doxid-_chemi_q_i_f_c_8h_1aae3ec08bfa9031ff5a3aee9eebdc1875>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setOptimizerFatol<doxid-_chemi_q_i_f_c_8h_1a2c60296f22a5c3d2b79b194cfc75a2d8>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setLearningRate<doxid-_chemi_q_i_f_c_8h_1aa45474eef8eb830b36ff62efab13f60a>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setEvolutionTime<doxid-_chemi_q_i_f_c_8h_1adb9bce782572809474d8bfb805209336>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setHamiltonianSimulationSlices<doxid-_chemi_q_i_f_c_8h_1a7d5ccdc7d940147460c495a566c85627>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void :ref:`setSaveDataDir<doxid-_chemi_q_i_f_c_8h_1ab3e2454f231223067408305835b4105d>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* dir);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` bool :ref:`exec<doxid-_chemi_q_i_f_c_8h_1a76ea93400681d101a95281b713f55211>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq);

	// macros

	#define :target:`CONFIG_PATH<doxid-_x_m_l_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`
	#define :target:`CONST_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a18005d49ae00702328d036fc06855285>`(NAME)
	#define :target:`CONTROL_CONST_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a6d0815a9698bafe7f2d1687e3287ae16>`(NAME)
	#define :target:`CONTROL_SINGLE_ANGLE_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a68f818200ac956e8ccee01f59d6c3e49>`(NAME)
	#define :target:`DECL_ANGLE_GATE_MATRIX<doxid-_c_p_u_impl_q_p_u_8h_1ad412042fda449c86a58d4be0c1bdb968>`(NAME)
	#define :target:`DECL_GATE_MATRIX<doxid-_c_p_u_impl_q_p_u_8h_1a52269caa683e0718f0d36d007952c9d8>`(NAME)
	#define :target:`DEF_EVALUATIONS<doxid-_data_struct_8h_1a286a563a032a1f9f515bcb1a5184cbf1>`
	#define :target:`DEF_ITERATIONS<doxid-_data_struct_8h_1a50f8a0cd81ff8db643ee8695677f7f4a>`
	#define :target:`DEF_KEY<doxid-_data_struct_8h_1a5cc4c4a7a1567c960d293509236ff415>`
	#define :target:`DEF_MESSAGE<doxid-_data_struct_8h_1a024abd075c62ffea7afebc77aff37f39>`
	#define :target:`DEF_OPTI_STATUS_CALCULATING<doxid-_data_struct_8h_1ad12b051fc919de28fe3d92a42d057ad5>`
	#define :target:`DEF_OPTI_STATUS_MAX_FEV<doxid-_data_struct_8h_1a24e823761c2dd3ffe7b861378d239d3e>`
	#define :target:`DEF_OPTI_STATUS_MAX_ITER<doxid-_data_struct_8h_1a41bb871714391ec14163c891161ba288>`
	#define :target:`DEF_OPTI_STATUS_PARA_ERROR<doxid-_data_struct_8h_1ab6523b6826b88c6e46bd1c899d8dda26>`
	#define :target:`DEF_OPTI_STATUS_SUCCESS<doxid-_data_struct_8h_1aa391b63c60fad305c422476bfe3cf3f3>`
	#define :target:`DEF_UNINIT_FLOAT<doxid-_data_struct_8h_1ab6d4111b534900bc248363f235c23787>`
	#define :target:`DEF_UNINIT_INT<doxid-_data_struct_8h_1ad70c5e9d9df24752e23b160a9e7f69d3>`
	#define :target:`DEF_VALUE<doxid-_data_struct_8h_1a3d2399018cea5da40b50cb6ac9c99600>`
	#define :target:`DEF_WARING<doxid-_data_struct_8h_1af8d6490745b3eeee37db778adddfc26d>`
	#define :target:`DoubleGateMatrixSize<doxid-_transform_decomposition_8h_1a786eca5682d042d2a5a9d8c3e967213e>`
	#define :target:`IBMQ_BACKENDS_CONFIG<doxid-_i_b_m_q_8h_1a983c90909c7f80e717ea9ea1add1d150>`
	#define :target:`IBMQ_BACKENDS_CONFIG_FILE<doxid-_i_b_m_q_8h_1ad611e840c8fc3ed51fd84402f436aaad>`
	#define :target:`MACRO_GET_GATETYPE<doxid-_origin_i_r_to_q_prog_8h_1a9d1e3b75ddfa6d98b095382065226e85>`(name)
	#define :target:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`
	#define :target:`NoiseOp<doxid-_noise_c_p_u_impl_q_p_u_8h_1ad01e905fa484518e596588e907885a21>`
	#define :target:`PI<doxid-_c_p_u_impl_q_p_u_single_thread_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :target:`PI<doxid-_noise_c_p_u_impl_q_p_u_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :target:`PI<doxid-_c_p_u_impl_q_p_u_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :ref:`QCERR<doxid-_q_panda_namespace_8h_1acb29825331db5ae6632fbb0647a72534>`(x)

	#define :ref:`QCERR_AND_THROW_ERRSTR<doxid-_q_panda_namespace_8h_1aac47299986cc9e801758ad7946bea4b2>`( \
		std_exception, \
		x \
		)

	#define :target:`QIF_REGISTER<doxid-_control_flow_8h_1a35a941193ad6c93151abfcef3528b3d9>`(className)
	#define :target:`QPANDA_BEGIN<doxid-_q_panda_namespace_8h_1a375c0f5e0d6568b83528815afc55ff80>`
	#define :target:`QPANDA_END<doxid-_q_panda_namespace_8h_1a9d806bab2e1c7ce92bcacc6b92a9bc56>`
	#define :target:`QWHILE_REGISTER<doxid-_control_flow_8h_1a2e7197bd17e1381a1b7d3543c885c833>`(className)
	#define :target:`Q_CONTROL_GATE_TIME_SEQUENCE<doxid-_x_m_l_config_param_8h_1a18c981104367d54320e94f028309eaae>`
	#define :target:`Q_GATE_TIME_SEQUENCE_CONFIG<doxid-_x_m_l_config_param_8h_1ae73d10cbfe7c6a9b3fababc0e5fbef6a>`
	#define :target:`Q_MEASURE_TIME_SEQUENCE<doxid-_x_m_l_config_param_8h_1a524976054d08f0464a66332520d8037d>`
	#define :ref:`Q_PI<doxid-_data_struct_8h_1a473347ab5d3559b4e38772c222e0de5f>`
	#define :ref:`Q_PI_2<doxid-_data_struct_8h_1a7b39aafc1ce98f1f7fafe38a6c7ebebc>`
	#define :target:`Q_RESET_TIME_SEQUENCE<doxid-_x_m_l_config_param_8h_1a6aa7cca90e5227875cc89c1471c4665a>`
	#define :target:`Q_SINGLE_GATE_TIME_SEQUENCE<doxid-_x_m_l_config_param_8h_1a33b35706116c3e2aacdd31e8926323a5>`
	#define :target:`Q_SWAP_TIME_SEQUENCE<doxid-_x_m_l_config_param_8h_1a08804783a864da578727d960277e8c2f>`

	#define :target:`REGISTER_ANGLE_GATE_MATRIX<doxid-_c_p_u_impl_q_p_u_8h_1a687b351bc98ff94af7e6dbe8e2330cab>`( \
		NAME, \
		Nx, \
		Ny, \
		Nz \
		)

	#define :target:`REGISTER_CBIT_NAME_<doxid-_c_bit_factory_8h_1a525e2032447e839948cf7e4e58036a1d>`(classname)
	#define :target:`REGISTER_CEXPR<doxid-_c_expr_factory_8h_1ac10412947dd322dd48a27281c2c905e4>`(classname)
	#define :target:`REGISTER_CLASSICAL_PROGRAM<doxid-_classical_program_8h_1a63cb828b756b7fecd311bb7bf9a7e7f4>`(className)
	#define :target:`REGISTER_CMEM_SIZE_<doxid-_c_mem_factory_8h_1a4242abc25a0eb7e62744e7e57f3ef2ca>`(classname)

	#define :target:`REGISTER_GATE_MATRIX<doxid-_c_p_u_impl_q_p_u_8h_1ad5f4a3bb046db093ac0a53ce2e4c32f9>`( \
		NAME, \
		U00, \
		U01, \
		U10, \
		U11 \
		)

	#define :target:`REGISTER_MEASURE<doxid-_quantum_measure_8h_1ae544a6292807422a6aa83bb4590bea80>`(className)
	#define :target:`REGISTER_PHYSICAL_QUBIT<doxid-_physical_qubit_factory_8h_1ac0fd399f03c12f868397e773537ce30b>`(classname)
	#define :target:`REGISTER_QCIRCUIT<doxid-_q_circuit_8h_1a3e42ff079ec9d8a23f0918a0beb54f17>`(className)
	#define :target:`REGISTER_QPROGRAM<doxid-_q_program_8h_1a10351e486d0664cd0074c0256e23821a>`(className)
	#define :target:`REGISTER_QRES_NAME<doxid-_q_result_factory_8h_1aa32a38eda5b34a5784c80f3fb5e8b2f3>`(classname)
	#define :target:`REGISTER_QUANTUM_MACHINE<doxid-_quantum_machine_factory_8h_1af337fede31e3237363c0a93ae25d4ec1>`(classname)
	#define :target:`REGISTER_QUBIT<doxid-_qubit_factory_8h_1a48daedf3982e615fafd5b51904200304>`(classname)
	#define :target:`REGISTER_QUBIT_POOL_SIZE_<doxid-_qubit_pool_factory_8h_1abefada4c93076db141865fe08b110e39>`(classname)
	#define :target:`REGISTER_RESET<doxid-_q_reset_8h_1a77a508fb5edb4fac1e164e89cf1ade0b>`(className)
	#define :target:`SINGLETON_DECLARE<doxid-macro_8h_1a86a90fab08d07cd727c94da9594a1de2>`(Type)
	#define :target:`SINGLETON_IMPLEMENT_EAGER<doxid-macro_8h_1add8c8d20b359e4be7a7451fa1052db63>`(Type)
	#define :target:`SINGLETON_IMPLEMENT_LAZY<doxid-macro_8h_1ad5ff7948e947124a9de03a299399cffd>`(Type)
	#define :target:`SINGLE_ANGLE_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a3ba9b536f4f4be4ddb39870acb88f43a>`(NAME)
	#define :target:`SQ2<doxid-_c_p_u_impl_q_p_u_8h_1a0b19f406e0cc4cbaf7a935f155567869>`
	#define :target:`SQ2<doxid-_c_p_u_impl_q_p_u_single_thread_8h_1a0b19f406e0cc4cbaf7a935f155567869>`
	#define :target:`SQ2<doxid-_noise_c_p_u_impl_q_p_u_8h_1a0b19f406e0cc4cbaf7a935f155567869>`
	#define :target:`SingleGateMatrixSize<doxid-_transform_decomposition_8h_1a5cc35d85fd0872be5f41ffd4c971f52c>`
	#define :target:`USING_QPANDA<doxid-_q_panda_namespace_8h_1af7466c9c1ed8b95983912dd5449b75f4>`
	#define :target:`ZeroJudgement<doxid-_transform_decomposition_8h_1ae5cd83615b00885b469014317591e8d8>`
	#define :target:`_DOUBLE_ANGLE_GATE<doxid-_partial_amplitude_graph_8h_1ac4ac74220876e7668927a747d8c4c385>`(NAME)
	#define :target:`_DOUBLE_GATE<doxid-_partial_amplitude_graph_8h_1a25aa5fb0f107d2c3e3b9c6851251e880>`(NAME)
	#define :target:`_SINGLE_ANGLE_GATE<doxid-_partial_amplitude_graph_8h_1ab04bb57d9d2c1c3ad8b126dd3db64bdc>`(NAME)
	#define :target:`_SINGLE_GATE<doxid-_partial_amplitude_graph_8h_1abd4b56edaa9b31f023d2a10e7d66cb62>`(NAME)
	#define :target:`_TRIPLE_GATE<doxid-_partial_amplitude_graph_8h_1a8cbc0d2696af3e70b30079778246f130>`(NAME)

	#define :target:`const_single_qubit_gate<doxid-_c_p_u_impl_q_p_u_8h_1ad852122396459f511d981c1b0cc8c570>`( \
		GATE_NAME, \
		qn, \
		isConjugate, \
		error_rate \
		)

	#define :target:`control_const_single_qubit_gate<doxid-_c_p_u_impl_q_p_u_8h_1a7388a268e200122bfff00ebbd313a78e>`( \
		GATE_NAME, \
		qn, \
		vControlBit, \
		isConjugate, \
		error_rate \
		)

	#define :target:`control_single_qubit_angle_gate<doxid-_c_p_u_impl_q_p_u_8h_1ac9fa7b2e86c6d084cb527a2838c98018>`( \
		GATE_NAME, \
		qn, \
		theta, \
		vControlBit, \
		isConjugate, \
		error_rate \
		)

	#define :target:`iunit<doxid-_quantum_gate_parameter_8h_1ac1aec01c10b9205cebf2e8efd8e1e029>`

	#define :target:`single_qubit_angle_gate<doxid-_c_p_u_impl_q_p_u_8h_1a3ac2db895d08fa984afb344692cc5b20>`( \
		GATE_NAME, \
		qn, \
		theta, \
		isConjugate, \
		error_rate \
		)

.. _details-global:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Variables
----------------

.. index:: pair: variable; PI
.. _doxid-_q_global_variable_8h_1a4d5c20a533e37f77b0bcc6c5eb160b09:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`qstate_type<doxid-_q_panda_namespace_8h_1aa3be5ca16b07cae5d6e1b07151ed01c0>` PI

Square root of two

Global Functions
----------------

.. index:: pair: function; initialize
.. _doxid-_chemi_q_i_f_c_8h_1a54f4eda15dd20e82919fcc100fb101b1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* initialize(char* dir)

Initialize the quantum chemistry calculation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- The dir of the psi4 chemistry calculation package



.. rubric:: Returns:

ChemiQ\* a ChemiQ object ptr

.. index:: pair: function; finalize
.. _doxid-_chemi_q_i_f_c_8h_1a35c742ebb04759d05160c183573ab4bb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void finalize(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq)

Finalize the quantum chemistry calculation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the ChemiQ object ptr will be finalized

.. index:: pair: function; setMolecule
.. _doxid-_chemi_q_i_f_c_8h_1aff908db723c06f88faaaef4d80526cab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setMolecule(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecule)

Set the molecular model to calculate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- std::string

		- molecule model

.. index:: pair: function; setMolecules
.. _doxid-_chemi_q_i_f_c_8h_1a62cbe512973d55ce78d1098c69f651b8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setMolecules(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecules)

Set the molecular model to calculate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- char\*

		- the molecules ptr

.. index:: pair: function; setMultiplicity
.. _doxid-_chemi_q_i_f_c_8h_1afa4616781c758abdd0e310cc583cc306:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setMultiplicity(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int multiplicity)

Set the multiplicity of the molecular model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- int

		- multiplicity

.. index:: pair: function; setCharge
.. _doxid-_chemi_q_i_f_c_8h_1a0937e49cf4c0ac3e114c6c2c449bfe40:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setCharge(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int charge)

Set the charge of the molecular model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- int

		- charge

.. index:: pair: function; setBasis
.. _doxid-_chemi_q_i_f_c_8h_1a39356f40f231e4533f6225413d8b3901:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setBasis(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* basis)

Set the calculation basis.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- std::string

		- basis

.. index:: pair: function; setTransformType
.. _doxid-_chemi_q_i_f_c_8h_1a57571abf529d58ef4d197eb838a0df97:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setTransformType(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type)

Set the transform type from Fermion operator to Pauli operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- int

		- transform type



.. rubric:: See also:

:ref:`QPanda::TransFormType <doxid-namespace_q_panda_1a5f9863b9f685c15e539744e808edde8b>`

.. index:: pair: function; setUccType
.. _doxid-_chemi_q_i_f_c_8h_1a345009bff8bc327845abc1717c1714a3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setUccType(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type)

Set the ucc type to contruct the Fermion operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- int

		- ucc type



.. rubric:: See also:

:ref:`QPanda::UccType <doxid-namespace_q_panda_1a7f68ed9ecff5c30e9105f9cf9ac259ba>`

.. index:: pair: function; setOptimizerType
.. _doxid-_chemi_q_i_f_c_8h_1a05337011ecbc3cdaec08d1b03cecfd47:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setOptimizerType(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type)

Set the optimizer type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- int

		- optimizer type



.. rubric:: See also:

:ref:`QPanda::OptimizerType <doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>`

.. index:: pair: function; setOptimizerIterNum
.. _doxid-_chemi_q_i_f_c_8h_1ad864b5c29eacb4a7c6254a7ef20e0cb6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setOptimizerIterNum(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value)

Set the optimizer iteration number.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- size_t

		- iteration number

.. index:: pair: function; setOptimizerFuncCallNum
.. _doxid-_chemi_q_i_f_c_8h_1a561c06e5f054902e7cb65a8b242090f8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setOptimizerFuncCallNum(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value)

Set the optimizer function callback number.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- size_t

		- function callback number

.. index:: pair: function; setOptimizerXatol
.. _doxid-_chemi_q_i_f_c_8h_1aae3ec08bfa9031ff5a3aee9eebdc1875:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setOptimizerXatol(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

Set the optimizer iteration number.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- size_t

		- iteration number

.. index:: pair: function; setOptimizerFatol
.. _doxid-_chemi_q_i_f_c_8h_1a2c60296f22a5c3d2b79b194cfc75a2d8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setOptimizerFatol(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

Set the optimizer fatol.It is the Absolute error in func(xopt) between iterations that is acceptable for convergence.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- double

		- absolute error between func(xopt)

.. index:: pair: function; setLearningRate
.. _doxid-_chemi_q_i_f_c_8h_1aa45474eef8eb830b36ff62efab13f60a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setLearningRate(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

Set the learing rate when using Gradient optimizer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- double

		- learing rate

.. index:: pair: function; setEvolutionTime
.. _doxid-_chemi_q_i_f_c_8h_1adb9bce782572809474d8bfb805209336:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setEvolutionTime(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

Set the evolution time when doing hamiltonian simulation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- double

		- evolution time

.. index:: pair: function; setHamiltonianSimulationSlices
.. _doxid-_chemi_q_i_f_c_8h_1a7d5ccdc7d940147460c495a566c85627:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setHamiltonianSimulationSlices(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value)

Set the hamiltonian simulation slices (e^iAt/n\*e^iBt/n)^n, n is the slices.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- double

		- hamiltonian simulation slices

.. index:: pair: function; setSaveDataDir
.. _doxid-_chemi_q_i_f_c_8h_1ab3e2454f231223067408305835b4105d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` void setSaveDataDir(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* dir)

Set the directory to save the calculated data. If it's a not exist dir data will not be saved.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- std::string

		- dir

.. index:: pair: function; exec
.. _doxid-_chemi_q_i_f_c_8h_1a76ea93400681d101a95281b713f55211:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` bool exec(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq)

exec molecule calculate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr



.. rubric:: Returns:

bool true:success; false:failed

Macros
------

.. index:: pair: define; QCERR
.. _doxid-_q_panda_namespace_8h_1acb29825331db5ae6632fbb0647a72534:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define QCERR(x)

QPanda2 cout error message.

.. index:: pair: define; QCERR_AND_THROW_ERRSTR
.. _doxid-_q_panda_namespace_8h_1aac47299986cc9e801758ad7946bea4b2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define QCERR_AND_THROW_ERRSTR(std_exception, x)

output the error string to standard error and throw a standard exception. A standard exception can be of the following types: runtime_error, invalid_argument, range_error, etc

.. index:: pair: define; Q_PI
.. _doxid-_data_struct_8h_1a473347ab5d3559b4e38772c222e0de5f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define Q_PI

pi

.. index:: pair: define; Q_PI_2
.. _doxid-_data_struct_8h_1a7b39aafc1ce98f1f7fafe38a6c7ebebc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	#define Q_PI_2

pi/2

