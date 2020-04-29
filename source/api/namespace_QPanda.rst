.. index:: pair: namespace; QPanda
.. _doxid-namespace_q_panda:

namespace QPanda
================

.. toctree::
	:hidden:

	namespace_QPanda_Variational.rst
	enum_QPanda_ArchType.rst
	enum_QPanda_ContentSpecifier.rst
	enum_QPanda_DoubleGateTransferType.rst
	enum_QPanda_GraphType.rst
	enum_QPanda_IBMQBackends.rst
	enum_QPanda_OperatorSpecifier.rst
	enum_QPanda_OptimizerType.rst
	enum_QPanda_QASMGateType.rst
	enum_QPanda_QMachineType.rst
	enum_QPanda_QProgStoredNodeType.rst
	enum_QPanda_SequenceNodeType.rst
	enum_QPanda_SingleGateTransferType.rst
	enum_QPanda_SwapQubitsMethod.rst
	enum_QPanda_TEXT_PIC_TYPE.rst
	enum_QPanda_TransFormType.rst
	enum_QPanda_UccType.rst
	struct_QPanda_Dist.rst
	struct_QPanda_GataFuncInfo.rst
	struct_QPanda_GateOperationInfo.rst
	struct_QPanda_QGateNode.rst
	struct_QPanda_QGatesTransform.rst
	struct_QPanda_QGraphItem.rst
	struct_QPanda_QOptimizationResult.rst
	struct_QPanda_QPosition.rst
	struct_QPanda_QScanPara.rst
	struct_QPanda_QTwoPara.rst
	struct_QPanda_QubitPointerCmp.rst
	struct_QPanda_RegParamInfo.rst
	struct_QPanda_SequenceNode.rst
	struct_QPanda__blocked_matrix.rst
	struct_QPanda__matrix_block.rst
	struct_QPanda_axis.rst
	struct_QPanda_edge.rst
	struct_QPanda_gate.rst
	struct_QPanda_node.rst
	struct_QPanda_node_cmp.rst
	class_QPanda_AbstractHandleNodes.rst
	class_QPanda_CPUQVM.rst
	class_QPanda_CPUSingleThreadQVM.rst
	class_QPanda_Configuration.rst
	class_QPanda_DecomposeControlSingleQGateIntoMetadataDoubleQGate.rst
	class_QPanda_DeleteUnitQNode.rst
	class_QPanda_DrawBox.rst
	class_QPanda_DrawByLayer.rst
	class_QPanda_DrawPicture.rst
	class_QPanda_FillLayerByNextLayerNodes.rst
	class_QPanda_GPUQVM.rst
	class_QPanda_GetUsedQubits.rst
	class_QPanda_IdealMachineInterface.rst
	class_QPanda_IdealQVM.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable.rst
	class_QPanda_MultiPrecisionMachineInterface.rst
	class_QPanda_NodeIter.rst
	class_QPanda_NoiseQVM.rst
	class_QPanda_OriginCollection.rst
	class_QPanda_OriginMeasure.rst
	class_QPanda_PickUpNodes.rst
	class_QPanda_QGateParseMap.rst
	class_QPanda_QMachineStatus.rst
	class_QPanda_QObject.rst
	class_QPanda_QProgToDAG.rst
	class_QPanda_QVM.rst
	class_QPanda_QWhileRegisterAction.rst
	class_QPanda_QuantumCircuitRegisterAction.rst
	class_QPanda_QuantumMeasureRegisterAction.rst
	class_QPanda_QuantumProgramRegisterAction.rst
	class_QPanda_QuantumResetRegisterAction.rst
	class_QPanda_QubitAddr.rst
	class_QPanda_TryToMergeTimeSequence.rst
	class_QPanda_Wire.rst
	class_QPanda_calloc_fail.rst
	class_QPanda_gate_alloc_fail.rst

Overview
~~~~~~~~

