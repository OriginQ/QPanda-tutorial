.. _global:
.. index:: pair: namespace; global

Global Namespace
================

.. toctree::
	:hidden:

	namespace_Base64.rst
	namespace_Eigen.rst
	namespace_GATEGPU.rst
	namespace_QGATE_SPACE.rst
	namespace_QPanda.rst
	namespace_gpu.rst
	namespace_std.rst
	enum_ComputeBackend.rst
	enum_GateType.rst
	enum_MetadataGateType.rst
	enum_NOISE_MODEL.rst
	enum_NodeType.rst
	enum_OperatorType.rst
	enum_Operatortype.rst
	enum_QError.rst
	struct_Complex.rst
	struct_QGateParam.rst
	struct_QubitVertice.rst
	class_AbstractComplexTensor.rst
	class_CPUComplexTensor.rst
	class_CPUImplQPUSingleThread.rst
	class_CPUImplQPUSingleThreadWithOracle.rst
	class_CPUImplQPUWithOracle.rst
	class_ComplexTensor.rst
	class_Edge.rst
	class_Instructions.rst
	class_MPS_Tensor.rst
	class_MeasureQVMType.rst
	class_NoisyQuantum.rst
	class_QProgMap.rst
	class_QuantumError.rst
	class_QuickBB.rst
	class_RandomEngine19937.rst
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
	namespace :ref:`Eigen<doxid-namespace_eigen>`;
	namespace :ref:`GATEGPU<doxid-namespace_g_a_t_e_g_p_u>`;
	namespace :ref:`QGATE_SPACE<doxid-namespace_q_g_a_t_e___s_p_a_c_e>`;
	namespace :ref:`QPanda<doxid-namespace_q_panda>`;
		namespace :ref:`QPanda::DRAW_TEXT_PIC<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c>`;
		namespace :ref:`QPanda::Variational<doxid-namespace_q_panda_1_1_variational>`;
	namespace :ref:`gpu<doxid-namespacegpu>`;
	namespace :ref:`std<doxid-namespacestd>`;

	// typedefs

	typedef std::map<std::string, std::map<std::string, uint32_t>> :target:`config_map<doxid-instructions_8h_1a55d4d0d6f7920946e3cd55c30e9496ed>`;
	typedef double :target:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>`;
	typedef std::complex<:ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>`> :target:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`;
	typedef std::vector<:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`> :target:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`;
	typedef std::vector<size_t> :target:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`;
	typedef std::vector<double> :target:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`;
	typedef std::unordered_map<std::string, :ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>`> :target:`prob_map<doxid-_q_panda_namespace_8h_1a984c8c48bbaa623e633d6800bf7e2b55>`;
	typedef std::unordered_map<std::string, :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`> :target:`stat_map<doxid-_q_panda_namespace_8h_1a5b1ec78da541eaa2f329249b544e0488>`;
	typedef std::map<std::string, double> :target:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>`;
	typedef std::vector<std::pair<size_t, double>> :target:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>`;
	typedef std::shared_ptr<:ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`> :target:`QNodeRef<doxid-_qubit_mapping_8h_1a5cd44073de95edede4a142612af4ae41>`;
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
	typedef Eigen::Matrix<:ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>`, Eigen::Dynamic, 1> :target:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`;
	typedef Eigen::Matrix<:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`, Eigen::Dynamic, 1> :target:`cvector_t<doxid-_m_p_s_tensor_8h_1a7154a7c56ab0263fd556061c5a87a225>`;
	typedef Eigen::Matrix<:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor> :target:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`;
	typedef std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`> :target:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`;

	typedef bool (*:target:`noise_mode_function<doxid-_noise_model_8h_1a23eefdad48b57ed970997f0938dcc4e3>`)(
		rapidjson::Value &,
		NoiseOp &
		);

	typedef std::vector<:ref:`QGateParam<doxid-struct_q_gate_param>`> :target:`vQParam<doxid-_q_p_u_impl_8h_1a902a178b3747917bdcc89bca8c9ccda5>`;
	typedef size_t :target:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>`;
	typedef std::vector<:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>`> :target:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`;
	typedef std::map<:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>`, :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`> :target:`graph_data_t<doxid-_quick_b_b_8h_1a85d3dda5284997d6cf7a47d3aa359798>`;
	typedef float :target:`qdata_t<doxid-_tensor_8h_1a32cbdf9f66e36c2fc6b54cf9e32230d3>`;
	typedef size_t :target:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`;
	typedef std::complex<:ref:`qdata_t<doxid-_tensor_8h_1a32cbdf9f66e36c2fc6b54cf9e32230d3>`> :target:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`;
	typedef std::vector<:ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`> :target:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`;
	typedef std::vector<std::pair<size_t, bool>> :target:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`;
	typedef std::vector<std::pair<:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`>> :target:`qubit_vector_t<doxid-_tensor_node_8h_1af892fbee44ef3346256861d11383f4a1>`;
	typedef std::map<size_t, :ref:`Edge<doxid-class_edge>`> :target:`edge_map_t<doxid-_tensor_node_8h_1aa2ec0dbc2b2371ca27fda6883430e1d5>`;
	typedef std::map<:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`Vertice<doxid-class_vertice>`> :target:`vertice_map_t<doxid-_tensor_node_8h_1afc10359c1366160cefe2a9357c1a86b9>`;
	typedef std::vector<:ref:`vertice_map_t<doxid-_tensor_node_8h_1afc10359c1366160cefe2a9357c1a86b9>`> :target:`vertice_matrix_t<doxid-_tensor_node_8h_1a061ff6aeab93806ea04a98640129ede3>`;
	typedef struct :ref:`QubitVertice<doxid-struct_qubit_vertice>` :target:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`;

	// enums

	enum :ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>`;
	enum :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`;
	enum :ref:`MetadataGateType<doxid-_q_global_variable_8h_1a9a37c80c5a19aef6f365af1f5dc1f766>`;
	enum :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`;
	enum :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`;
	enum :ref:`OperatorType<doxid-_q_global_variable_8h_1a6a02b2d1d62293b20242e3dcfbdd0117>`;
	enum :ref:`Operatortype<doxid-_q_global_variable_8h_1aac90bf8209b1a1a01eb17974a1311649>`;
	enum :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>`;

	// structs

	struct :ref:`Complex<doxid-struct_complex>`;
	struct :ref:`QGateParam<doxid-struct_q_gate_param>`;
	struct :ref:`QubitVertice<doxid-struct_qubit_vertice>`;

	// classes

	class :ref:`AbstractComplexTensor<doxid-class_abstract_complex_tensor>`;
	class :ref:`AbstractDistributedFullAmplitudeEngine<doxid-class_abstract_distributed_full_amplitude_engine>`;
	class :ref:`AbstractQuantumGates<doxid-class_abstract_quantum_gates>`;
	class :ref:`CPUComplexTensor<doxid-class_c_p_u_complex_tensor>`;
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
	class :ref:`MPS_Tensor<doxid-class_m_p_s___tensor>`;
	class :ref:`MeasureQVMType<doxid-class_measure_q_v_m_type>`;
	class :ref:`NoisyCPUImplQPU<doxid-class_noisy_c_p_u_impl_q_p_u>`;
	class :ref:`NoisyQuantum<doxid-class_noisy_quantum>`;
	class :ref:`QPUImpl<doxid-class_q_p_u_impl>`;
	class :ref:`QProgMap<doxid-class_q_prog_map>`;
	class :ref:`QuantumError<doxid-class_quantum_error>`;
	class :ref:`QuickBB<doxid-class_quick_b_b>`;
	class :ref:`RandomEngine<doxid-class_random_engine>`;
	class :ref:`RandomEngine19937<doxid-class_random_engine19937>`;
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

	const :ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>` :ref:`PI<doxid-_q_global_variable_8h_1a4d5c20a533e37f77b0bcc6c5eb160b09>` = 3.14159265358979323846;
	constexpr :ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>` :target:`SQRT2<doxid-_q_global_variable_8h_1aa72a9c39cd34ac99b237647f7795f856>` = 1.4142135623731;
	const :ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` :target:`kThreadDim<doxid-_g_p_u_struct_8h_1aeef7ee927cfb0dc21622a8e9c1fc9738>` = 1024;

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

	uint32_t :target:`QI<doxid-instructions_8h_1aeb80d65149e5a389de36f4d66d70125d>`(
		uint32_t rs1,
		uint32_t rs2,
		uint32_t pi,
		uint32_t opcode1,
		uint32_t opcode2
		);

	uint32_t :target:`MEASURE<doxid-instructions_8h_1a8abbc52ba579bbc9c490a1d979bd6cb4>`(
		uint32_t rs1,
		uint32_t pi
		);

	std::string :target:`_file_name<doxid-_q_panda_namespace_8h_1a5ee6583e59e93d2276d25312f3503746>`(const char* file = "");

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

	bool :target:`equal<doxid-_noise_model_8h_1a2fcd3d51181ffa3697051397cd4a62bc>`(
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& lhs,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& rhs
		);

	bool :target:`damping_kraus_operator<doxid-_noise_model_8h_1afe0044f9b1b74dd7808c59337cd8f8da>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`dephasing_kraus_operator<doxid-_noise_model_8h_1a95f9961f2457b7a4d4baf4cdc1de1060>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`decoherence_kraus_operator<doxid-_noise_model_8h_1a10a56d0f95c5578dc8d902fbcef62786>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`double_damping_kraus_operator<doxid-_noise_model_8h_1aff1403e30ab6821043c2d6df250b8123>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`double_decoherence_kraus_operator<doxid-_noise_model_8h_1a01c1af1dcffaae3f34653baaa262f7fe>` (
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`pauli_kraus_map<doxid-_noise_model_8h_1a045504bffe3877a5c8694bfee128431d>`(
		rapidjson::Value&,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`decoherence_kraus_operator_p1_p2<doxid-_noise_model_8h_1aa96b30941223d1d9541e5037b8d1c851>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`bitflip_kraus_operator<doxid-_noise_model_8h_1a949bfb1ad80a62d5a40071fec9128103>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`depolarizing_kraus_operator<doxid-_noise_model_8h_1aa354ecc773d9eba253b55c89dbe3eba1>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :ref:`bit_phase_flip_operator<doxid-group___virtual_quantum_processor_1ga387b0f99344a6794da969d23de3a96b0>` (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise);
	bool :ref:`phase_damping_oprator<doxid-group___virtual_quantum_processor_1gaec6e538178b20f1f902fcdf30ff9062d>`(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise);

	bool :target:`double_decoherence_kraus_operator_p1_p2<doxid-_noise_model_8h_1aab737c8bea9726b06445a821c4a20dd7>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`double_bitflip_kraus_operator<doxid-_noise_model_8h_1abfa9d8790dddfa552432d775c86d2600>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :target:`double_depolarizing_kraus_operator<doxid-_noise_model_8h_1ae395fd30ea36d7174f721b8836813033>` (
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	bool :ref:`double_bit_phase_flip_operator<doxid-group___virtual_quantum_processor_1gacc4ff7b27f520f6fb21a41c8848cdc0d>` (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise);
	bool :ref:`double_phase_damping_oprator<doxid-group___virtual_quantum_processor_1gaef3f3a9f7026dc7a790cb2e58448b5ae>`(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise);

	bool :target:`kraus_matrix_oprator<doxid-_noise_model_8h_1a4565d2e7881ac7371bd88f355b171883>`(
		rapidjson::Value& value,
		:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise
		);

	double :target:`_default_random_generator<doxid-_random_engine_8h_1a76645e3b89b68e020526bda5352f3d54>`();

	double :target:`random_generator19937<doxid-_random_engine_8h_1a356389f609905c977c32e90691e1e443>`(
		double begine = 0,
		double end = 1
		);

	void :target:`H_Gate<doxid-_quantum_gates_8h_1a33f6afef750f382d1e8df8a851196780>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`T_Gate<doxid-_quantum_gates_8h_1a5f96175b2bb6a8ca8869e35c25eb990b>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`S_Gate<doxid-_quantum_gates_8h_1a7d0422e3b2635c753468283299298770>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`X_Gate<doxid-_quantum_gates_8h_1a309ee2fec720447bc542bfd31da19614>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`Y_Gate<doxid-_quantum_gates_8h_1aaa84cc245e73903282e35811044d59e6>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`Z_Gate<doxid-_quantum_gates_8h_1aa4444e1f7423598e4193c630edb16805>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`X1_Gate<doxid-_quantum_gates_8h_1aa544bc1fa8a9c8218d16d1dd08abc8ea>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`Y1_Gate<doxid-_quantum_gates_8h_1a78f69f80b413d120c4392b5e22828f69>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`Z1_Gate<doxid-_quantum_gates_8h_1a0a13b92011644012b4fbb9e551d303d1>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`RX_Gate<doxid-_quantum_gates_8h_1a7ab9109e48d22b86cabfc2e45520a141>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double angle,
		bool isDagger
		);

	void :target:`RY_Gate<doxid-_quantum_gates_8h_1a7dc2c46a8e176530b17eb14eedc95f34>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double angle,
		bool isDagger
		);

	void :target:`RZ_Gate<doxid-_quantum_gates_8h_1a975b311aecb9aebf80b25e068013c727>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double angle,
		bool isDagger
		);

	void :target:`U1_Gate<doxid-_quantum_gates_8h_1aecff3cfe7855df698fb02f96b7f197a9>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double angle,
		bool isDagger
		);

	void :target:`U2_Gate<doxid-_quantum_gates_8h_1ad1e6a8aab3b6ce22d1f31abba65e7dd4>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double phi,
		double lambda,
		bool isDagger
		);

	void :target:`U3_Gate<doxid-_quantum_gates_8h_1ae8a4f4f2334ca91a60accef7810ec369>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double theta,
		double phi,
		double lambda,
		bool isDagger
		);

	void :target:`U4_Gate<doxid-_quantum_gates_8h_1aa43adf6d8e4ba956ff9874549a1c076c>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double alpha,
		double beta,
		double gamma,
		double delta,
		bool isDagger
		);

	void :target:`CZ_Gate<doxid-_quantum_gates_8h_1a04925e5eb89ea5a7b9678248014cbf4c>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`CNOT_Gate<doxid-_quantum_gates_8h_1a6a2cdb8ffda4aa596afdb48e05620db4>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`ISWAP_Gate<doxid-_quantum_gates_8h_1a70146d0ca23f663c65e8eba3edca84bc>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`SQISWAP_Gate<doxid-_quantum_gates_8h_1a9bc45f6b002cb4df8123d4adeb637ede>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`SWAP_Gate<doxid-_quantum_gates_8h_1a8eba39db111b03c120fd7a152b360733>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	void :target:`CR_Gate<doxid-_quantum_gates_8h_1abc08b433de2e5417f6fcd8124e7f253a>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		double angle,
		bool isDagger
		);

	void :target:`TOFFOLI_Gate<doxid-_quantum_gates_8h_1a13c5c96c92bd0759a504143f9341d1d9>`(
		:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& gate_tensor,
		bool isDagger
		);

	DLLEXPORT :ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* :ref:`initialize<doxid-_chemi_q_i_f_c_8h_1a54f4eda15dd20e82919fcc100fb101b1>`(char* dir);
	DLLEXPORT void :ref:`finalize<doxid-_chemi_q_i_f_c_8h_1a35c742ebb04759d05160c183573ab4bb>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq);
	DLLEXPORT void :ref:`setMolecule<doxid-_chemi_q_i_f_c_8h_1aff908db723c06f88faaaef4d80526cab>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecule);
	DLLEXPORT void :ref:`setMolecules<doxid-_chemi_q_i_f_c_8h_1a62cbe512973d55ce78d1098c69f651b8>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecules);
	DLLEXPORT void :ref:`setMultiplicity<doxid-_chemi_q_i_f_c_8h_1afa4616781c758abdd0e310cc583cc306>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int multiplicity);
	DLLEXPORT void :ref:`setCharge<doxid-_chemi_q_i_f_c_8h_1a0937e49cf4c0ac3e114c6c2c449bfe40>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int charge);
	DLLEXPORT void :ref:`setBasis<doxid-_chemi_q_i_f_c_8h_1a39356f40f231e4533f6225413d8b3901>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* basis);
	DLLEXPORT void :ref:`setEqTolerance<doxid-_chemi_q_i_f_c_8h_1a44dc21780dca0c8b323964422b1c0493>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double val);
	DLLEXPORT void :ref:`setTransformType<doxid-_chemi_q_i_f_c_8h_1a57571abf529d58ef4d197eb838a0df97>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type);
	DLLEXPORT void :ref:`setUccType<doxid-_chemi_q_i_f_c_8h_1a345009bff8bc327845abc1717c1714a3>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type);
	DLLEXPORT void :ref:`setOptimizerType<doxid-_chemi_q_i_f_c_8h_1a05337011ecbc3cdaec08d1b03cecfd47>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type);
	DLLEXPORT void :ref:`setOptimizerIterNum<doxid-_chemi_q_i_f_c_8h_1ad864b5c29eacb4a7c6254a7ef20e0cb6>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value);
	DLLEXPORT void :ref:`setOptimizerFuncCallNum<doxid-_chemi_q_i_f_c_8h_1a561c06e5f054902e7cb65a8b242090f8>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value);
	DLLEXPORT void :ref:`setOptimizerXatol<doxid-_chemi_q_i_f_c_8h_1aae3ec08bfa9031ff5a3aee9eebdc1875>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	DLLEXPORT void :ref:`setOptimizerFatol<doxid-_chemi_q_i_f_c_8h_1a2c60296f22a5c3d2b79b194cfc75a2d8>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	DLLEXPORT void :ref:`setLearningRate<doxid-_chemi_q_i_f_c_8h_1aa45474eef8eb830b36ff62efab13f60a>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	DLLEXPORT void :ref:`setEvolutionTime<doxid-_chemi_q_i_f_c_8h_1adb9bce782572809474d8bfb805209336>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value);
	DLLEXPORT void :ref:`setHamiltonianSimulationSlices<doxid-_chemi_q_i_f_c_8h_1a7d5ccdc7d940147460c495a566c85627>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value);
	DLLEXPORT void :ref:`setSaveDataDir<doxid-_chemi_q_i_f_c_8h_1ab3e2454f231223067408305835b4105d>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* dir);
	DLLEXPORT int :ref:`getQubitsNum<doxid-_chemi_q_i_f_c_8h_1a81e94b8cdf104c702a20d2f52eebced7>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq);
	DLLEXPORT bool :ref:`exec<doxid-_chemi_q_i_f_c_8h_1a76ea93400681d101a95281b713f55211>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq);
	const DLLEXPORT char* :ref:`getLastError<doxid-_chemi_q_i_f_c_8h_1a6f7a633eff5c786c3d94002c6b8ed6dc>`(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq);

	// macros

	#define :target:`ANGLE_VAR_BASE<doxid-_json_config_param_8h_1af592bbef89c099f8d0ca85ac99e053b1>`
	#define :target:`COMPENSATE_ANGLE<doxid-_json_config_param_8h_1adff2a0561cde8a1d2c6814483863688b>`
	#define :target:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`
	#define :target:`CONST_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a18005d49ae00702328d036fc06855285>`(NAME)
	#define :target:`CONTROL_CONST_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a6d0815a9698bafe7f2d1687e3287ae16>`(NAME)
	#define :target:`CONTROL_SINGLE_ANGLE_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a68f818200ac956e8ccee01f59d6c3e49>`(NAME)
	#define :target:`DECL_ANGLE_GATE_MATRIX<doxid-_c_p_u_impl_q_p_u_8h_1ad412042fda449c86a58d4be0c1bdb968>`(NAME)
	#define :target:`DECL_GATE_MATRIX<doxid-_c_p_u_impl_q_p_u_8h_1a52269caa683e0718f0d36d007952c9d8>`(NAME)
	#define :target:`DEFAULT_THREAD_CNT<doxid-_thread_pool_8h_1afaec1f11c35702b38040be5ed91dfd5e>`
	#define :target:`DOUBLE_GATE_TIME<doxid-_grid_device_8h_1a7ecbe58a45346d1d72c6a1dd3c349d5f>`
	#define :target:`DoubleGateMatrixSize<doxid-_transform_decomposition_8h_1a786eca5682d042d2a5a9d8c3e967213e>`
	#define :target:`GATE_BARRIER<doxid-_tranform_q_gate_type_string_and_enum_8h_1a6c7e2c067c0520d67bf21365ddff2fc5>`
	#define :target:`GATE_CNOT<doxid-_tranform_q_gate_type_string_and_enum_8h_1aa70918acb12d7206233c9d51e935a2c3>`
	#define :target:`GATE_CPHASE<doxid-_tranform_q_gate_type_string_and_enum_8h_1afa36c891f1f8e486f87b943d5c9b554d>`
	#define :target:`GATE_CU<doxid-_tranform_q_gate_type_string_and_enum_8h_1af3a7f838fedac1e3b5932d4ca94ebdc4>`
	#define :target:`GATE_CZ<doxid-_tranform_q_gate_type_string_and_enum_8h_1ae365f3a56f9bbe6804e508d31088d6b6>`
	#define :target:`GATE_ECHO<doxid-_tranform_q_gate_type_string_and_enum_8h_1a93e7b186e3d6d6701dd57b11e231a5d8>`
	#define :target:`GATE_H<doxid-_tranform_q_gate_type_string_and_enum_8h_1accf1399ed9e119b2ebf1052343a8d900>`
	#define :target:`GATE_I<doxid-_tranform_q_gate_type_string_and_enum_8h_1a658192c84784d8c41556ec2060ee7c1f>`
	#define :target:`GATE_ISWAP<doxid-_tranform_q_gate_type_string_and_enum_8h_1add29a4c4aa0ee58dc2fadc8eef1578c4>`
	#define :target:`GATE_ISWAPTheta<doxid-_tranform_q_gate_type_string_and_enum_8h_1a0b644e94bde80ac69c44defff475bee2>`
	#define :target:`GATE_QDoubleGate<doxid-_tranform_q_gate_type_string_and_enum_8h_1a1c6415c6857039a2d667d820e26669cf>`
	#define :target:`GATE_RPHI<doxid-_tranform_q_gate_type_string_and_enum_8h_1a2ed7e448bba3c78b3c7144893385c426>`
	#define :target:`GATE_RX<doxid-_tranform_q_gate_type_string_and_enum_8h_1ac92a2dfe0627d9dff1d58d0372f4077d>`
	#define :target:`GATE_RY<doxid-_tranform_q_gate_type_string_and_enum_8h_1a84559b227a6bc8186adfe562e3e19d18>`
	#define :target:`GATE_RZ<doxid-_tranform_q_gate_type_string_and_enum_8h_1a48512e139cb1a052fa3415072ee88481>`
	#define :target:`GATE_S<doxid-_tranform_q_gate_type_string_and_enum_8h_1a08d87fe113f166f07f48999cca3ed782>`
	#define :target:`GATE_SQISWAP<doxid-_tranform_q_gate_type_string_and_enum_8h_1aa51ec35406c5c4eaae0663308a70fb1b>`
	#define :target:`GATE_SWAP<doxid-_tranform_q_gate_type_string_and_enum_8h_1ae6d42c357b188bfe0bdda90cc37fbb5d>`
	#define :target:`GATE_T<doxid-_tranform_q_gate_type_string_and_enum_8h_1ad25c2469366ad1f114d81446ccc1ed36>`
	#define :target:`GATE_TYPE_MEASURE<doxid-_noise_model_8h_1a6b86504a58ad7b643150bd14dcef22eb>`
	#define :target:`GATE_TYPE_READOUT<doxid-_noise_model_8h_1a6a266722b48d853ac9923eef94ef0816>`
	#define :target:`GATE_TYPE_RESET<doxid-_noise_model_8h_1a5ac8e272c8a4eabdeb5a35c3494df9d3>`
	#define :target:`GATE_U1<doxid-_tranform_q_gate_type_string_and_enum_8h_1ab1908d026e4a23e1d670a3dd8e527f18>`
	#define :target:`GATE_U2<doxid-_tranform_q_gate_type_string_and_enum_8h_1a154270213218edde8b1eec1d789ffba7>`
	#define :target:`GATE_U3<doxid-_tranform_q_gate_type_string_and_enum_8h_1a6d683e20d2deeb9113624089eda3524d>`
	#define :target:`GATE_U4<doxid-_tranform_q_gate_type_string_and_enum_8h_1a137c1fe302b99579d93ea9694ba7784e>`
	#define :target:`GATE_X<doxid-_tranform_q_gate_type_string_and_enum_8h_1a34f5a4f262106b39200bc9410214bd2e>`
	#define :target:`GATE_X1<doxid-_tranform_q_gate_type_string_and_enum_8h_1ad73c6d04ea4aec14fb0bd5ebe02cd55b>`
	#define :target:`GATE_Y<doxid-_tranform_q_gate_type_string_and_enum_8h_1a21e02e2eb12a12b2dc29222059c8f905>`
	#define :target:`GATE_Y1<doxid-_tranform_q_gate_type_string_and_enum_8h_1a2e16e050b1c22c31c438f0bc0a59501e>`
	#define :target:`GATE_Z<doxid-_tranform_q_gate_type_string_and_enum_8h_1ae4764c59ee9523bedf9b94da3d6afb7d>`
	#define :target:`GATE_Z1<doxid-_tranform_q_gate_type_string_and_enum_8h_1a61252043ca3cf2606a60dc1519ff90f4>`
	#define :target:`HIGH_FREQUENCY_QUBIT<doxid-_json_config_param_8h_1adcfbdc73a733e0cd5784510956e2c68e>`
	#define :target:`INF<doxid-_origin_c_o_b_y_l_a_8h_1a12c2040f25d8e3a7b9e1c2024c618cb6>`
	#define :target:`INF<doxid-_origin_l_b_f_g_s_b_8h_1a12c2040f25d8e3a7b9e1c2024c618cb6>`
	#define :target:`INF<doxid-_origin_s_l_s_q_p_8h_1a12c2040f25d8e3a7b9e1c2024c618cb6>`
	#define :target:`KMETADATA_GATE_TYPE_COUNT<doxid-_transform_decomposition_8h_1a14d296229066432844f3c67b1375898d>`
	#define :target:`MACRO_GET_GATETYPE<doxid-_origin_i_r_to_q_prog_8h_1a9d1e3b75ddfa6d98b095382065226e85>`(name)
	#define :target:`MAX_COMPARE_PRECISION<doxid-_q_stat_matrix_8h_1aaab9ae15c383b59119c5834d77704d26>`
	#define :target:`MAX_LAYER<doxid-_process_on_traversing_8h_1a912d8a5fc768baa70d250f6d8f0cf751>`
	#define :target:`MAX_THREADS<doxid-_thread_pool_8h_1a8b5173357adb02a86c027316e0acdfa0>`
	#define :target:`PI<doxid-_noise_c_p_u_impl_q_p_u_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :target:`PI<doxid-_c_p_u_impl_q_p_u_single_thread_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :target:`PI<doxid-_c_p_u_impl_q_p_u_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :target:`PI<doxid-_prase_expression_str_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :target:`PI<doxid-_oracle_8h_1a598a3330b3c21701223ee0ca14316eca>`
	#define :target:`PRINT_TRACE<doxid-_search_space_8h_1a31c31bc14c0a859acd22b782f55e38a2>`
	#define :target:`PRINT_TRACE<doxid-_q_p_e_8h_1a31c31bc14c0a859acd22b782f55e38a2>`
	#define :target:`PRINT_TRACE<doxid-_grover_algorithm_8h_1a31c31bc14c0a859acd22b782f55e38a2>`
	#define :target:`PRINT_TRACE<doxid-_search_data_type_8h_1a31c31bc14c0a859acd22b782f55e38a2>`
	#define :target:`PRINT_TRACE<doxid-_quantum_counting_8h_1a31c31bc14c0a859acd22b782f55e38a2>`
	#define :target:`PRINT_TRACE<doxid-_oracle_8h_1a31c31bc14c0a859acd22b782f55e38a2>`
	#define :ref:`QCERR<doxid-_q_panda_namespace_8h_1acb29825331db5ae6632fbb0647a72534>`(x)

	#define :target:`QCERR_AND_THROW<doxid-_q_panda_namespace_8h_1aa593575691cacd4f398f17842c52da25>`( \
		std_exception, \
		_Message_ \
		)

	#define :ref:`QCERR_AND_THROW_ERRSTR<doxid-_q_panda_namespace_8h_1aac47299986cc9e801758ad7946bea4b2>`( \
		std_exception, \
		x \
		)

	#define :target:`QCIRCUIT_OPTIMIZER<doxid-_json_config_param_8h_1a90c1173bac3e0c194a52b65b22382c66>`
	#define :target:`QIF_REGISTER<doxid-_control_flow_8h_1a35a941193ad6c93151abfcef3528b3d9>`(className)

	#define :target:`QPANDA_ASSERT<doxid-_q_panda_namespace_8h_1a14cac1e094ac288c788c71afac2ffc4c>`( \
		con, \
		argv \
		)

	#define :target:`QPANDA_BEGIN<doxid-_q_panda_namespace_8h_1a375c0f5e0d6568b83528815afc55ff80>`
	#define :target:`QPANDA_END<doxid-_q_panda_namespace_8h_1a9d806bab2e1c7ce92bcacc6b92a9bc56>`
	#define :target:`QPANDA_MAJOR_VERSION<doxid-_q_panda_version_8h_1a48e2632dfb9270c54aae8fe071ad474e>`
	#define :target:`QPANDA_MINOR_VERSION<doxid-_q_panda_version_8h_1a4098041d07b1dbc91cc2d4604d3ecd1c>`

	#define :target:`QPANDA_OP<doxid-_q_panda_namespace_8h_1aa7eaf0750827df972ee0af8b14e4b0b1>`( \
		con, \
		op \
		)

	#define :target:`QPANDA_PATCH_VERSION<doxid-_q_panda_version_8h_1af34d2ab9691f05843fe2b55e21c40845>`

	#define :target:`QPANDA_RETURN<doxid-_q_panda_namespace_8h_1a6b4c9da880c984086f036b337f9eae29>`( \
		con, \
		value \
		)

	#define :target:`QUBIT_ADJACENT_MATRIX<doxid-_json_config_param_8h_1a5d878ab7b4d9b9dec04e5da21c834d69>`
	#define :target:`QWHILE_REGISTER<doxid-_control_flow_8h_1a2e7197bd17e1381a1b7d3543c885c833>`(className)

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
	#define :target:`SAFE_DELETE_PTR<doxid-_judge_two_node_iter_is_swappable_8h_1a9ab67f7f66ec2e7a2dc3542cf06a6fb8>`(p)
	#define :target:`SINGLETON_DECLARE<doxid-macro_8h_1a86a90fab08d07cd727c94da9594a1de2>`(Type)
	#define :target:`SINGLETON_IMPLEMENT_EAGER<doxid-macro_8h_1add8c8d20b359e4be7a7451fa1052db63>`(Type)
	#define :target:`SINGLETON_IMPLEMENT_LAZY<doxid-macro_8h_1ad5ff7948e947124a9de03a299399cffd>`(Type)
	#define :target:`SINGLE_ANGLE_GATE<doxid-_c_p_u_impl_q_p_u_8h_1a3ba9b536f4f4be4ddb39870acb88f43a>`(NAME)
	#define :target:`SINGLE_GATE_TIME<doxid-_grid_device_8h_1a3d2e28c7dbe57ee37779ec3ede77ebaa>`
	#define :target:`SQ2<doxid-_c_p_u_impl_q_p_u_single_thread_8h_1a0b19f406e0cc4cbaf7a935f155567869>`
	#define :target:`SQ2<doxid-_c_p_u_impl_q_p_u_8h_1a0b19f406e0cc4cbaf7a935f155567869>`
	#define :target:`SQ2<doxid-_noise_c_p_u_impl_q_p_u_8h_1a0b19f406e0cc4cbaf7a935f155567869>`
	#define :target:`SWAP_TIME<doxid-_grid_device_8h_1acea310a60cd0d3bbd40c1eaf149a3f29>`
	#define :target:`SingleGateMatrixSize<doxid-_transform_decomposition_8h_1a5cc35d85fd0872be5f41ffd4c971f52c>`
	#define :target:`UNDEF_DOUBLE<doxid-_transform_decomposition_8h_1a88c85d3154f2c63a1019a79f203f8f0f>`
	#define :target:`USING_QPANDA<doxid-_q_panda_namespace_8h_1af7466c9c1ed8b95983912dd5449b75f4>`
	#define :target:`VIRTUAL_Z_CONFIG<doxid-_json_config_param_8h_1acf581a6115c010987537a843e5bec8d4>`
	#define :target:`ZeroJudgement<doxid-_transform_decomposition_8h_1ae5cd83615b00885b469014317591e8d8>`
	#define :target:`_DOUBLE_ANGLE_GATE<doxid-_partial_amplitude_graph_8h_1ac4ac74220876e7668927a747d8c4c385>`(NAME)
	#define :target:`_DOUBLE_GATE<doxid-_partial_amplitude_graph_8h_1a25aa5fb0f107d2c3e3b9c6851251e880>`(NAME)
	#define :target:`_SINGLE_ANGLE_GATE<doxid-_partial_amplitude_graph_8h_1ab04bb57d9d2c1c3ad8b126dd3db64bdc>`(NAME)
	#define :target:`_SINGLE_GATE<doxid-_partial_amplitude_graph_8h_1abd4b56edaa9b31f023d2a10e7d66cb62>`(NAME)
	#define :target:`_TRIPLE_GATE<doxid-_partial_amplitude_graph_8h_1a8cbc0d2696af3e70b30079778246f130>`(NAME)
	#define :target:`__FILENAME__<doxid-_q_panda_namespace_8h_1a5fccb4fc71e44089a1b1a77fc76c0b68>`

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

	const :ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>` PI = 3.14159265358979323846

Square root of two

Global Functions
----------------

.. index:: pair: function; integerToBinary
.. _doxid-group___utilities_1gaa65528bba400afbe3456b569805c1275:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename UnsignedIntegralType>
	std::string integerToBinary(
		const UnsignedIntegralType& number,
		int ret_len
		)

Unsigned integer to binary string.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- UnsignedIntegralType & number

	*
		- int

		- binary string length



.. rubric:: Returns:

std::string unsigned integer string

.. index:: pair: function; integerToString
.. _doxid-group___utilities_1ga674c5935aa6e6b7f5fc63dab3b4376c2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename UnsignedIntegralType>
	std::string integerToString(const UnsignedIntegralType& number)

Unsigned integer to binary string.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- UnsignedIntegralType & number



.. rubric:: Returns:

std::string unsigned integer string

.. index:: pair: function; getDecIndex
.. _doxid-group___utilities_1gae427c07ca7652b1f831ccf1eda056393:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename UnsignedIntegralType>
	UnsignedIntegralType getDecIndex(
		const UnsignedIntegralType& num1,
		const UnsignedIntegralType& num2,
		std::vector<size_t> qvec,
		size_t len
		)

Get quantum state dec index in pmeasure.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- UnsignedIntegralType & num1

	*
		- const

		- UnsignedIntegralType & num2

	*
		- std::vector<size_t>

		- qvec

	*
		- size_t

		- binary string length



.. rubric:: Returns:

Unsigned Integral Type

.. index:: pair: function; initialize
.. _doxid-_chemi_q_i_f_c_8h_1a54f4eda15dd20e82919fcc100fb101b1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT :ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* initialize(char* dir)

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

	DLLEXPORT void finalize(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq)

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

	DLLEXPORT void setMolecule(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecule)

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

	DLLEXPORT void setMolecules(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* molecules)

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

	DLLEXPORT void setMultiplicity(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int multiplicity)

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

	DLLEXPORT void setCharge(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int charge)

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

	DLLEXPORT void setBasis(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* basis)

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

.. index:: pair: function; setEqTolerance
.. _doxid-_chemi_q_i_f_c_8h_1a44dc21780dca0c8b323964422b1c0493:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT void setEqTolerance(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double val)

Set Eq Tolerance.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr

	*
		- double

		- EqTolerance value

.. index:: pair: function; setTransformType
.. _doxid-_chemi_q_i_f_c_8h_1a57571abf529d58ef4d197eb838a0df97:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT void setTransformType(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type)

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

QPanda::TransFormType

.. index:: pair: function; setUccType
.. _doxid-_chemi_q_i_f_c_8h_1a345009bff8bc327845abc1717c1714a3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT void setUccType(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type)

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

QPanda::UccType

.. index:: pair: function; setOptimizerType
.. _doxid-_chemi_q_i_f_c_8h_1a05337011ecbc3cdaec08d1b03cecfd47:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT void setOptimizerType(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int type)

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

QPanda::OptimizerType

.. index:: pair: function; setOptimizerIterNum
.. _doxid-_chemi_q_i_f_c_8h_1ad864b5c29eacb4a7c6254a7ef20e0cb6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT void setOptimizerIterNum(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value)

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

	DLLEXPORT void setOptimizerFuncCallNum(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value)

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

	DLLEXPORT void setOptimizerXatol(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

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

	DLLEXPORT void setOptimizerFatol(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

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

	DLLEXPORT void setLearningRate(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

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

	DLLEXPORT void setEvolutionTime(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, double value)

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

	DLLEXPORT void setHamiltonianSimulationSlices(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, int value)

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

	DLLEXPORT void setSaveDataDir(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq, char* dir)

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

.. index:: pair: function; getQubitsNum
.. _doxid-_chemi_q_i_f_c_8h_1a81e94b8cdf104c702a20d2f52eebced7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT int getQubitsNum(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq)

get qubits num with the above config.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr



.. rubric:: Returns:

int -1:means failed.

.. index:: pair: function; exec
.. _doxid-_chemi_q_i_f_c_8h_1a76ea93400681d101a95281b713f55211:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DLLEXPORT bool exec(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq)

exec molecule calculate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr



.. rubric:: Returns:

bool true:success; false:failed

.. index:: pair: function; getLastError
.. _doxid-_chemi_q_i_f_c_8h_1a6f7a633eff5c786c3d94002c6b8ed6dc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const DLLEXPORT char* getLastError(:ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`* chemiq)

get last error.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ChemiQ\*

		- the target ChemiQ object ptr



.. rubric:: Returns:

char\* last error

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