QPanda2 base namespace. :ref:`More...<details-namespace_q_panda>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace QPanda {

	// namespaces

	namespace :ref:`QPanda::Variational<doxid-namespace_q_panda_1_1_variational>`;

	// typedefs

	typedef std::complex<double> :target:`complex_d<doxid-namespace_q_panda_1ac3d0f6af35ff25d21d77efc61890bce3>`;
	typedef std::vector<int> :target:`vector_i<doxid-namespace_q_panda_1ac7e08fc52ffbe9452add2c576b8ac4a3>`;
	typedef std::vector<double> :target:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`;
	typedef std::vector<std::string> :target:`vector_s<doxid-namespace_q_panda_1a81f654d5e024b7b9de5b4a14ded7b164>`;
	typedef std::vector<:ref:`QGraphItem<doxid-struct_q_panda_1_1_q_graph_item>`> :target:`QGraph<doxid-namespace_q_panda_1ae453b3fa92a6aec65ebb5c554d47f1e5>`;
	typedef std::pair<std::string, double> :target:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`;
	typedef std::function<:ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`(:ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`)> :target:`QFunc<doxid-namespace_q_panda_1a801c623e7ed0e99219b7e63e3f27d4e1>`;
	typedef std::function<double(const std::string&)> :target:`QUserDefinedFunc<doxid-namespace_q_panda_1a70bd7af3a5b6b5650c425d3aa9f52774>`;
	typedef std::map<std::string, double> :target:`QProbMap<doxid-namespace_q_panda_1a3ff20da17ad123a7d8669295f0802e9b>`;
	typedef std::map<size_t, char> :ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`;
	typedef std::pair<size_t, char> :target:`QTermPair<doxid-namespace_q_panda_1a306befdf66281e6a3d8d4d52ee8023b5>`;
	typedef std::pair<:ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`, double> :target:`QHamiltonianItem<doxid-namespace_q_panda_1af4bacee5a2d4023c0c88daa63659701b>`;
	typedef std::vector<:ref:`QHamiltonianItem<doxid-namespace_q_panda_1af4bacee5a2d4023c0c88daa63659701b>`> :target:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>`;
	typedef std::pair<:ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`, std::string> :target:`QPauliPair<doxid-namespace_q_panda_1a922b9a7c131f853272fc7115017e9bb8>`;
	typedef std::map<std::string, :ref:`complex_d<doxid-namespace_q_panda_1ac3d0f6af35ff25d21d77efc61890bce3>`> :target:`QPauliMap<doxid-namespace_q_panda_1a34d536a170f46858ef57b8b4bc2e85d1>`;
	typedef std::map<size_t, size_t> :target:`QIndexMap<doxid-namespace_q_panda_1a6816e6752588f193e62b20ee8c415570>`;
	typedef std::pair<std::string, :ref:`QPosition<doxid-struct_q_panda_1_1_q_position>`> :target:`QAtomPos<doxid-namespace_q_panda_1a8529c6a429d92fa793a36f554d0d42fb>`;
	typedef std::vector<:ref:`QAtomPos<doxid-namespace_q_panda_1a8529c6a429d92fa793a36f554d0d42fb>`> :target:`QMoleculeGeometry<doxid-namespace_q_panda_1a2310d7c1417b874ecb7f9df5aba74384>`;
	typedef std::vector<std::vector<:ref:`QPosition<doxid-struct_q_panda_1_1_q_position>`>> :target:`QAtomsPosGroup<doxid-namespace_q_panda_1a7cce52c44c65bd3ec17e249b9dad5315>`;
	typedef std::pair<size_t, bool> :target:`OrbitalAct<doxid-namespace_q_panda_1a9c6d0253907c2569d9b1190d87c440fd>`;
	typedef std::vector<:ref:`OrbitalAct<doxid-namespace_q_panda_1a9c6d0253907c2569d9b1190d87c440fd>`> :target:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`;
	typedef std::pair<:ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`, std::string> :target:`FermionPair<doxid-namespace_q_panda_1a4d9726c70eb40664ad8816323dc3420b>`;
	typedef :ref:`FermionOp<doxid-class_q_panda_1_1_fermion_op>`<:ref:`complex_d<doxid-namespace_q_panda_1ac3d0f6af35ff25d21d77efc61890bce3>`> :target:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`;
	typedef :ref:`PauliOp<doxid-class_q_panda_1_1_pauli_op>`<:ref:`complex_d<doxid-namespace_q_panda_1ac3d0f6af35ff25d21d77efc61890bce3>`> :target:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`;
	typedef :ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`* (*:target:`CreateClassicalQProgram<doxid-namespace_q_panda_1a8e863438215e55293e6888776d035fed>`)(ClassicalCondition &);

	typedef :ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`* (*:target:`CreateQIfTrueFalse_cb<doxid-namespace_q_panda_1a7000829c94e35e8ec34754dcf3ab0285>`)(
		ClassicalCondition &,
		QProg,
		QProg
		);

	typedef :ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`* (*:target:`CreateQIfTrueOnly_cb<doxid-namespace_q_panda_1a7788fff614f34e49856571d7a6e67bac>`)(
		ClassicalCondition &,
		QProg
		);

	typedef :ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`* (*:target:`CreateQWhile_cb<doxid-namespace_q_panda_1a36f049facff04a87084023a0cd28f40a>`)(
		ClassicalCondition &,
		QProg
		);

	typedef :ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`* (*:target:`CreateQCircuit<doxid-namespace_q_panda_1ab8c010d113d8febb212ee484acb321a3>`)();

	typedef void (*:target:`QGATE_FUN<doxid-namespace_q_panda_1abb3e82bd13f4421d284e30ef5fb2e673>`)(
		QuantumGate *,
		QVec &,
		QPUImpl *,
		bool,
		QVec &,
		GateType
		);

	typedef std::map<int, :ref:`QGATE_FUN<doxid-namespace_q_panda_1abb3e82bd13f4421d284e30ef5fb2e673>`> :target:`QGATE_FUN_MAP<doxid-namespace_q_panda_1a8fdcbe482b7b92ff5dccc38cd68fd789>`;
	typedef int64_t :target:`qmap_size_t<doxid-namespace_q_panda_1a0fa97ce1598fc0399345a33fde3d9509>`;
	typedef :ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`* (*:target:`CreateQProgram<doxid-namespace_q_panda_1a56c39ff2ef01b4b9bc43db917c14936f>`)();
	typedef :ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`* (*:target:`CreateReset<doxid-namespace_q_panda_1a1baefdbe7a211e28b9f569e7a097352a>`)(Qubit *);

	typedef :ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`* (*:target:`CreateMeasure<doxid-namespace_q_panda_1aaa3162dce15c83be0503e264ff0059dd>`)(
		Qubit *,
		CBit *
		);

	typedef long long :target:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`;
	typedef std::pair<std::string, std::string> :target:`CONFIGPAIR<doxid-namespace_q_panda_1a8721144e3a186226ea5fb253cf070b9e>`;
	typedef std::function<int(std::vector<std::string>&, std::vector<std::string>&)> :ref:`MetadataValidity_cb<doxid-namespace_q_panda_1a702b41a7cbaaed0e602ffdd3f2511317>`;
	typedef std::vector<:ref:`SequenceNode<doxid-struct_q_panda_1_1_sequence_node>`> :target:`LayerVector<doxid-namespace_q_panda_1a5ed71ba2abd92c86403dd13b08c531ad>`;
	typedef std::vector<:ref:`LayerVector<doxid-namespace_q_panda_1a5ed71ba2abd92c86403dd13b08c531ad>`> :target:`ResultVector<doxid-namespace_q_panda_1a960ac3f5e928f3a42f4d2f2191320897>`;
	typedef std::vector<std::pair<size_t, size_t>> :target:`edges_vec<doxid-namespace_q_panda_1a92853354a820eec4470ae33d66336d52>`;
	typedef Eigen::MatrixXi :target:`AdjacencyMatrix<doxid-namespace_q_panda_1a97e0cecb440ec41f5e549157287bc9c1>`;
	typedef std::pair<:ref:`SequenceNode<doxid-struct_q_panda_1_1_sequence_node>`, std::vector<:ref:`SequenceNode<doxid-struct_q_panda_1_1_sequence_node>`>> :target:`LayerNode<doxid-namespace_q_panda_1a938929f0b8ce3f9d0ce8b83788e9f69f>`;
	typedef std::vector<:ref:`LayerNode<doxid-namespace_q_panda_1a938929f0b8ce3f9d0ce8b83788e9f69f>`> :target:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`;
	typedef std::vector<:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`> :target:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`;
	typedef rapidjson::Value :target:`Value<doxid-namespace_q_panda_1a357287aa8ffcc2a405908fc71aa6d032>`;
	typedef struct :ref:`QPanda::_matrix_block<doxid-struct_q_panda_1_1__matrix__block>` :target:`matrixBlock_t<doxid-namespace_q_panda_1a9753db2b417a7379fcaa4d34f65c8b1f>`;
	typedef struct :ref:`QPanda::_blocked_matrix<doxid-struct_q_panda_1_1__blocked__matrix>` :target:`blockedMatrix_t<doxid-namespace_q_panda_1a8f8db55e468baa3e5febdb847979eadc>`;
	typedef std::function<:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`(InputType, OutputType)> :target:`Oracle<doxid-namespace_q_panda_1a66441c31970a84d96c8108a14f331dd1>`;
	typedef :ref:`FermionOp<doxid-class_q_panda_1_1_fermion_op>`<:ref:`complex_var<doxid-class_q_panda_1_1complex__var>`> :target:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`;
	typedef :ref:`PauliOp<doxid-class_q_panda_1_1_pauli_op>`<:ref:`complex_var<doxid-class_q_panda_1_1complex__var>`> :target:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`;
	typedef :ref:`Oracle<doxid-namespace_q_panda_1a66441c31970a84d96c8108a14f331dd1>`<:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> :target:`BV_Oracle<doxid-namespace_q_panda_1ae77eda567be203be8fc4bbe4102358f0>`;
	typedef :ref:`Oracle<doxid-namespace_q_panda_1a66441c31970a84d96c8108a14f331dd1>`<:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> :target:`DJ_Oracle<doxid-namespace_q_panda_1a128c4092d904b9f5b0ee5b6fc6e25a95>`;
	typedef :ref:`Oracle<doxid-namespace_q_panda_1a66441c31970a84d96c8108a14f331dd1>`<:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> :target:`grover_oracle<doxid-namespace_q_panda_1a11c0bf85de02b818d471d9dc2997ad30>`;

	// enums

	enum :ref:`ArchType<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2a>`;
	enum :ref:`ContentSpecifier<doxid-namespace_q_panda_1a72e1cfe14a3974764bed0e98fd46b487>`;
	enum :ref:`DoubleGateTransferType<doxid-namespace_q_panda_1ad1987cd7e0569564c5bcd31d4a5a7e0d>`;
	enum :ref:`GraphType<doxid-namespace_q_panda_1a57710cc0949cf69a28d46e57bcc29f62>`;
	enum :ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>`;
	enum :ref:`OperatorSpecifier<doxid-namespace_q_panda_1a1b2dbb4edc761803cfa90e7a88bb0c49>`;
	enum :ref:`OptimizerType<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>`;
	enum :ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>`;
	enum :ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>`;
	enum :ref:`QProgStoredNodeType<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8a>`;
	enum :ref:`SequenceNodeType<doxid-namespace_q_panda_1a9d64ac127dc702cf9fc6a1b4cdd96a97>`;
	enum :ref:`SingleGateTransferType<doxid-namespace_q_panda_1acb66bed7e528a5a642087aa9882468b8>`;
	enum :ref:`SwapQubitsMethod<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73>`;
	enum :ref:`TEXT_PIC_TYPE<doxid-namespace_q_panda_1afc58110f73ad7ce75b10a2030ff338b8>`;
	enum :ref:`TransFormType<doxid-namespace_q_panda_1a5f9863b9f685c15e539744e808edde8b>`;
	enum :ref:`UccType<doxid-namespace_q_panda_1a7f68ed9ecff5c30e9105f9cf9ac259ba>`;

	// structs

	struct :ref:`Dist<doxid-struct_q_panda_1_1_dist>`;
	struct :ref:`GataFuncInfo<doxid-struct_q_panda_1_1_gata_func_info>`;
	struct :ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>`;
	struct :ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`;
	struct :ref:`QGatesTransform<doxid-struct_q_panda_1_1_q_gates_transform>`;
	struct :ref:`QGraphItem<doxid-struct_q_panda_1_1_q_graph_item>`;
	struct :ref:`QOptimizationResult<doxid-struct_q_panda_1_1_q_optimization_result>`;
	struct :ref:`QPosition<doxid-struct_q_panda_1_1_q_position>`;
	struct :ref:`QScanPara<doxid-struct_q_panda_1_1_q_scan_para>`;
	struct :ref:`QTwoPara<doxid-struct_q_panda_1_1_q_two_para>`;
	struct :ref:`QubitPointerCmp<doxid-struct_q_panda_1_1_qubit_pointer_cmp>`;
	struct :ref:`RegParamInfo<doxid-struct_q_panda_1_1_reg_param_info>`;
	struct :ref:`SequenceNode<doxid-struct_q_panda_1_1_sequence_node>`;
	struct :ref:`_blocked_matrix<doxid-struct_q_panda_1_1__blocked__matrix>`;
	struct :ref:`_matrix_block<doxid-struct_q_panda_1_1__matrix__block>`;
	struct :ref:`axis<doxid-struct_q_panda_1_1axis>`;
	struct :ref:`edge<doxid-struct_q_panda_1_1edge>`;
	struct :ref:`gate<doxid-struct_q_panda_1_1gate>`;
	struct :ref:`node<doxid-struct_q_panda_1_1node>`;
	struct :ref:`node_cmp<doxid-struct_q_panda_1_1node__cmp>`;

	// classes

	class :ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`;
	class :ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`;

	template <typename... Args>
	class :ref:`AbstractHandleNodes<doxid-class_q_panda_1_1_abstract_handle_nodes>`;

	class :ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`;
	class :ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`;
	class :ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`;
	class :ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`;
	class :ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`;
	class :ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`;
	class :ref:`AdjacentQGates<doxid-class_q_panda_1_1_adjacent_q_gates>`;
	class :ref:`Brent<doxid-class_q_panda_1_1_brent>`;
	class :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`;
	class :ref:`CBitFactory<doxid-class_q_panda_1_1_c_bit_factory>`;
	class :ref:`CBitFactoryHelper<doxid-class_q_panda_1_1_c_bit_factory_helper>`;
	class :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`;
	class :ref:`CExprFactory<doxid-class_q_panda_1_1_c_expr_factory>`;
	class :ref:`CExprFactoryHelper<doxid-class_q_panda_1_1_c_expr_factory_helper>`;
	class :ref:`CMem<doxid-class_q_panda_1_1_c_mem>`;
	class :ref:`CMemFactory<doxid-class_q_panda_1_1_c_mem_factory>`;
	class :ref:`CMemFactoryHelper<doxid-class_q_panda_1_1_c_mem_factory_helper>`;
	class :ref:`CPUQVM<doxid-class_q_panda_1_1_c_p_u_q_v_m>`;
	class :ref:`CPUSingleThreadQVM<doxid-class_q_panda_1_1_c_p_u_single_thread_q_v_m>`;
	class :ref:`CancelControlQubitVector<doxid-class_q_panda_1_1_cancel_control_qubit_vector>`;
	class :ref:`ChemiQ<doxid-class_q_panda_1_1_chemi_q>`;
	class :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`;
	class :ref:`ClassicalProg<doxid-class_q_panda_1_1_classical_prog>`;
	class :ref:`ClassicalProgFactory<doxid-class_q_panda_1_1_classical_prog_factory>`;
	class :ref:`ClassicalProgRegisterAction<doxid-class_q_panda_1_1_classical_prog_register_action>`;
	class :ref:`ConfigMap<doxid-class_q_panda_1_1_config_map>`;
	class :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`;
	class :ref:`DecomposeControlSingleQGateIntoMetadataDoubleQGate<doxid-class_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate>`;
	class :ref:`DecomposeControlUnitarySingleQGate<doxid-class_q_panda_1_1_decompose_control_unitary_single_q_gate>`;
	class :ref:`DecomposeDoubleQGate<doxid-class_q_panda_1_1_decompose_double_q_gate>`;
	class :ref:`DecomposeMultipleControlQGate<doxid-class_q_panda_1_1_decompose_multiple_control_q_gate>`;
	class :ref:`DecomposeUnitarySingleQGateIntoMetadataSingleQGate<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate>`;
	class :ref:`DeleteUnitQNode<doxid-class_q_panda_1_1_delete_unit_q_node>`;
	class :ref:`DoubleGateTypeValidator<doxid-class_q_panda_1_1_double_gate_type_validator>`;
	class :ref:`DrawBox<doxid-class_q_panda_1_1_draw_box>`;
	class :ref:`DrawByLayer<doxid-class_q_panda_1_1_draw_by_layer>`;
	class :ref:`DrawPicture<doxid-class_q_panda_1_1_draw_picture>`;
	class :ref:`DrawQProg<doxid-class_q_panda_1_1_draw_q_prog>`;
	class :ref:`Exp<doxid-class_q_panda_1_1_exp>`;

	template <class T>
	class :ref:`FermionOp<doxid-class_q_panda_1_1_fermion_op>`;

	class :ref:`FillLayerByNextLayerNodes<doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes>`;
	class :ref:`FillQProg<doxid-class_q_panda_1_1_fill_q_prog>`;
	class :ref:`GPUQVM<doxid-class_q_panda_1_1_g_p_u_q_v_m>`;
	class :ref:`GetAllNodeType<doxid-class_q_panda_1_1_get_all_node_type>`;
	class :ref:`GetUsedQubits<doxid-class_q_panda_1_1_get_used_qubits>`;
	class :ref:`GraphDijkstra<doxid-class_q_panda_1_1_graph_dijkstra>`;
	class :ref:`GraphMatch<doxid-class_q_panda_1_1_graph_match>`;
	class :ref:`HadamardQCircuit<doxid-class_q_panda_1_1_hadamard_q_circuit>`;
	class :ref:`IdealMachineInterface<doxid-class_q_panda_1_1_ideal_machine_interface>`;
	class :ref:`IdealQVM<doxid-class_q_panda_1_1_ideal_q_v_m>`;
	class :ref:`Item<doxid-class_q_panda_1_1_item>`;
	class :ref:`JudgeTwoNodeIterIsSwappable<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable>`;
	class :ref:`MergeSingleGate<doxid-class_q_panda_1_1_merge_single_gate>`;
	class :ref:`MetadataValidity<doxid-class_q_panda_1_1_metadata_validity>`;
	class :ref:`MultiPrecisionMachineInterface<doxid-class_q_panda_1_1_multi_precision_machine_interface>`;
	class :ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`;
	class :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`;
	class :ref:`NoiseQVM<doxid-class_q_panda_1_1_noise_q_v_m>`;
	class :ref:`OptimizerFactory<doxid-class_q_panda_1_1_optimizer_factory>`;
	class :ref:`OriginCBit<doxid-class_q_panda_1_1_origin_c_bit>`;
	class :ref:`OriginCExpr<doxid-class_q_panda_1_1_origin_c_expr>`;
	class :ref:`OriginCMem<doxid-class_q_panda_1_1_origin_c_mem>`;
	class :ref:`OriginCircuit<doxid-class_q_panda_1_1_origin_circuit>`;
	class :ref:`OriginClassicalProg<doxid-class_q_panda_1_1_origin_classical_prog>`;
	class :ref:`OriginCollection<doxid-class_q_panda_1_1_origin_collection>`;
	class :ref:`OriginIRVisitor<doxid-class_q_panda_1_1_origin_i_r_visitor>`;
	class :ref:`OriginItem<doxid-class_q_panda_1_1_origin_item>`;
	class :ref:`OriginMeasure<doxid-class_q_panda_1_1_origin_measure>`;
	class :ref:`OriginNelderMead<doxid-class_q_panda_1_1_origin_nelder_mead>`;
	class :ref:`OriginPhysicalQubit<doxid-class_q_panda_1_1_origin_physical_qubit>`;
	class :ref:`OriginPowell<doxid-class_q_panda_1_1_origin_powell>`;
	class :ref:`OriginProgram<doxid-class_q_panda_1_1_origin_program>`;
	class :ref:`OriginQGate<doxid-class_q_panda_1_1_origin_q_gate>`;
	class :ref:`OriginQIf<doxid-class_q_panda_1_1_origin_q_if>`;
	class :ref:`OriginQMachineStatus<doxid-class_q_panda_1_1_origin_q_machine_status>`;
	class :ref:`OriginQResult<doxid-class_q_panda_1_1_origin_q_result>`;
	class :ref:`OriginQWhile<doxid-class_q_panda_1_1_origin_q_while>`;
	class :ref:`OriginQubit<doxid-class_q_panda_1_1_origin_qubit>`;
	class :ref:`OriginQubitPool<doxid-class_q_panda_1_1_origin_qubit_pool>`;
	class :ref:`OriginQubitPoolv2<doxid-class_q_panda_1_1_origin_qubit_poolv2>`;
	class :ref:`OriginReset<doxid-class_q_panda_1_1_origin_reset>`;
	class :ref:`PartialAmplitudeGraph<doxid-class_q_panda_1_1_partial_amplitude_graph>`;
	class :ref:`PartialAmplitudeQVM<doxid-class_q_panda_1_1_partial_amplitude_q_v_m>`;

	template <class T>
	class :ref:`PauliOp<doxid-class_q_panda_1_1_pauli_op>`;

	class :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`;
	class :ref:`PhysicalQubitFactory<doxid-class_q_panda_1_1_physical_qubit_factory>`;
	class :ref:`PhysicalQubitFactoryHelper<doxid-class_q_panda_1_1_physical_qubit_factory_helper>`;
	class :ref:`PickUpNodes<doxid-class_q_panda_1_1_pick_up_nodes>`;
	class :ref:`Psi4Wrapper<doxid-class_q_panda_1_1_psi4_wrapper>`;
	class :ref:`QAOA<doxid-class_q_panda_1_1_q_a_o_a>`;
	class :ref:`QASMToQProg<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog>`;
	class :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`;
	class :ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`;
	class :ref:`QGate<doxid-class_q_panda_1_1_q_gate>`;
	class :ref:`QGateCompare<doxid-class_q_panda_1_1_q_gate_compare>`;
	class :ref:`QGateCounter<doxid-class_q_panda_1_1_q_gate_counter>`;
	class :ref:`QGateNodeFactory<doxid-class_q_panda_1_1_q_gate_node_factory>`;
	class :ref:`QGateParseMap<doxid-class_q_panda_1_1_q_gate_parse_map>`;
	class :ref:`QIfFactory<doxid-class_q_panda_1_1_q_if_factory>`;
	class :ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog>`;
	class :ref:`QIfRegisterAction<doxid-class_q_panda_1_1_q_if_register_action>`;
	class :ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`;
	class :ref:`QMachineStatusFactory<doxid-class_q_panda_1_1_q_machine_status_factory>`;
	class :ref:`QMachineTypeTarnfrom<doxid-class_q_panda_1_1_q_machine_type_tarnfrom>`;
	class :ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>`;
	class :ref:`QNode<doxid-class_q_panda_1_1_q_node>`;
	class :ref:`QNodeDeepCopy<doxid-class_q_panda_1_1_q_node_deep_copy>`;
	class :ref:`QObject<doxid-class_q_panda_1_1_q_object>`;
	class :ref:`QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`;
	class :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`;
	class :ref:`QProgBuilder<doxid-class_q_panda_1_1_q_prog_builder>`;
	class :ref:`QProgClockCycle<doxid-class_q_panda_1_1_q_prog_clock_cycle>`;
	class :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`;
	class :ref:`QProgDataParse<doxid-class_q_panda_1_1_q_prog_data_parse>`;
	class :ref:`QProgExecution<doxid-class_q_panda_1_1_q_prog_execution>`;
	class :ref:`QProgFlattening<doxid-class_q_panda_1_1_q_prog_flattening>`;
	class :ref:`QProgStored<doxid-class_q_panda_1_1_q_prog_stored>`;
	class :ref:`QProgToDAG<doxid-class_q_panda_1_1_q_prog_to_d_a_g>`;
	class :ref:`QProgToMatrix<doxid-class_q_panda_1_1_q_prog_to_matrix>`;
	class :ref:`QProgToOriginIR<doxid-class_q_panda_1_1_q_prog_to_origin_i_r>`;
	class :ref:`QProgToQASM<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m>`;
	class :ref:`QProgToQCircuit<doxid-class_q_panda_1_1_q_prog_to_q_circuit>`;
	class :ref:`QProgToQGate<doxid-class_q_panda_1_1_q_prog_to_q_gate>`;
	class :ref:`QProgToQMeasure<doxid-class_q_panda_1_1_q_prog_to_q_measure>`;
	class :ref:`QProgToQuil<doxid-class_q_panda_1_1_q_prog_to_quil>`;
	class :ref:`QReset<doxid-class_q_panda_1_1_q_reset>`;
	class :ref:`QResetFactory<doxid-class_q_panda_1_1_q_reset_factory>`;
	class :ref:`QResult<doxid-class_q_panda_1_1_q_result>`;
	class :ref:`QResultFactory<doxid-class_q_panda_1_1_q_result_factory>`;
	class :ref:`QResultFactoryHelper<doxid-class_q_panda_1_1_q_result_factory_helper>`;
	class :ref:`QRunesToQProg<doxid-class_q_panda_1_1_q_runes_to_q_prog>`;
	class :ref:`QString<doxid-class_q_panda_1_1_q_string>`;
	class :ref:`QVM<doxid-class_q_panda_1_1_q_v_m>`;
	class :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`;
	class :ref:`QWhileFactory<doxid-class_q_panda_1_1_q_while_factory>`;
	class :ref:`QWhileProg<doxid-class_q_panda_1_1_q_while_prog>`;
	class :ref:`QWhileRegisterAction<doxid-class_q_panda_1_1_q_while_register_action>`;
	class :ref:`QuantumCircuitFactory<doxid-class_q_panda_1_1_quantum_circuit_factory>`;
	class :ref:`QuantumCircuitRegisterAction<doxid-class_q_panda_1_1_quantum_circuit_register_action>`;
	class :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`;
	class :ref:`QuantumMachineFactory<doxid-class_q_panda_1_1_quantum_machine_factory>`;
	class :ref:`QuantumMachineFactoryHelper<doxid-class_q_panda_1_1_quantum_machine_factory_helper>`;
	class :ref:`QuantumMeasureFactory<doxid-class_q_panda_1_1_quantum_measure_factory>`;
	class :ref:`QuantumMeasureRegisterAction<doxid-class_q_panda_1_1_quantum_measure_register_action>`;
	class :ref:`QuantumMetadata<doxid-class_q_panda_1_1_quantum_metadata>`;
	class :ref:`QuantumProgramFactory<doxid-class_q_panda_1_1_quantum_program_factory>`;
	class :ref:`QuantumProgramRegisterAction<doxid-class_q_panda_1_1_quantum_program_register_action>`;
	class :ref:`QuantumResetRegisterAction<doxid-class_q_panda_1_1_quantum_reset_register_action>`;
	class :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`;
	class :ref:`QubitAddr<doxid-class_q_panda_1_1_qubit_addr>`;
	class :ref:`QubitFactory<doxid-class_q_panda_1_1_qubit_factory>`;
	class :ref:`QubitFactoryHelper<doxid-class_q_panda_1_1_qubit_factory_helper>`;
	class :ref:`QubitPool<doxid-class_q_panda_1_1_qubit_pool>`;
	class :ref:`QubitPoolFactory<doxid-class_q_panda_1_1_qubit_pool_factory>`;
	class :ref:`QubitPoolFactoryHelper<doxid-class_q_panda_1_1_qubit_pool_factory_helper>`;
	class :ref:`QubitReference<doxid-class_q_panda_1_1_qubit_reference>`;
	class :ref:`QubitReferenceInterface<doxid-class_q_panda_1_1_qubit_reference_interface>`;
	class :ref:`RJson<doxid-class_q_panda_1_1_r_json>`;
	class :ref:`SingleAmplitudeQVM<doxid-class_q_panda_1_1_single_amplitude_q_v_m>`;
	class :ref:`SingleGateTypeValidator<doxid-class_q_panda_1_1_single_gate_type_validator>`;
	class :ref:`TimeSequenceConfig<doxid-class_q_panda_1_1_time_sequence_config>`;
	class :ref:`TopologyMatch<doxid-class_q_panda_1_1_topology_match>`;
	class :ref:`TransformByCNOT<doxid-class_q_panda_1_1_transform_by_c_n_o_t>`;
	class :ref:`TransformByCZ<doxid-class_q_panda_1_1_transform_by_c_z>`;
	class :ref:`TransformByISWAP<doxid-class_q_panda_1_1_transform_by_i_s_w_a_p>`;
	class :ref:`TransformBySWAP<doxid-class_q_panda_1_1_transform_by_s_w_a_p>`;
	class :ref:`TransformDecomposition<doxid-class_q_panda_1_1_transform_decomposition>`;
	class :ref:`TransformQGateType<doxid-class_q_panda_1_1_transform_q_gate_type>`;
	class :ref:`TransformSwapAlg<doxid-class_q_panda_1_1_transform_swap_alg>`;
	class :ref:`TransformSwapAlgFactory<doxid-class_q_panda_1_1_transform_swap_alg_factory>`;
	class :ref:`Traversal<doxid-class_q_panda_1_1_traversal>`;
	class :ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`;

	template <typename... Args>
	class :ref:`TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`;

	class :ref:`TraverseByNodeIter<doxid-class_q_panda_1_1_traverse_by_node_iter>`;
	class :ref:`TryToMergeTimeSequence<doxid-class_q_panda_1_1_try_to_merge_time_sequence>`;
	class :ref:`Wire<doxid-class_q_panda_1_1_wire>`;
	class :ref:`XmlConfigParam<doxid-class_q_panda_1_1_xml_config_param>`;
	class :ref:`calloc_fail<doxid-class_q_panda_1_1calloc__fail>`;
	class :ref:`complex_var<doxid-class_q_panda_1_1complex__var>`;
	class :ref:`gate_alloc_fail<doxid-class_q_panda_1_1gate__alloc__fail>`;
	class :ref:`init_fail<doxid-class_q_panda_1_1init__fail>`;
	class :ref:`qalloc_fail<doxid-class_q_panda_1_1qalloc__fail>`;
	class :ref:`qcircuit_construction_fail<doxid-class_q_panda_1_1qcircuit__construction__fail>`;
	class :ref:`qprog_construction_fail<doxid-class_q_panda_1_1qprog__construction__fail>`;
	class :ref:`qprog_syntax_error<doxid-class_q_panda_1_1qprog__syntax__error>`;
	class :ref:`qvm_attributes_error<doxid-class_q_panda_1_1qvm__attributes__error>`;
	class :ref:`result_get_fail<doxid-class_q_panda_1_1result__get__fail>`;
	class :ref:`run_fail<doxid-class_q_panda_1_1run__fail>`;
	class :ref:`undefine_error<doxid-class_q_panda_1_1undefine__error>`;

	// global variables

	const std::map<std::string, size_t> :target:`g_kAtomElectrons<doxid-namespace_q_panda_1a4cb28451a9e0cc205901508065549cff>`;
	static std::map<std::string, std::function<double(double, double)>> :target:`_binary_operation<doxid-namespace_q_panda_1af66a1d039b083b3769af218048178fba>`;
	const unsigned short :target:`kUshortMax<doxid-namespace_q_panda_1a68dd96c18f3b06c25555036e9c52eb50>`;
	const int :target:`kCountMoveBit<doxid-namespace_q_panda_1a889ec7a7fbc231bda91e2b80d9fce93d>`;
	const int :ref:`kInfinite<doxid-namespace_q_panda_1ac9fc71c9a8eeab90084ef39bbcf3d1b9>`;
	const int :ref:`kError<doxid-namespace_q_panda_1a5412d3664a88fc95732e34ff8dd4cd57>`;

	// global functions

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t :ref:`getElectronNum<doxid-group___chemi_q_1ga02b35349588cbecff66ed7b11df23836>`(const std::string& atom);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`JordanWignerTransform<doxid-group___chemi_q_1gabe3d00970e6051f8fa3b1723ce700625>`(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`JordanWignerTransform<doxid-group___chemi_q_1gaa35e415e385783eec78f5b8f0b6bc70b>`(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermion);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`JordanWignerTransform<doxid-group___chemi_q_1ga380e66e8e43918dbf73a0690bef5e9f5>`(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`ParityTransform<doxid-group___chemi_q_1gaf59314f2325b2fcde54820e67c5da280>`(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item, size_t maxqubit);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`ParityTransform<doxid-group___chemi_q_1gaff1de62492b7cc268d8781bd53209cd3>`(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermio);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`ParityTransform<doxid-group___chemi_q_1gaa4e7311a00586689562edc4d0078cb8b>`(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` std::vector<Eigen::MatrixXi> :ref:`BKMatrix<doxid-group___chemi_q_1ga91de3b2612b1bbacc6b33ac13466632b>`(size_t qn);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`BravyiKitaevTransform<doxid-group___chemi_q_1ga1ce91fc2dab3957e73c6aa3f7b327885>`(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item, size_t maxqubit, std::vector<Eigen::MatrixXi> BK);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`BravyiKitaevTransform<doxid-namespace_q_panda_1afedd09bfbf8604cc573d0f1aa18235fe>`(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermion, std::vector<Eigen::MatrixXi> BK);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`BravyiKitaevTransform<doxid-group___chemi_q_1ga4bc6e42d8e1587c1b99c85218e79b0df>`(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion, std::vector<Eigen::MatrixXi> BK);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t :ref:`getCCS_N_Trem<doxid-group___chemi_q_1ga1e525807937cc2fb95224ba97872c6ec>`(size_t qn, size_t en);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t :ref:`getCCSD_N_Trem<doxid-group___chemi_q_1gabe33b2e96c7837abf24a9026d3fb9476>`(size_t qn, size_t en);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` :ref:`getCCS<doxid-group___chemi_q_1ga2dee7304bfeecd7a50d85a2e6c7c910c>`(size_t qn, size_t en, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para_vec);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`getCCS<doxid-group___chemi_q_1ga24061dcef88f99903c778485d0b79e0e>`(size_t qn, size_t en, :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`getCCS<doxid-group___chemi_q_1ga14ad05ec8598381b3ae4719810e279f1>`(size_t qn, size_t en, std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` :ref:`getCCSD<doxid-group___chemi_q_1ga4eace51dd20fd3c5878174e6e3c95a59>`(size_t qn, size_t en, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para_vec);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`getCCSD<doxid-group___chemi_q_1ga5fd9958db5f1b82d4e10de9298b1a340>`(size_t qn, size_t en, :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`getCCSD<doxid-group___chemi_q_1ga05b705ee2069c55b9c13781634f2b0f6>`(size_t qn, size_t en, std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`transCC2UCC<doxid-group___chemi_q_1ga59ff6451901ac75cfce2308a8c9becc6>`(const :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`& cc);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`transCC2UCC<doxid-group___chemi_q_1gaae2511f96ce8c475dd606b1dbe279c82>`(const :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`& cc);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` :ref:`simulateHamiltonian<doxid-group___chemi_q_1gac65531ce19de3b5766bc33b1dca2c014>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`& pauli, double t, size_t slices);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` :ref:`simulateOneTerm<doxid-group___chemi_q_1ga97962c33b3af98a7a1e25d9ba716e82e>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, const :ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`& hamiltonian_term, const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& coef, double t);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` :ref:`simulateZTerm<doxid-group___chemi_q_1gadf8fdd11093b481f74988c0330591a63>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& coef, double t);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` :ref:`parsePsi4DataToFermion<doxid-group___chemi_q_1ga4995c648e2dc98bbb2344483ac2b31ab>`(const std::string& data);

	bool :target:`operator <<doxid-namespace_q_panda_1a63d976778f52af47db0cb2ae4d8d314c>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p2
		);

	bool :target:`operator <<doxid-namespace_q_panda_1a216658e7a2c03a04c757c7dbbffca6ef>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const double& coef
		);

	bool :target:`operator <=<doxid-namespace_q_panda_1aa2b39b9c0997df72288b31aa0cd2e3b6>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p2
		);

	bool :target:`operator <=<doxid-namespace_q_panda_1a84967f5bda8d683d86b5d6bc5e2ae5f1>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const double& coef
		);

	bool :target:`operator ><doxid-namespace_q_panda_1a6c3fddd96d45ff1d41152f55c2757c49>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p2
		);

	bool :target:`operator >=<doxid-namespace_q_panda_1a6440753a0e7c0fb8d526113b2d96a7ef>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p2
		);

	double :target:`operator -<doxid-namespace_q_panda_1a53215f5f198f8c5c2d13950f140da059>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p2
		);

	double :target:`operator +<doxid-namespace_q_panda_1a9c396087b03515c16c4b1b53b9d9ea6d>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p1,
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p2
		);

	double :target:`operator *<doxid-namespace_q_panda_1a7985644e05e299cab239eef14ad499cb>` (
		const double& coef,
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p
		);

	double :target:`operator *<doxid-namespace_q_panda_1a5c454816fce94caa60f1fad06a021256>` (
		const :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`& p,
		const double& coef
		);

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`simulateZTerm<doxid-group___hamiltonian_simulation_1ga366679393b4da372cae09336afd5bd85>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, double coef, double t);

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`simulateOneTerm<doxid-group___hamiltonian_simulation_1ga671d3f9e4f7405c92a4dd67e2caefa09>`(
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec,
		const :ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`& hamiltonian_term,
		double coef,
		double t
		);

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`simulateHamiltonian<doxid-group___hamiltonian_simulation_1ga45d2c199bcacd1c45488aba60b4f294e>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>`& hamiltonian, double t, size_t slices);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`simulatePauliZHamiltonian<doxid-group___hamiltonian_simulation_1gaee4eac1151b17cb8cbcba893284087bd>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>`& hamiltonian, double t);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`applySingleGateToAll<doxid-group___hamiltonian_simulation_1ga16d8ca96691e3f00aa30436cede022b7>`(const std::string& gate, const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec);
	void :ref:`applySingleGateToAll<doxid-group___hamiltonian_simulation_1ga5d07ddf5202fafc04e5682f77bf29b72>`(const std::string& gate, const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`ising_model<doxid-group___hamiltonian_simulation_1ga6d49c4b9b3a175a3f2645ababc7258f9>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`QGraph<doxid-namespace_q_panda_1ae453b3fa92a6aec65ebb5c554d47f1e5>`& graph, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& gamma);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`pauliX_model<doxid-group___hamiltonian_simulation_1ga92c972b836c6e0d2168656608437988b>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& beta);
	double :ref:`vector_dot<doxid-group___max_cut_problem_generator_1gaabca13165ac231f4d1432a127051fcae>`(std::vector<double>& x, std::vector<double>& y);

	double :ref:`all_cut_of_graph<doxid-group___max_cut_problem_generator_1ga86d1510c5d9a68fa500efc1a696749e4>`(
		std::vector<std::vector<double>> adjacent_matrix,
		std::vector<double>& all_cut_list,
		std::vector<size_t>& target_value_list
		);

	bool :ref:`init<doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>`(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type = :ref:`CPU<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13aea39cfc1ace612a8e2c4da2c62ae5659>`);
	void :ref:`finalize<doxid-group___core_1gacd2f5cfc79160543f03c5bef34d27185>`();
	:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`qAlloc<doxid-group___core_1ga9a81705d142b143260f86f742adf0d86>`();
	:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`qAlloc<doxid-group___core_1ga2a307b5ad8cdee51c52bdbf0d299e509>`(size_t stQubitAddr);
	std::map<std::string, bool> :ref:`directlyRun<doxid-group___core_1ga65ef685dd053d017b2f9e48f38c03370>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg);
	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`qAllocMany<doxid-group___core_1ga9dcf62b20ef64d5b561e7919e7903a97>`(size_t stQubitNumber);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`cAlloc<doxid-group___core_1ga5fcf81bd208ecf4ba4e53249599fdb4d>`();
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`cAlloc<doxid-group___core_1ga792cdfc228747df979116019ab869dca>`(size_t stCBitaddr);
	std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`cAllocMany<doxid-group___core_1ga820833650151100c4a29aafc2f345863>`(size_t stCBitNumber);
	void :ref:`cFree<doxid-group___core_1ga95bc1fb6ac649bd590680a2676e71ea6>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&);
	void :ref:`cFreeAll<doxid-group___core_1gaa438f340325085ab44936e0413c2d40d>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> vCBit);
	:ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* :ref:`getstat<doxid-group___core_1ga2dcbb445a1e5c3b5cdec9b44e1325096>`();
	size_t :ref:`getAllocateQubitNum<doxid-group___core_1ga9f99c54c66e54057d1f635b0bf4ed26e>`();
	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`getProbTupleList<doxid-group___core_1ga9f7eb33268e651402871173ad289f201>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`getProbList<doxid-group___core_1ga37ce2c0c342a9dce0293c31412179e56>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`getProbDict<doxid-group___core_1gac7d6f9130bb14da46068f669cbeb786f>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`probRunTupleList<doxid-group___core_1ga940377aac8c4e06aa93b6d9ad1ca44c6>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`probRunList<doxid-group___core_1ga8b769442bdd06bce0bd573dfa0b86125>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`probRunDict<doxid-group___core_1gaad2d0834f62ae9c4b18573c7e8a50922>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-group___core_1gaac240d65f6c9c0e955a583b7d7a7735b>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, int);
	std::map<std::string, size_t> :ref:`quickMeasure<doxid-group___core_1gaaaf64d793f51d39ead7ceba1cf7d6d01>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`accumulateProbability<doxid-group___core_1gab7fa40c4a3d8d4b6c9dc5a5bf389162f>`(:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& prob_list);

	std::map<std::string, size_t> :ref:`quick_measure<doxid-group___core_1gabbf7eea831182a82092f70285c027d42>`(
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector,
		int shots,
		:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& accumulate_probabilites
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-group___core_1gacaafce8fec4c04e15a492fb695176bb1>`();
	:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* :ref:`initQuantumMachine<doxid-group___core_1gab28a403fe4f2894e330ccd90e01295e4>`(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type = :ref:`CPU<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13aea39cfc1ace612a8e2c4da2c62ae5659>`);
	void :ref:`destroyQuantumMachine<doxid-group___core_1ga40086744d5e1d0ee04381ebd63ae40c7>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm);
	:ref:`QPanda::QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`MeasureAll<doxid-group___core_1ga5d448b1c38b2b3a13022c5c3a3587b40>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`transformOriginIRToQProg<doxid-group___utilities_1ga6c05a9faf342cc818885312391c779a5>`(std::string filePath, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`convert_originir_to_qprog<doxid-group___utilities_1gaac2060fa16ef56111baae96c504dc5e3>`(std::string file_path, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`convert_originir_string_to_qprog<doxid-group___utilities_1ga663bf50e836b485b1681d99140e262e1>`(std::string str_originir, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`convert_qasm_to_qprog<doxid-group___utilities_1ga58cc63a9077019716862a43ecdf0f82c>`(std::string file_path, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm);
	size_t :target:`getAllocateCMem<doxid-namespace_q_panda_1ad435d1a0c920566388c51081f1e3c9c6>`();

	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`PMeasure<doxid-namespace_q_panda_1a07805971399f768521716b88ea7a8169>`(
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector,
		int select_max
		);

	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`PMeasure_no_index<doxid-namespace_q_panda_1aea06168ff9630a5cf458575e8555947d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector);
	size_t :ref:`getAllocateCMemNum<doxid-group___core_1gaa455e0e99622f5f997c6931981bb33ea>`();
	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`pMeasure<doxid-group___core_1ga3c19a648c8c21b9b8819b1c8180f20c0>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector, int select_max);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`pMeasureNoIndex<doxid-group___core_1ga44c86a2a14f084483580f898a70e6a20>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator +<doxid-namespace_q_panda_1a79f9ba0093102c6960f516287b008a46>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator +<doxid-namespace_q_panda_1aded49dbb459e1f542d1280eb8397e49f>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` right_operand);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator +<doxid-namespace_q_panda_1aa8cedabac34fe21ae12b018e42baf768>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` right_operand);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator -<doxid-namespace_q_panda_1a5fec65b0613f12a6f06fd2965a01d26b>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` right_operand);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator -<doxid-namespace_q_panda_1a8d5fea538033ed9d3ac24401aa14e087>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` right_operand);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator -<doxid-namespace_q_panda_1ac5923717dd7d1a73d01f92871810c00a>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator *<doxid-namespace_q_panda_1ac6a456742e3549447b5e8bb19fd72b36>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator *<doxid-namespace_q_panda_1a18356d1a02aa870b69d0c5f915e84069>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator *<doxid-namespace_q_panda_1a6fab8cd22d0e5e4478b16b6196bc29ce>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator/<doxid-namespace_q_panda_1af85c9ed743b10e12397b3b4104d1225c>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator/<doxid-namespace_q_panda_1a74a5972004b3c74a1261bd4968bdbd30>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator/<doxid-namespace_q_panda_1a17cd104975ee9939997dad2c86785dfb>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator ==<doxid-namespace_q_panda_1aa9297f3e011a704952923a239ed485e6>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator ==<doxid-namespace_q_panda_1a22eae2f3c1f05e1fee911486b7a7fa4e>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator ==<doxid-namespace_q_panda_1ae4ffce30cd5834bfa72cf60791e43ac2>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator !=<doxid-namespace_q_panda_1afa028caf35a9d9e084dbd9afa8e264fe>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator !=<doxid-namespace_q_panda_1ae7aa69e58e9f257d5f07bbad7560115f>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator !=<doxid-namespace_q_panda_1ac28a7de2c7ade1c51a36590f4046b4fc>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator &&<doxid-namespace_q_panda_1a0622629da6582f9db3b4859db6e9c71d>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator &&<doxid-namespace_q_panda_1a146832792072501ef6f8c69f9394fd8a>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator &&<doxid-namespace_q_panda_1ae3cc8a3d921c0d9ca686f3c3deb04606>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator||<doxid-namespace_q_panda_1a90c5d18d15b8e3fe96ef21f38eff1ee9>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator||<doxid-namespace_q_panda_1a1b70c6c23572784848a181f2309a4d78>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator||<doxid-namespace_q_panda_1a55ca90e077299a68ef87191540cc086a>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator ><doxid-namespace_q_panda_1acf5b980b8cfd9452873c985f67806811>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator ><doxid-namespace_q_panda_1a00e9365fb4e4f165aa62225e4cc9ba8b>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator ><doxid-namespace_q_panda_1a5f1847279db90cc7f6c8f2d961962c5b>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator >=<doxid-namespace_q_panda_1a00bdd8d5aa2957ea3fc00b9795d87d87>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator >=<doxid-namespace_q_panda_1a8966318840d7a56babd9c266c4c9af62>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator >=<doxid-namespace_q_panda_1a5ff46a34486693c3ca936313cde32c84>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator <<doxid-namespace_q_panda_1ad854327d50cdac2935994d88729b0839>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator <<doxid-namespace_q_panda_1a76d5f1bf63f25f024dc5270f39f8665f>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator <<doxid-namespace_q_panda_1a5851cfdf3eaed882d2778100f0e4fa51>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator <=<doxid-namespace_q_panda_1a695273f4329fcab26841425707e6e658>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator <=<doxid-namespace_q_panda_1a4ccd295b1fcbda29af2683acc49f4fa2>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator <=<doxid-namespace_q_panda_1ae650e6b11b8821ac1127be8eda6f77d0>` (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`operator !<doxid-namespace_q_panda_1ac1b69a3a29906767c863d992c1cd1f0c>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);

	:ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog>` :target:`CreateIfProg<doxid-namespace_q_panda_1a93709bbafb1c6c826163e7cbac44da61>`(
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node
		);

	:ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog>` :target:`CreateIfProg<doxid-namespace_q_panda_1a86122f95eb0d2e6c8b17dcef57d93a3e>`(
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_condition,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` false_node
		);

	:ref:`QWhileProg<doxid-class_q_panda_1_1_q_while_prog>` :target:`CreateWhileProg<doxid-namespace_q_panda_1a17626d7f89c3f51a78343f2d2376e7ce>`(
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` trueNode
		);

	:ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog>` :ref:`createIfProg<doxid-group___quantum_circuit_1ga690686c448897c743b39344efd3a2635>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` cc, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node);
	:ref:`QIfProg<doxid-class_q_panda_1_1_q_if_prog>` :ref:`createIfProg<doxid-group___quantum_circuit_1gac3b1d1883da275951d60ab75be41c8f8>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` cc, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` false_node);
	:ref:`QWhileProg<doxid-class_q_panda_1_1_q_while_prog>` :ref:`createWhileProg<doxid-group___quantum_circuit_1ga9b163c962fe2929ba69f38e28dee1e00>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` cc, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`CreateEmptyCircuit<doxid-namespace_q_panda_1a496ade517171ec5855bf1ad6be455163>`();
	:ref:`HadamardQCircuit<doxid-class_q_panda_1_1_hadamard_q_circuit>` :target:`CreateHadamardQCircuit<doxid-namespace_q_panda_1ab3864bf9ee3f084900448304f082cccb>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& pQubitVector);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`createEmptyCircuit<doxid-group___quantum_circuit_1ga93edfc442e07f17d304fc5532bce9f27>`();
	:ref:`HadamardQCircuit<doxid-class_q_panda_1_1_hadamard_q_circuit>` :ref:`createHadamardQCircuit<doxid-group___quantum_circuit_1ga760c74090f1b930c58a143f986e9046a>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& pQubitVector);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`I<doxid-group___quantum_circuit_1ga420edded52b644d85416c1cb878edb38>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`X<doxid-group___quantum_circuit_1ga64ee2bc42f9e7f1a7d27ec70efc4073e>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`X1<doxid-group___quantum_circuit_1ga7b5a0450074e01e5933e47e62faeea47>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`RX<doxid-group___quantum_circuit_1ga20fe3265a85bc707131f82bdad8a3ae3>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, double angle);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`U1<doxid-group___quantum_circuit_1ga0636e14563f5f60c42f3cd841b796821>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, double angle);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`U2<doxid-group___quantum_circuit_1gaa952ca3b1d8d35cf80105d990a3fb577>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit, double phi, double lambda);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`U3<doxid-group___quantum_circuit_1gab90f69275f15eea2223adf26486a54b6>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit, double theta, double phi, double lambda);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`Y<doxid-group___quantum_circuit_1gac495b5f125f5b881baa360830808bb29>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`Y1<doxid-group___quantum_circuit_1ga62ca170907611ac249d186d4ecc0bc3d>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`RY<doxid-group___quantum_circuit_1gae11dc10d7b2482ea2c3d3edf08674725>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, double angle);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`Z<doxid-group___quantum_circuit_1gae9f4f72d036a731903e9cd26c80702f9>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`Z1<doxid-group___quantum_circuit_1ga74a5df4e01a0ee3c611579e4fa0b0263>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`RZ<doxid-group___quantum_circuit_1ga40387ee9be69126efd039bf27bd99c4d>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, double angle);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`S<doxid-group___quantum_circuit_1ga783130fd86b04a4117356e7f2889ee79>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`H<doxid-group___quantum_circuit_1ga1a443031d0f938174e0bf28ffca71090>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`CNOT<doxid-group___quantum_circuit_1gacb08d7c792208de29a5be63b2a3c56a5>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`CZ<doxid-group___quantum_circuit_1ga7cac8e053b8f27d7454c309c11d63c05>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`U4<doxid-group___quantum_circuit_1gae9a8b5d4ae321720900196e7b3d64a80>`(double alpha, double beta, double gamma, double delta, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`U4<doxid-group___quantum_circuit_1gaf19109d7e8a9ef242fa801d7f87a0425>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`QDouble<doxid-group___quantum_circuit_1ga48274d9c8be0e07e8199327862848fa6>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit1, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qubit2);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`CU<doxid-group___quantum_circuit_1ga7ec1e35e939877c8ca64be7f1cf27571>`(double alpha, double beta, double gamma, double delta, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`CU<doxid-group___quantum_circuit_1ga05c90f9ef40613e8305f2279c0d10d50>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`iSWAP<doxid-namespace_q_panda_1a8ec185e6e71d8677a8c67a1a7da94961>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_fisrt, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_second);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`iSWAP<doxid-group___quantum_circuit_1gadc2cef7687d02928a866519f1a91d41c>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_fisrt, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_second, double theta);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`CR<doxid-group___quantum_circuit_1gafe5a2234741c39e2c13c104249a48c9a>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targit_qubit, double theta);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`SqiSWAP<doxid-group___quantum_circuit_1ga9f5b46f53bcbb46da139cc46d3c93ca8>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_fisrt, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_second);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`SWAP<doxid-group___quantum_circuit_1gab20d995e1b986584d78a915585011da2>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_fisrt, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_second);

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :target:`oracle<doxid-namespace_q_panda_1aca81172ac9118b18e3e6e1afe5a6ff36>`(
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubits,
		std::string oracle_name
		);

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :target:`copy_qgate<doxid-namespace_q_panda_1af28e34b38637ae249216aae19e48a9f1>`(
		:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* qgate_old,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector
		);

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :target:`copy_qgate<doxid-namespace_q_panda_1a2cb487fdeaed0cdb55264af3a2e8c495>`(
		:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& qgate,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector
		);

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :target:`copy_qgate<doxid-namespace_q_panda_1a33da7cdf61acf74919d98aba874942d5>`(
		:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`* qgate,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector
		);

	template <typename _Ty>
	_Ty :ref:`deepCopy<doxid-group___quantum_circuit_1ga5cbebca719de8665deb5b54a6a8dbcea>`(_Ty& node);

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`CreateEmptyQProg<doxid-namespace_q_panda_1aa7d29b1b76f27d94a6698fe3cf08090e>`();
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`createEmptyQProg<doxid-group___quantum_circuit_1ga5af30111cb3b8e0c745cf36de80e2d8e>`();
	:ref:`QReset<doxid-class_q_panda_1_1_q_reset>` :ref:`Reset<doxid-group___quantum_circuit_1gaa7f97690f18c8da7fda06f3d9d2f13e9>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
	:ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` :ref:`Measure<doxid-group___core_1ga15b15ba85d24d7355880ad63fd4c2107>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);
	std::string :ref:`qProgToBinary<doxid-group___quantum_machine_1gab866832e6095f21fe98f8ec7cae1bfab>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*);
	void :ref:`execute_qprog<doxid-group___quantum_machine_1ga3c31a727dcc23d3c9a918a4ec8441522>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu, :ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param);

	bool :target:`loadIBMQuantumTopology<doxid-namespace_q_panda_1a5960f65e11f3b6d435243a908c1b9fe2>`(
		const std::string& xmlStr,
		const std::string& backendName,
		int& qubitsCnt,
		std::vector<std::vector<int>>& vec
		);

	bool :target:`binaryQProgFileParse<doxid-namespace_q_panda_1a0fe60adeac67c5f4b7839be990d2c783>`(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::string& filename,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		);

	bool :target:`binaryQProgDataParse<doxid-namespace_q_panda_1a3c33f0aceffa982e7dfecec808bc72cf>`(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::vector<uint8_t>& data,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		);

	bool :ref:`transformBinaryDataToQProg<doxid-group___utilities_1ga126fbcaac23e41abf1cd661028cc9f57>`(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::vector<uint8_t>& data,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		);

	bool :ref:`transformBinaryDataToQProg<doxid-group___utilities_1ga284d5b244a500b2103933ba318433455>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);

	bool :ref:`convert_binary_data_to_qprog<doxid-group___utilities_1ga964bc45fa95994092d40d3df1fee947d>`(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::vector<uint8_t>& data,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		);

	bool :ref:`convert_binary_data_to_qprog<doxid-group___utilities_1gae732643b9f76756d4cbd21b52b9ee49a>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	std::vector<uint8_t> :ref:`transformQProgToBinary<doxid-group___utilities_1gab977f2314768f84df494fc726b269957>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);

	void :target:`storeQProgInBinary<doxid-namespace_q_panda_1a60aa47d7c1cb1990a5ab03d9899eb890>`(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::string& filename
		);

	void :ref:`transformQProgToBinary<doxid-group___utilities_1gae59f3170912283e6f2912778bda63a4d>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename);
	std::vector<uint8_t> :ref:`convert_qprog_to_binary<doxid-group___utilities_1gac91ac2b0027e3eb2f08ae86a1fc5201e>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	void :ref:`convert_qprog_to_binary<doxid-group___utilities_1gaa5d087d0a28e6d87372ad75f6a3ae010>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename);

	template <typename _Ty>
	std::string :ref:`transformQProgToOriginIR<doxid-group___utilities_1gac85a4be007c80a0c9bcac301414797c3>`(_Ty& node, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine);

	template <typename _Ty>
	std::string :ref:`convert_qprog_to_originir<doxid-group___utilities_1ga139b35c89a0f7882bc77200bcf3e7b08>`(_Ty& node, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine);

	std::string :ref:`transformQProgToQASM<doxid-group___utilities_1gaa13be205f3f69ecf28d1d7759bdd8461>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& pQProg, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine, :ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` ibmBackend = :ref:`IBMQ_QASM_SIMULATOR<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8ca09728e1eb958bbe0ec92174a7ce111cd>`);
	std::string :ref:`convert_qprog_to_qasm<doxid-group___utilities_1ga2f95b62aff4c3ae3bbeac669bc64ec82>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, :ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` ibmBackend = :ref:`IBMQ_QASM_SIMULATOR<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8ca09728e1eb958bbe0ec92174a7ce111cd>`);
	std::string :ref:`transformQProgToQuil<doxid-group___utilities_1ga1afab9eb4d36a2758e559b40f63e82cc>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine);
	std::string :ref:`convert_qprog_to_quil<doxid-group___utilities_1ga6ba609a5a9659c9247464add93496ccb>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`transformQRunesToQProg<doxid-group___utilities_1ga1f9755f387cd30e9ac65ea502269f908>`(std::string, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*);
	int :ref:`arbitraryRotationMetadataValidity<doxid-group___utilities_1ga785ac4c99106792eb8c00392e5576104>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`doubleContinuousMetadataValidity<doxid-group___utilities_1gac4ba5476ec612a6f63122f9c33ccfbd8>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`singleContinuousAndDiscreteMetadataValidity<doxid-group___utilities_1ga429a2bcbd0f51f6a5560bcb088c10e1e>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`doubleDiscreteMetadataValidity<doxid-group___utilities_1ga5534bc47fbbbf2ccd5bd994feeebfd6a>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`doubleGateMetadataValidity<doxid-group___utilities_1gaceaea9db4f27bd09e4930b2ffa2fdfb5>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`validateSingleQGateType<doxid-group___utilities_1ga0d5aad0edcc57eae1140ca91bf50bb5e>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`validateDoubleQGateType<doxid-namespace_q_panda_1a9cbe217c5ed732b605e0b9bf6fe862c7>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	bool :ref:`isMatchTopology<doxid-group___utilities_1ga459114e3940a2ff0128cf51ca92f98ca>`(const :ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate, const std::vector<std::vector<int>>& vecTopoSt);
	std::string :ref:`getAdjacentQGateType<doxid-group___utilities_1ga0adcec3f1d6e1cb173e5afadc3aac5ab>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr, std::vector<:ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`>& adjacentNodes);
	bool :ref:`isSwappable<doxid-group___utilities_1ga18c8e4e48c21b6901eb93bd05e40ea30>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr1, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr2);
	bool :ref:`isSupportedGateType<doxid-group___utilities_1ga28afe2b7d347e24df633c81ebb0d8ff1>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr);
	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getCircuitMatrix<doxid-group___utilities_1gaecf3d5fffaaa40080b612fed1cd9d975>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` srcProg, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrStart = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(), const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrEnd = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`());

	void :ref:`pickUpNode<doxid-group___utilities_1ga8484fc54a5cab80edc24654cc68201e1>`(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& outPutProg,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& srcProg,
		const std::vector<:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`> reject_node_types,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrStart = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrEnd = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		bool bDagger = false
		);

	void :ref:`get_all_used_qubits<doxid-group___utilities_1ga60e9de7c80e617edb5f326689625a0c5>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, std::vector<int>& vecQuBitsInUse);

	void :target:`get_all_used_qubits<doxid-namespace_q_panda_1a87279012c2e2d7a20d8bcfcc0b81f174>`(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vecQuBitsInUse
		);

	void :ref:`get_all_used_class_bits<doxid-group___utilities_1gaaf010d547364709f49981078bf40cfae>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, std::vector<int>& vecClBitsInUse);
	std::string :ref:`printAllNodeType<doxid-group___utilities_1gae41e9802e11fe16be10a56819e6c6709>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	void :ref:`get_gate_parameter<doxid-group___utilities_1ga79406ec5a5ba912ce1675534c4ed9366>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> pGate, std::string& para_str);

	template <typename _Ty>
	size_t :target:`getUnSupportQGateNumber<doxid-namespace_q_panda_1a94332811af460accd8755c4588335818>`(
		_Ty node,
		const std::vector<std::vector<std::string>>& gates
		);

	template <typename _Ty>
	size_t :ref:`getUnsupportQGateNum<doxid-namespace_q_panda_1a33cbad3ede8ec096606f502b412ddc54>`(
		_Ty node,
		const std::vector<std::vector<std::string>>& gates
		);

	template <typename _Ty>
	size_t :target:`getQGateNumber<doxid-namespace_q_panda_1ad29015acb67f99bc608cdc35685d62ed>`(_Ty& node);

	template <typename _Ty>
	size_t :ref:`getQGateNum<doxid-group___utilities_1gaa2167d6194906299c48b50228436f367>`(_Ty& node);

	size_t :ref:`getQProgClockCycle<doxid-group___utilities_1ga002a279e27f4843dbadd82c19553cdc1>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	std::string :ref:`UnicodeToUTF8<doxid-namespace_q_panda_1a2f8937555b21b0f5386dd1b9600d5fff>`(const std::wstring& wstr);
	std::wstring :ref:`utf8ToWstring<doxid-namespace_q_panda_1a6faca68de87292f58a9610c14319c6a6>`(const std::string& str);
	std::string :ref:`ulongToUtf8<doxid-namespace_q_panda_1ab1858b9fa9df505290bfc2fbbc4a8340>`(unsigned long val);
	void :ref:`initConsole<doxid-namespace_q_panda_1ad53087d7c6fb017694c54a34aad3ca5e>`();
	std::string :ref:`draw_qprog<doxid-group___utilities_1ga5b68a36676155a7e2413fa1f2c3c02d2>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_start = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(), const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_end = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`());
	std::string :ref:`draw_qprog_with_clock<doxid-group___utilities_1ga9729586010920bb1c7035ab3b207f119>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_start = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(), const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_end = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`());
	std::ostream& :ref:`operator <<<doxid-group___utilities_1gae4df8ff2e43a6a8ad196b3fe1ab31208>` (std::ostream& out, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);

	template <typename _Ty1, typename _Ty2, typename _Ty3>
	void :ref:`graph_query_replace<doxid-group___utilities_1gaa5d7f420dbaf504df35d77e11dc27313>`(
		_Ty1& graph_node,
		_Ty2& query_node,
		_Ty3& replace_node,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
		);

	template <typename _Ty1, typename _Ty2>
	bool :ref:`graph_query<doxid-group___utilities_1gae94b1400c910547de03936bc91a94214>`(
		_Ty1& graph_node,
		_Ty2& query_node,
		:ref:`ResultVector<doxid-namespace_q_panda_1a960ac3f5e928f3a42f4d2f2191320897>`& query_result
		);

	static bool :ref:`cast_qprog_qcircuit<doxid-group___utilities_1gab6fa6a562c8f53d3e1a07ceae99c46d1>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit);
	static :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`cast_qprog_qgate<doxid-group___utilities_1gafe6ca010315b8926648f71f591e04e6c>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);
	static :ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` :ref:`cast_qprog_qmeasure<doxid-group___utilities_1gaeca0972f111c64634cafdffb628dcbed>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`topology_match<doxid-group___utilities_1ga378f5da8f88411621aa9f364db018746>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine, :ref:`SwapQubitsMethod<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73>` method = :ref:`CNOT_GATE_METHOD<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73af0fd6c0d21b2b49d98160f724cff9cbe>`, :ref:`ArchType<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2a>` arch_type = :ref:`IBM_QX5_ARCH<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2aa1d998a495737ef4502e83b080f3dada0>`);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`fill_qprog_by_I<doxid-group___utilities_1ga44d0898c5b799ae5d5a61885bb843019>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& input_prog);
	void :ref:`flatten<doxid-group___utilities_1ga997126df699b036f29971b65d91f7720>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	void :ref:`flatten<doxid-group___utilities_1ga4ec2bd572ad776b199ed47e9c21ac049>`(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit);
	void :ref:`full_flatten<doxid-group___utilities_1gafbdb42f53bdf318319bbc3b2ff2dce46>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	bool :target:`isPerfectSquare<doxid-namespace_q_panda_1a4693edaa029c35f62a669042301e3e21>`(int number);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator +<doxid-namespace_q_panda_1aa1a52b0d7f0478bba3e817268c8997c4>` (
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator +<doxid-namespace_q_panda_1ac8403207ee727397353cd9ddb7480109>` (
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` value
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator +<doxid-namespace_q_panda_1a1eb37e79e9e7117fa651f1f42934c218>` (
		const :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` value,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator -<doxid-namespace_q_panda_1afb49aeda45ad5ad88e250f2dc642ef2c>` (
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator -<doxid-namespace_q_panda_1a01fd9b03853490fe834dc0efb76edd70>` (
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`& value
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator -<doxid-namespace_q_panda_1a9fc0db9d644c82110faf7da2019a9274>` (
		const :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`& value,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator *<doxid-namespace_q_panda_1a09a1e38685425e28558ef3a8d2f2daeb>` (
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator *<doxid-namespace_q_panda_1a792ce92e31ee1e34a49293fdfc02bfde>` (
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_left,
		const :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`& value
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`operator *<doxid-namespace_q_panda_1a23b964a8148302d67bae5b19b92e4041>` (
		const :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`& value,
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix_right
		);

	std::ostream& :target:`operator <<<doxid-namespace_q_panda_1aa550c479692708ecbe1d9dea766d6e71>` (
		std::ostream& out,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& mat
		);

	int :ref:`partition<doxid-group___utilities_1ga34e90d38e9f219c3633ddba0d1ca5b8f>`(
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& srcMatrix,
		int partitionRowNum,
		int partitionColumnNum,
		:ref:`blockedMatrix_t<doxid-namespace_q_panda_1a8f8db55e468baa3e5febdb847979eadc>`& blockedMat
		);

	int :ref:`blockMultip<doxid-group___utilities_1ga332ecf657ba1ac5c4817ce9abf280557>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& leftMatrix, const :ref:`blockedMatrix_t<doxid-namespace_q_panda_1a8f8db55e468baa3e5febdb847979eadc>`& blockedMat, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& resultMatrix);
	void :ref:`dagger<doxid-group___utilities_1gad7d29837687e202f654217bdc72c861e>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& srcMat);
	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`tensor<doxid-group___utilities_1ga89e38fe6a988250608482e752ca15853>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& leftMatrix, const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& rightMatrix);
	std::string :ref:`matrix_to_string<doxid-group___utilities_1ga4ade7ce8fa33b32b51559cd3689a6459>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& mat);

	std::string :target:`dec2bin<doxid-namespace_q_panda_1aec6984ada1cb1ac1785608b27fe9a4bb>`(
		unsigned n,
		size_t size
		);

	double :target:`RandomNumberGenerator<doxid-namespace_q_panda_1a602485ddcf8cb10d9ef3a0d2307a0f52>`();

	void :target:`add_up_a_map<doxid-namespace_q_panda_1a236eec682560af8ba1f837d7415abc1d>`(
		std::map<std::string, size_t>& meas_result,
		std::string key
		);

	void :target:`insertQCircuit<doxid-namespace_q_panda_1aa2817cdb0b95406da48723d0aec4bc36>`(
		:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`* pGateNode,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& qCircuit,
		:ref:`QNode<doxid-class_q_panda_1_1_q_node>`* pParentNode
		);

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`Reset_Qubit_Circuit<doxid-namespace_q_panda_1a8688d288b927322c0f48e72761378607>`(
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* q,
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& cbit,
		bool setVal
		);

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`Reset_Qubit<doxid-namespace_q_panda_1a1e731b2d10d51bb61c9a7e512160d2c8>`(
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* q,
		bool setVal,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
		);

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`Reset_All<doxid-namespace_q_panda_1ac0cf4b681f9fb782ad82a13620ace05e>`(
		std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> qubit_vector,
		bool setVal,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
		);

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`parityCheckCircuit<doxid-group___utilities_1ga45bce8581a43de45a3bbf5b3c7cbafcd>`(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> qubit_vec);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`apply_QGate<doxid-group___utilities_1ga296d3416ba243601d3939bb960284d97>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubits, std::function<:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)> gate);

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`applyQGate<doxid-namespace_q_panda_1a699476ba07fb96ce1973339df54349df>`(
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubits,
		std::function<:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)> gate
		);

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`Toffoli<doxid-group___utilities_1ga360ff2641ae0d9229ff920de8050fadf>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qc1, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qc2, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target);
	std::vector<std::string> :ref:`split<doxid-group___utilities_1gad46a951a6cfb7b6339415f05686a80f4>`(const std::string& str, const std::string& delim);
	bool :ref:`str2int<doxid-group___utilities_1ga5ea0e3dbc8f13d4acf35ae04e30633c6>`(std::string s, long long& num);
	bool :ref:`str2double<doxid-group___utilities_1gab6004f2bad15ec13d4f40d3ab35c3979>`(std::string s, double& num);
	std::string :ref:`ll2str<doxid-group___utilities_1ga94d1661951a9556739e9c890275c421b>`(long long num);
	std::string :ref:`int2str<doxid-group___utilities_1ga4ba82eb2f8ee44b6bbe7387295f47e46>`(int num);
	std::string :ref:`double2str<doxid-group___utilities_1gabcdf63fbfaf0af391fbce6dca1a932c7>`(double num);

	bool :target:`parse_oracle_name<doxid-namespace_q_panda_1a715127012f0839078dd279c34ba974c6>`(
		std::string rawname,
		std::string& oraclename,
		std::vector<size_t>& qubits
		);

	std::string :target:`generate_oracle_name<doxid-namespace_q_panda_1a7359d6b06c01b1d90b59ca47c4e07631>`(
		std::string oraclename,
		std::vector<size_t> qubits
		);

	double :target:`argc<doxid-namespace_q_panda_1a97a3eacc50b9c372c98f59a838792142>`(:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` num);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`bernsteinVaziraniAlgorithm<doxid-group___b___v___algorithm_1ga9fddd471931a1b3590405d5caf32151f>`(std::string stra, bool b, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`BV_Oracle<doxid-namespace_q_panda_1ae77eda567be203be8fc4bbe4102358f0>` oracle);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`deutschJozsaAlgorithm<doxid-group___d_j___algorithm_1ga5ee04d03753fbd09dffd803716552f58>`(std::vector<bool> boolean_function, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`DJ_Oracle<doxid-namespace_q_panda_1a128c4092d904b9f5b0ee5b6fc6e25a95>` oracle);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`groverAlgorithm<doxid-group___grover___algorithm_1gaca53d0d6f02da195f90cf87f4f7c1a05>`(size_t target, size_t search_range, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`grover_oracle<doxid-namespace_q_panda_1a11c0bf85de02b818d471d9dc2997ad30>` oracle);

	} // namespace QPanda
.. _details-namespace_q_panda:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPanda2 base namespace.

Typedefs
--------

.. index:: pair: typedef; QTerm
.. _doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::map<size_t, char> QTerm

The QTerm value char only will be 'X','Y','Z'. If QTerm is empty it reperents 'I'.

.. index:: pair: typedef; MetadataValidity_cb
.. _doxid-namespace_q_panda_1a702b41a7cbaaed0e602ffdd3f2511317:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<int(std::vector<std::string>&, std::vector<std::string>&)> MetadataValidity_cb

typedef MetadataValidity_cb that add all functions of metadata validity

Global Variables
----------------

.. index:: pair: variable; kInfinite
.. _doxid-namespace_q_panda_1ac9fc71c9a8eeab90084ef39bbcf3d1b9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const int kInfinite

Int infinite.

.. index:: pair: variable; kError
.. _doxid-namespace_q_panda_1a5412d3664a88fc95732e34ff8dd4cd57:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const int kError

Error identifier.

Global Functions
----------------

.. index:: pair: function; BravyiKitaevTransform
.. _doxid-namespace_q_panda_1afedd09bfbf8604cc573d0f1aa18235fe:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` BravyiKitaevTransform(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermion, std::vector<Eigen::MatrixXi> BK)

BravyiKitaev transform from FermionOperator to PauliOperator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- FermionOperator&

		- fermion operator

	*
		- std::vector<Eigen::MatrixXi>

		- BK



.. rubric:: Returns:

PauliOperator



.. rubric:: See also:

:ref:`FermionOperator <doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; operator+
.. _doxid-namespace_q_panda_1a79f9ba0093102c6960f516287b008a46:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator + (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator +.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- :ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator+
.. _doxid-namespace_q_panda_1aded49dbb459e1f542d1280eb8397e49f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator + (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` right_operand)

Uverload operator +.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator+
.. _doxid-namespace_q_panda_1aa8cedabac34fe21ae12b018e42baf768:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator + (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` right_operand)

Overload operator +.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator-
.. _doxid-namespace_q_panda_1a5fec65b0613f12a6f06fd2965a01d26b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator - (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` right_operand)

Overload operator -.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator-
.. _doxid-namespace_q_panda_1a8d5fea538033ed9d3ac24401aa14e087:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator - (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` left_operand, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` right_operand)

Overload operator -.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator-
.. _doxid-namespace_q_panda_1ac5923717dd7d1a73d01f92871810c00a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator - (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator -.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator*
.. _doxid-namespace_q_panda_1ac6a456742e3549447b5e8bb19fd72b36:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator * (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator \*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator*
.. _doxid-namespace_q_panda_1a18356d1a02aa870b69d0c5f915e84069:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator * (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator \*.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator*
.. _doxid-namespace_q_panda_1a6fab8cd22d0e5e4478b16b6196bc29ce:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator * (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator -.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator/
.. _doxid-namespace_q_panda_1af85c9ed743b10e12397b3b4104d1225c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator/ (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator /.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator/
.. _doxid-namespace_q_panda_1a74a5972004b3c74a1261bd4968bdbd30:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator/ (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator /.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator/
.. _doxid-namespace_q_panda_1a17cd104975ee9939997dad2c86785dfb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator/ (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator /.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator==
.. _doxid-namespace_q_panda_1aa9297f3e011a704952923a239ed485e6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator == (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator ==.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator==
.. _doxid-namespace_q_panda_1a22eae2f3c1f05e1fee911486b7a7fa4e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator == (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator ==.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator==
.. _doxid-namespace_q_panda_1ae4ffce30cd5834bfa72cf60791e43ac2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator == (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator ==.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator!=
.. _doxid-namespace_q_panda_1afa028caf35a9d9e084dbd9afa8e264fe:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator != (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator !=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator!=
.. _doxid-namespace_q_panda_1ae7aa69e58e9f257d5f07bbad7560115f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator != (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator !=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator!=
.. _doxid-namespace_q_panda_1ac28a7de2c7ade1c51a36590f4046b4fc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator != (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_cond)

Overload operator !=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator&&
.. _doxid-namespace_q_panda_1a0622629da6582f9db3b4859db6e9c71d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator && (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator &&.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator&&
.. _doxid-namespace_q_panda_1a146832792072501ef6f8c69f9394fd8a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator && (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator &&.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator&&
.. _doxid-namespace_q_panda_1ae3cc8a3d921c0d9ca686f3c3deb04606:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator && (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_cond)

Overload operator &&.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator||
.. _doxid-namespace_q_panda_1a90c5d18d15b8e3fe96ef21f38eff1ee9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator|| (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator \|\|.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator||
.. _doxid-namespace_q_panda_1a1b70c6c23572784848a181f2309a4d78:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator|| (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator \|\|.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator||
.. _doxid-namespace_q_panda_1a55ca90e077299a68ef87191540cc086a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator|| (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` classical_cond)

Overload operator \|\|.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator>
.. _doxid-namespace_q_panda_1acf5b980b8cfd9452873c985f67806811:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator > (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator >



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator>
.. _doxid-namespace_q_panda_1a00e9365fb4e4f165aa62225e4cc9ba8b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator > (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator >



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator>
.. _doxid-namespace_q_panda_1a5f1847279db90cc7f6c8f2d961962c5b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator > (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator >



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator>=
.. _doxid-namespace_q_panda_1a00bdd8d5aa2957ea3fc00b9795d87d87:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator >= (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator >=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator>=
.. _doxid-namespace_q_panda_1a8966318840d7a56babd9c266c4c9af62:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator >= (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator >=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator>=
.. _doxid-namespace_q_panda_1a5ff46a34486693c3ca936313cde32c84:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator >= (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator >=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator<
.. _doxid-namespace_q_panda_1ad854327d50cdac2935994d88729b0839:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator < (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator <.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator<
.. _doxid-namespace_q_panda_1a76d5f1bf63f25f024dc5270f39f8665f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator < (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator <.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator<
.. _doxid-namespace_q_panda_1a5851cfdf3eaed882d2778100f0e4fa51:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator < (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator <.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator<=
.. _doxid-namespace_q_panda_1a695273f4329fcab26841425707e6e658:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator <= (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator <=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator<=
.. _doxid-namespace_q_panda_1a4ccd295b1fcbda29af2683acc49f4fa2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator <= (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`, :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Overload operator <=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- left_operand

		- left operand

	*
		- right_operand

		- cbit_size_t type right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator<=
.. _doxid-namespace_q_panda_1ae650e6b11b8821ac1127be8eda6f77d0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator <= (:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` class_cond)

Overload operator <=.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- cbit_size_t type left operand

	*
		- class_cond

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator!
.. _doxid-namespace_q_panda_1ac1b69a3a29906767c863d992c1cd1f0c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` operator ! (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

Overload operator !



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- right_operand

		- right operand



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; iSWAP
.. _doxid-namespace_q_panda_1a8ec185e6e71d8677a8c67a1a7da94961:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` iSWAP(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_fisrt, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* targitBit_second)

Construct a new quantum iSWAP gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- control qubit

	*
		- Qubit\*

		- target qubit



.. rubric:: Returns:

:ref:`QPanda::QGate <doxid-class_q_panda_1_1_q_gate>` quantum gate

.. index:: pair: function; validateDoubleQGateType
.. _doxid-namespace_q_panda_1a9cbe217c5ed732b605e0b9bf6fe862c7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int validateDoubleQGateType(
		std::vector<std::string>& gates,
		std::vector<std::string>& valid_gates
		)

Verify the validity of double quantum gates.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<std::string>&

		- the gates is judged

	*
		- std::vector<std::string>&

		- output the valid gates



.. rubric:: Returns:

int double quantum gate type

.. index:: pair: function; getUnsupportQGateNum
.. _doxid-namespace_q_panda_1a33cbad3ede8ec096606f502b412ddc54:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty>
	size_t getUnsupportQGateNum(
		_Ty node,
		const std::vector<std::vector<std::string>>& gates
		)

Count quantum program unsupported gate numner.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty&

		- quantum program, quantum circuit, quantum while or quantum if

	*
		- const

		- std::vector<std::vector<std::string>>& support gates



.. rubric:: Returns:

size_t Unsupported :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` number

.. index:: pair: function; UnicodeToUTF8
.. _doxid-namespace_q_panda_1a2f8937555b21b0f5386dd1b9600d5fff:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string UnicodeToUTF8(const std::wstring& wstr)

convert unicode string to UTF8 string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::wstring&

		- the source wstring encoded by Unicode



.. rubric:: Returns:

string Converted String

.. index:: pair: function; utf8ToWstring
.. _doxid-namespace_q_panda_1a6faca68de87292f58a9610c14319c6a6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::wstring utf8ToWstring(const std::string& str)

convert UTF8 string to wide string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- the source string



.. rubric:: Returns:

wstring Converted wide String

.. index:: pair: function; ulongToUtf8
.. _doxid-namespace_q_panda_1ab1858b9fa9df505290bfc2fbbc4a8340:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string ulongToUtf8(unsigned long val)

convert unsigned long to string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- unsigned long

		- the source val



.. rubric:: Returns:

std::string Converted string

.. index:: pair: function; initConsole
.. _doxid-namespace_q_panda_1ad53087d7c6fb017694c54a34aad3ca5e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void initConsole()

set windows console to utf-8 encode

