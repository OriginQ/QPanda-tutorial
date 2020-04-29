.. index:: pair: group; Utilities
.. _doxid-group___utilities:

Utilities
=========

.. toctree::
	:hidden:

	class_QPanda_AdjacentQGates.rst
	class_QPanda_CancelControlQubitVector.rst
	class_QPanda_ConfigMap.rst
	class_QPanda_DecomposeControlUnitarySingleQGate.rst
	class_QPanda_DecomposeDoubleQGate.rst
	class_QPanda_DecomposeMultipleControlQGate.rst
	class_QPanda_DecomposeUnitarySingleQGateIntoMetadataSingleQGate.rst
	class_DeleteUnitQnode.rst
	class_QPanda_DoubleGateTypeValidator.rst
	class_QPanda_DrawQProg.rst
	class_QPanda_Exp.rst
	class_QPanda_FillQProg.rst
	class_QPanda_GetAllNodeType.rst
	class_QPanda_GraphDijkstra.rst
	class_QPanda_GraphMatch.rst
	class_QPanda_MergeSingleGate.rst
	class_QPanda_MetadataValidity.rst
	class_QPanda_NodeInfo.rst
	class_QPanda_OriginIRVisitor.rst
	class_QPanda_QASMToQProg.rst
	class_QPanda_QCircuitParam.rst
	class_QPanda_QGateCompare.rst
	class_QPanda_QGateCounter.rst
	class_QPanda_QPandaException.rst
	class_QPanda_QProgBuilder.rst
	class_QPanda_QProgClockCycle.rst
	class_QPanda_QProgDAG.rst
	class_QPanda_QProgDataParse.rst
	class_QPanda_QProgFlattening.rst
	class_QPanda_QProgStored.rst
	class_QPanda_QProgToMatrix.rst
	class_QPanda_QProgToOriginIR.rst
	class_QPanda_QProgToQASM.rst
	class_QPanda_QProgToQCircuit.rst
	class_QPanda_QProgToQGate.rst
	class_QPanda_QProgToQMeasure.rst
	class_QPanda_QProgToQuil.rst
	class_QPanda_QRunesToQProg.rst
	class_QPanda_QString.rst
	class_QPanda_QuantumMetadata.rst
	class_ReadLock.rst
	class_SharedMutex.rst
	class_QPanda_SingleGateTypeValidator.rst
	class_QPanda_TimeSequenceConfig.rst
	class_QPanda_TopologyMatch.rst
	class_QPanda_TransformByCNOT.rst
	class_QPanda_TransformByCZ.rst
	class_QPanda_TransformByISWAP.rst
	class_QPanda_TransformBySWAP.rst
	class_QPanda_TransformDecomposition.rst
	class_QPanda_TransformQGateType.rst
	class_QPanda_TransformSwapAlg.rst
	class_QPanda_TransformSwapAlgFactory.rst
	class_QPanda_Traversal.rst
	class_QPanda_TraversalConfig.rst
	class_QPanda_TraversalInterface.rst
	class_QPanda_TraverseByNodeIter.rst
	class_WriteLock.rst
	class_QPanda_XmlConfigParam.rst
	class_QPanda_init_fail.rst
	class_QPanda_qalloc_fail.rst
	class_QPanda_qcircuit_construction_fail.rst
	class_QPanda_qprog_construction_fail.rst
	class_QPanda_qprog_syntax_error.rst
	class_QPanda_qvm_attributes_error.rst
	class_QPanda_result_get_fail.rst
	class_QPanda_run_fail.rst
	class_QPanda_undefine_error.rst

Overview
~~~~~~~~

QPanda2 base Utilities classes and interface. :ref:`More...<details-group___utilities>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// classes

	class :ref:`QPanda::AdjacentQGates<doxid-class_q_panda_1_1_adjacent_q_gates>`;
	class :ref:`QPanda::CancelControlQubitVector<doxid-class_q_panda_1_1_cancel_control_qubit_vector>`;
	class :ref:`QPanda::ConfigMap<doxid-class_q_panda_1_1_config_map>`;
	class :ref:`QPanda::DecomposeControlUnitarySingleQGate<doxid-class_q_panda_1_1_decompose_control_unitary_single_q_gate>`;
	class :ref:`QPanda::DecomposeDoubleQGate<doxid-class_q_panda_1_1_decompose_double_q_gate>`;
	class :ref:`QPanda::DecomposeMultipleControlQGate<doxid-class_q_panda_1_1_decompose_multiple_control_q_gate>`;
	class :ref:`QPanda::DecomposeUnitarySingleQGateIntoMetadataSingleQGate<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate>`;
	class :ref:`DeleteUnitQnode<doxid-class_delete_unit_qnode>`;
	class :ref:`QPanda::DoubleGateTypeValidator<doxid-class_q_panda_1_1_double_gate_type_validator>`;
	class :ref:`QPanda::DrawQProg<doxid-class_q_panda_1_1_draw_q_prog>`;
	class :ref:`QPanda::Exp<doxid-class_q_panda_1_1_exp>`;
	class :ref:`QPanda::FillQProg<doxid-class_q_panda_1_1_fill_q_prog>`;
	class :ref:`QPanda::GetAllNodeType<doxid-class_q_panda_1_1_get_all_node_type>`;
	class :ref:`QPanda::GraphDijkstra<doxid-class_q_panda_1_1_graph_dijkstra>`;
	class :ref:`QPanda::GraphMatch<doxid-class_q_panda_1_1_graph_match>`;
	class :ref:`QPanda::MergeSingleGate<doxid-class_q_panda_1_1_merge_single_gate>`;
	class :ref:`QPanda::MetadataValidity<doxid-class_q_panda_1_1_metadata_validity>`;
	class :ref:`QPanda::NodeInfo<doxid-class_q_panda_1_1_node_info>`;
	class :ref:`QPanda::OriginIRVisitor<doxid-class_q_panda_1_1_origin_i_r_visitor>`;
	class :ref:`QPanda::QASMToQProg<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog>`;
	class :ref:`QPanda::QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`;
	class :ref:`QPanda::QGateCompare<doxid-class_q_panda_1_1_q_gate_compare>`;
	class :ref:`QPanda::QGateCounter<doxid-class_q_panda_1_1_q_gate_counter>`;
	class :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`;
	class :ref:`QPanda::QProgBuilder<doxid-class_q_panda_1_1_q_prog_builder>`;
	class :ref:`QPanda::QProgClockCycle<doxid-class_q_panda_1_1_q_prog_clock_cycle>`;
	class :ref:`QPanda::QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`;
	class :ref:`QPanda::QProgDataParse<doxid-class_q_panda_1_1_q_prog_data_parse>`;
	class :ref:`QPanda::QProgFlattening<doxid-class_q_panda_1_1_q_prog_flattening>`;
	class :ref:`QPanda::QProgStored<doxid-class_q_panda_1_1_q_prog_stored>`;
	class :ref:`QPanda::QProgToMatrix<doxid-class_q_panda_1_1_q_prog_to_matrix>`;
	class :ref:`QPanda::QProgToOriginIR<doxid-class_q_panda_1_1_q_prog_to_origin_i_r>`;
	class :ref:`QPanda::QProgToQASM<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m>`;
	class :ref:`QPanda::QProgToQCircuit<doxid-class_q_panda_1_1_q_prog_to_q_circuit>`;
	class :ref:`QPanda::QProgToQGate<doxid-class_q_panda_1_1_q_prog_to_q_gate>`;
	class :ref:`QPanda::QProgToQMeasure<doxid-class_q_panda_1_1_q_prog_to_q_measure>`;
	class :ref:`QPanda::QProgToQuil<doxid-class_q_panda_1_1_q_prog_to_quil>`;
	class :ref:`QPanda::QRunesToQProg<doxid-class_q_panda_1_1_q_runes_to_q_prog>`;
	class :ref:`QPanda::QString<doxid-class_q_panda_1_1_q_string>`;
	class :ref:`QPanda::QuantumMetadata<doxid-class_q_panda_1_1_quantum_metadata>`;
	class :ref:`ReadLock<doxid-class_read_lock>`;
	class :ref:`SharedMutex<doxid-class_shared_mutex>`;
	class :ref:`QPanda::SingleGateTypeValidator<doxid-class_q_panda_1_1_single_gate_type_validator>`;
	class :ref:`QPanda::TimeSequenceConfig<doxid-class_q_panda_1_1_time_sequence_config>`;
	class :ref:`QPanda::TopologyMatch<doxid-class_q_panda_1_1_topology_match>`;
	class :ref:`QPanda::TransformByCNOT<doxid-class_q_panda_1_1_transform_by_c_n_o_t>`;
	class :ref:`QPanda::TransformByCZ<doxid-class_q_panda_1_1_transform_by_c_z>`;
	class :ref:`QPanda::TransformByISWAP<doxid-class_q_panda_1_1_transform_by_i_s_w_a_p>`;
	class :ref:`QPanda::TransformBySWAP<doxid-class_q_panda_1_1_transform_by_s_w_a_p>`;
	class :ref:`QPanda::TransformDecomposition<doxid-class_q_panda_1_1_transform_decomposition>`;
	class :ref:`QPanda::TransformQGateType<doxid-class_q_panda_1_1_transform_q_gate_type>`;
	class :ref:`QPanda::TransformSwapAlg<doxid-class_q_panda_1_1_transform_swap_alg>`;
	class :ref:`QPanda::TransformSwapAlgFactory<doxid-class_q_panda_1_1_transform_swap_alg_factory>`;
	class :ref:`QPanda::Traversal<doxid-class_q_panda_1_1_traversal>`;
	class :ref:`QPanda::TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`;

	template <typename... Args>
	class :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`;

	class :ref:`QPanda::TraverseByNodeIter<doxid-class_q_panda_1_1_traverse_by_node_iter>`;
	class :ref:`WriteLock<doxid-class_write_lock>`;
	class :ref:`QPanda::XmlConfigParam<doxid-class_q_panda_1_1_xml_config_param>`;
	class :ref:`QPanda::init_fail<doxid-class_q_panda_1_1init__fail>`;
	class :ref:`QPanda::qalloc_fail<doxid-class_q_panda_1_1qalloc__fail>`;
	class :ref:`QPanda::qcircuit_construction_fail<doxid-class_q_panda_1_1qcircuit__construction__fail>`;
	class :ref:`QPanda::qprog_construction_fail<doxid-class_q_panda_1_1qprog__construction__fail>`;
	class :ref:`QPanda::qprog_syntax_error<doxid-class_q_panda_1_1qprog__syntax__error>`;
	class :ref:`QPanda::qvm_attributes_error<doxid-class_q_panda_1_1qvm__attributes__error>`;
	class :ref:`QPanda::result_get_fail<doxid-class_q_panda_1_1result__get__fail>`;
	class :ref:`QPanda::run_fail<doxid-class_q_panda_1_1run__fail>`;
	class :ref:`QPanda::undefine_error<doxid-class_q_panda_1_1undefine__error>`;

	// global functions

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::transformOriginIRToQProg<doxid-group___utilities_1ga6c05a9faf342cc818885312391c779a5>`(std::string filePath, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::convert_originir_to_qprog<doxid-group___utilities_1gaac2060fa16ef56111baae96c504dc5e3>`(std::string file_path, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::convert_originir_string_to_qprog<doxid-group___utilities_1ga663bf50e836b485b1681d99140e262e1>`(std::string str_originir, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::convert_qasm_to_qprog<doxid-group___utilities_1ga58cc63a9077019716862a43ecdf0f82c>`(std::string file_path, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm);

	bool :ref:`QPanda::transformBinaryDataToQProg<doxid-group___utilities_1ga126fbcaac23e41abf1cd661028cc9f57>`(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::vector<uint8_t>& data,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		);

	bool :ref:`QPanda::transformBinaryDataToQProg<doxid-group___utilities_1ga284d5b244a500b2103933ba318433455>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);

	bool :ref:`QPanda::convert_binary_data_to_qprog<doxid-group___utilities_1ga964bc45fa95994092d40d3df1fee947d>`(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::vector<uint8_t>& data,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		);

	bool :ref:`QPanda::convert_binary_data_to_qprog<doxid-group___utilities_1gae732643b9f76756d4cbd21b52b9ee49a>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	std::vector<uint8_t> :ref:`QPanda::transformQProgToBinary<doxid-group___utilities_1gab977f2314768f84df494fc726b269957>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	void :ref:`QPanda::transformQProgToBinary<doxid-group___utilities_1gae59f3170912283e6f2912778bda63a4d>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename);
	std::vector<uint8_t> :ref:`QPanda::convert_qprog_to_binary<doxid-group___utilities_1gac91ac2b0027e3eb2f08ae86a1fc5201e>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	void :ref:`QPanda::convert_qprog_to_binary<doxid-group___utilities_1gaa5d087d0a28e6d87372ad75f6a3ae010>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename);

	template <typename _Ty>
	std::string :ref:`QPanda::transformQProgToOriginIR<doxid-group___utilities_1gac85a4be007c80a0c9bcac301414797c3>`(_Ty& node, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine);

	template <typename _Ty>
	std::string :ref:`QPanda::convert_qprog_to_originir<doxid-group___utilities_1ga139b35c89a0f7882bc77200bcf3e7b08>`(_Ty& node, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine);

	std::string :ref:`QPanda::transformQProgToQASM<doxid-group___utilities_1gaa13be205f3f69ecf28d1d7759bdd8461>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& pQProg, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine, :ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` ibmBackend = :ref:`IBMQ_QASM_SIMULATOR<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8ca09728e1eb958bbe0ec92174a7ce111cd>`);
	std::string :ref:`QPanda::convert_qprog_to_qasm<doxid-group___utilities_1ga2f95b62aff4c3ae3bbeac669bc64ec82>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, :ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` ibmBackend = :ref:`IBMQ_QASM_SIMULATOR<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8ca09728e1eb958bbe0ec92174a7ce111cd>`);
	std::string :ref:`QPanda::transformQProgToQuil<doxid-group___utilities_1ga1afab9eb4d36a2758e559b40f63e82cc>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine);
	std::string :ref:`QPanda::convert_qprog_to_quil<doxid-group___utilities_1ga6ba609a5a9659c9247464add93496ccb>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`QPanda::transformQRunesToQProg<doxid-group___utilities_1ga1f9755f387cd30e9ac65ea502269f908>`(std::string, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*);
	int :ref:`QPanda::arbitraryRotationMetadataValidity<doxid-group___utilities_1ga785ac4c99106792eb8c00392e5576104>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`QPanda::doubleContinuousMetadataValidity<doxid-group___utilities_1gac4ba5476ec612a6f63122f9c33ccfbd8>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`QPanda::singleContinuousAndDiscreteMetadataValidity<doxid-group___utilities_1ga429a2bcbd0f51f6a5560bcb088c10e1e>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`QPanda::doubleDiscreteMetadataValidity<doxid-group___utilities_1ga5534bc47fbbbf2ccd5bd994feeebfd6a>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`QPanda::doubleGateMetadataValidity<doxid-group___utilities_1gaceaea9db4f27bd09e4930b2ffa2fdfb5>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	int :ref:`QPanda::validateSingleQGateType<doxid-group___utilities_1ga0d5aad0edcc57eae1140ca91bf50bb5e>`(std::vector<std::string>& gates, std::vector<std::string>& valid_gates);
	bool :ref:`QPanda::isMatchTopology<doxid-group___utilities_1ga459114e3940a2ff0128cf51ca92f98ca>`(const :ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate, const std::vector<std::vector<int>>& vecTopoSt);
	std::string :ref:`QPanda::getAdjacentQGateType<doxid-group___utilities_1ga0adcec3f1d6e1cb173e5afadc3aac5ab>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr, std::vector<:ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`>& adjacentNodes);
	bool :ref:`QPanda::isSwappable<doxid-group___utilities_1ga18c8e4e48c21b6901eb93bd05e40ea30>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr1, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr2);
	bool :ref:`QPanda::isSupportedGateType<doxid-group___utilities_1ga28afe2b7d347e24df633c81ebb0d8ff1>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr);
	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`QPanda::getCircuitMatrix<doxid-group___utilities_1gaecf3d5fffaaa40080b612fed1cd9d975>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` srcProg, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrStart = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(), const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrEnd = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`());

	void :ref:`QPanda::pickUpNode<doxid-group___utilities_1ga8484fc54a5cab80edc24654cc68201e1>`(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& outPutProg,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& srcProg,
		const std::vector<:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`> reject_node_types,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrStart = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrEnd = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		bool bDagger = false
		);

	void :ref:`QPanda::get_all_used_qubits<doxid-group___utilities_1ga60e9de7c80e617edb5f326689625a0c5>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, std::vector<int>& vecQuBitsInUse);
	void :ref:`QPanda::get_all_used_class_bits<doxid-group___utilities_1gaaf010d547364709f49981078bf40cfae>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, std::vector<int>& vecClBitsInUse);
	std::string :ref:`QPanda::printAllNodeType<doxid-group___utilities_1gae41e9802e11fe16be10a56819e6c6709>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	void :ref:`QPanda::get_gate_parameter<doxid-group___utilities_1ga79406ec5a5ba912ce1675534c4ed9366>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> pGate, std::string& para_str);

	template <typename _Ty>
	size_t :ref:`QPanda::getQGateNum<doxid-group___utilities_1gaa2167d6194906299c48b50228436f367>`(_Ty& node);

	size_t :ref:`QPanda::getQProgClockCycle<doxid-group___utilities_1ga002a279e27f4843dbadd82c19553cdc1>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);
	std::string :ref:`QPanda::draw_qprog<doxid-group___utilities_1ga5b68a36676155a7e2413fa1f2c3c02d2>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_start = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(), const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_end = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`());
	std::string :ref:`QPanda::draw_qprog_with_clock<doxid-group___utilities_1ga9729586010920bb1c7035ab3b207f119>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_start = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(), const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_end = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`());
	std::ostream& :ref:`QPanda::operator <<<doxid-group___utilities_1gae4df8ff2e43a6a8ad196b3fe1ab31208>` (std::ostream& out, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);

	template <typename _Ty1, typename _Ty2, typename _Ty3>
	void :ref:`QPanda::graph_query_replace<doxid-group___utilities_1gaa5d7f420dbaf504df35d77e11dc27313>`(
		_Ty1& graph_node,
		_Ty2& query_node,
		_Ty3& replace_node,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
		);

	template <typename _Ty1, typename _Ty2>
	bool :ref:`QPanda::graph_query<doxid-group___utilities_1gae94b1400c910547de03936bc91a94214>`(
		_Ty1& graph_node,
		_Ty2& query_node,
		:ref:`ResultVector<doxid-namespace_q_panda_1a960ac3f5e928f3a42f4d2f2191320897>`& query_result
		);

	static bool :ref:`QPanda::cast_qprog_qcircuit<doxid-group___utilities_1gab6fa6a562c8f53d3e1a07ceae99c46d1>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit);
	static :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`QPanda::cast_qprog_qgate<doxid-group___utilities_1gafe6ca010315b8926648f71f591e04e6c>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);
	static :ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` :ref:`QPanda::cast_qprog_qmeasure<doxid-group___utilities_1gaeca0972f111c64634cafdffb628dcbed>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::topology_match<doxid-group___utilities_1ga378f5da8f88411621aa9f364db018746>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine, :ref:`SwapQubitsMethod<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73>` method = :ref:`CNOT_GATE_METHOD<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73af0fd6c0d21b2b49d98160f724cff9cbe>`, :ref:`ArchType<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2a>` arch_type = :ref:`IBM_QX5_ARCH<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2aa1d998a495737ef4502e83b080f3dada0>`);
	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::fill_qprog_by_I<doxid-group___utilities_1ga44d0898c5b799ae5d5a61885bb843019>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& input_prog);
	void :ref:`QPanda::flatten<doxid-group___utilities_1ga997126df699b036f29971b65d91f7720>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	void :ref:`QPanda::flatten<doxid-group___utilities_1ga4ec2bd572ad776b199ed47e9c21ac049>`(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit);
	void :ref:`QPanda::full_flatten<doxid-group___utilities_1gafbdb42f53bdf318319bbc3b2ff2dce46>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);

	int :ref:`QPanda::partition<doxid-group___utilities_1ga34e90d38e9f219c3633ddba0d1ca5b8f>`(
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& srcMatrix,
		int partitionRowNum,
		int partitionColumnNum,
		:ref:`blockedMatrix_t<doxid-namespace_q_panda_1a8f8db55e468baa3e5febdb847979eadc>`& blockedMat
		);

	int :ref:`QPanda::blockMultip<doxid-group___utilities_1ga332ecf657ba1ac5c4817ce9abf280557>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& leftMatrix, const :ref:`blockedMatrix_t<doxid-namespace_q_panda_1a8f8db55e468baa3e5febdb847979eadc>`& blockedMat, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& resultMatrix);
	void :ref:`QPanda::dagger<doxid-group___utilities_1gad7d29837687e202f654217bdc72c861e>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& srcMat);
	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`QPanda::tensor<doxid-group___utilities_1ga89e38fe6a988250608482e752ca15853>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& leftMatrix, const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& rightMatrix);
	std::string :ref:`QPanda::matrix_to_string<doxid-group___utilities_1ga4ade7ce8fa33b32b51559cd3689a6459>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& mat);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::parityCheckCircuit<doxid-group___utilities_1ga45bce8581a43de45a3bbf5b3c7cbafcd>`(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> qubit_vec);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::apply_QGate<doxid-group___utilities_1ga296d3416ba243601d3939bb960284d97>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubits, std::function<:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)> gate);
	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`QPanda::Toffoli<doxid-group___utilities_1ga360ff2641ae0d9229ff920de8050fadf>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qc1, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qc2, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target);
	std::vector<std::string> :ref:`QPanda::split<doxid-group___utilities_1gad46a951a6cfb7b6339415f05686a80f4>`(const std::string& str, const std::string& delim);
	bool :ref:`QPanda::str2int<doxid-group___utilities_1ga5ea0e3dbc8f13d4acf35ae04e30633c6>`(std::string s, long long& num);
	bool :ref:`QPanda::str2double<doxid-group___utilities_1gab6004f2bad15ec13d4f40d3ab35c3979>`(std::string s, double& num);
	std::string :ref:`QPanda::ll2str<doxid-group___utilities_1ga94d1661951a9556739e9c890275c421b>`(long long num);
	std::string :ref:`QPanda::int2str<doxid-group___utilities_1ga4ba82eb2f8ee44b6bbe7387295f47e46>`(int num);
	std::string :ref:`QPanda::double2str<doxid-group___utilities_1gabcdf63fbfaf0af391fbce6dca1a932c7>`(double num);

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

.. _details-group___utilities:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPanda2 base Utilities classes and interface.

Global Functions
----------------

.. index:: pair: function; transformOriginIRToQProg
.. _doxid-group___utilities_1ga6c05a9faf342cc818885312391c779a5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::transformOriginIRToQProg(std::string filePath, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm)

OriginIR Transform To Quantum Program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- OriginIR file path

	*
		- QuantumMachine\*

		- quantum machine pointer



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>` quantum program

.. index:: pair: function; convert_originir_to_qprog
.. _doxid-group___utilities_1gaac2060fa16ef56111baae96c504dc5e3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::convert_originir_to_qprog(std::string file_path, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm)

Convert OriginIR To Quantum Program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- OriginIR file path

	*
		- QuantumMachine\*

		- quantum machine pointer



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>` quantum program

.. index:: pair: function; convert_originir_string_to_qprog
.. _doxid-group___utilities_1ga663bf50e836b485b1681d99140e262e1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::convert_originir_string_to_qprog(std::string str_originir, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm)

Convert OriginIR String To Quantum Program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- OriginIR String

	*
		- QuantumMachine\*

		- quantum machine pointer



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>` quantum program

.. index:: pair: function; convert_qasm_to_qprog
.. _doxid-group___utilities_1ga58cc63a9077019716862a43ecdf0f82c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::convert_qasm_to_qprog(std::string file_path, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm)

QASM Transform To Quantum Program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- QASM file path

	*
		- QuantumMachine\*

		- quantum machine pointer



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>` quantum program

.. index:: pair: function; transformBinaryDataToQProg
.. _doxid-group___utilities_1ga126fbcaac23e41abf1cd661028cc9f57:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::transformBinaryDataToQProg(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::vector<uint8_t>& data,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		)

Parse quantum program interface for binary data vector.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QuantumMachine\*

		- quantum machine pointer

	*
		- std::vector<uint8_t>&

		- data binary data vector

	*
		- QVec&

		- qubits

	*
		- std::vector<ClassicalCondition>&

		- cbits

	*
		- QProg&

		- Quantum program



.. rubric:: Returns:

bool

.. index:: pair: function; transformBinaryDataToQProg
.. _doxid-group___utilities_1ga284d5b244a500b2103933ba318433455:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::transformBinaryDataToQProg(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::string& filename,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		)

Parse quantum program interface for binary file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QuantumMachine\*

		- quantum machine pointer

	*
		- std::string&

		- binary file name

	*
		- QVec&

		- qubits

	*
		- std::vector<ClassicalCondition>&

		- cbits

	*
		- QProg&

		- Quantum program



.. rubric:: Returns:

bool

.. index:: pair: function; convert_binary_data_to_qprog
.. _doxid-group___utilities_1ga964bc45fa95994092d40d3df1fee947d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::convert_binary_data_to_qprog(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::vector<uint8_t>& data,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		)

Parse quantum program interface for binary data vector.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QuantumMachine\*

		- quantum machine pointer

	*
		- std::vector<uint8_t>&

		- data binary data vector

	*
		- QVec&

		- qubits

	*
		- std::vector<ClassicalCondition>&

		- cbits

	*
		- QProg&

		- Quantum program



.. rubric:: Returns:

bool

.. index:: pair: function; convert_binary_data_to_qprog
.. _doxid-group___utilities_1gae732643b9f76756d4cbd21b52b9ee49a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::convert_binary_data_to_qprog(
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm,
		const std::string& filename,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>& cbits,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		)

Parse quantum program interface for binary file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QuantumMachine\*

		- quantum machine pointer

	*
		- std::string&

		- binary file name

	*
		- QVec&

		- qubits

	*
		- std::vector<ClassicalCondition>&

		- cbits

	*
		- QProg&

		- Quantum program



.. rubric:: Returns:

bool

.. index:: pair: function; transformQProgToBinary
.. _doxid-group___utilities_1gab977f2314768f84df494fc726b269957:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<uint8_t> QPanda::transformQProgToBinary(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm)

Get quantum program binary data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QuantumMachine&

		- quantum



.. rubric:: Returns:

std::vector<uint8_t> quantum program binary data

.. index:: pair: function; transformQProgToBinary
.. _doxid-group___utilities_1gae59f3170912283e6f2912778bda63a4d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::transformQProgToBinary(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename)

Store quantum program in binary file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QuantumMachine\*

		- quantum machine

	*
		- std::string&

		- binary filename



.. rubric:: Returns:

void

.. index:: pair: function; convert_qprog_to_binary
.. _doxid-group___utilities_1gac91ac2b0027e3eb2f08ae86a1fc5201e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<uint8_t> QPanda::convert_qprog_to_binary(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm)

Get quantum program binary data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QuantumMachine&

		- quantum



.. rubric:: Returns:

std::vector<uint8_t> quantum program binary data

.. index:: pair: function; convert_qprog_to_binary
.. _doxid-group___utilities_1gaa5d087d0a28e6d87372ad75f6a3ae010:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::convert_qprog_to_binary(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, const std::string& filename)

Store quantum program in binary file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QuantumMachine\*

		- quantum machine

	*
		- std::string&

		- binary filename



.. rubric:: Returns:

void

.. index:: pair: function; transformQProgToOriginIR
.. _doxid-group___utilities_1gac85a4be007c80a0c9bcac301414797c3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty>
	std::string QPanda::transformQProgToOriginIR(
		_Ty& node,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine
		)

Quantum Program Transform To OriginIR



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty&

		- quantum program, quantum circuit, quantum while or quantum if



.. rubric:: Returns:

std::string QASM instruction set



.. rubric:: See also:

.. ref-code-block:: cpp

	  init(QuantumMachine_type::CPU);
	
	  auto qubit = qAllocMany(6);
	  auto cbit  = cAllocMany(2);
	  auto prog = CreateEmptyQProg();
	
	  prog << CZ(qubit[0], qubit[2]) << H(qubit[1]) << CNOT(qubit[1], qubit[2])
	  << RX(qubit[0],pi/2) << Measure(qubit[1],cbit[1]);
	extern QuantumMachine* global_quantum_machine;
	  std::cout << transformQProgToOriginIR(prog, global_quantum_machine) << std::endl;
	  finalize();

.. index:: pair: function; convert_qprog_to_originir
.. _doxid-group___utilities_1ga139b35c89a0f7882bc77200bcf3e7b08:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty>
	std::string QPanda::convert_qprog_to_originir(
		_Ty& node,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine
		)

Convert Quantum Program To OriginIR.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty&

		- quantum program, quantum circuit, quantum while or quantum if

	*
		- QuantumMachine\*

		- quantum machine



.. rubric:: Returns:

std::string QASM instruction set

.. index:: pair: function; transformQProgToQASM
.. _doxid-group___utilities_1gaa13be205f3f69ecf28d1d7759bdd8461:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::transformQProgToQASM(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& pQProg,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine,
		:ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` ibmBackend = :ref:`IBMQ_QASM_SIMULATOR<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8ca09728e1eb958bbe0ec92174a7ce111cd>`
		)

Quantum program transform to qasm instruction set.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- Quantum Program

	*
		- QuantumMachine\*

		- quantum machine pointer

	*
		- IBMQBackends

		- ibmBackend = IBMQ_QASM_SIMULATOR



.. rubric:: Returns:

std::string QASM instruction set



.. rubric:: See also:

.. ref-code-block:: cpp

	  init(QuantumMachine_type::CPU);
	
	  auto qubit = qAllocMany(6);
	  auto cbit  = cAllocMany(2);
	  auto prog = CreateEmptyQProg();
	
	  prog << CZ(qubit[0], qubit[2]) << H(qubit[1]) << CNOT(qubit[1], qubit[2])
	  << RX(qubit[0],pi/2) << Measure(qubit[1],cbit[1]);
	
	extern QuantumMachine* global_quantum_machine;
	  std::cout << transformQProgToQASM(prog, global_quantum_machine) << std::endl;
	  finalize();

.. index:: pair: function; convert_qprog_to_qasm
.. _doxid-group___utilities_1ga2f95b62aff4c3ae3bbeac669bc64ec82:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::convert_qprog_to_qasm(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm, :ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` ibmBackend = :ref:`IBMQ_QASM_SIMULATOR<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8ca09728e1eb958bbe0ec92174a7ce111cd>`)

Convert Quantum program to QASM instruction set.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- Quantum Program

	*
		- QuantumMachine\*

		- quantum machine pointer

	*
		- IBMQBackends

		- ibmBackend = IBMQ_QASM_SIMULATOR



.. rubric:: Returns:

std::string QASM instruction set

.. index:: pair: function; transformQProgToQuil
.. _doxid-group___utilities_1ga1afab9eb4d36a2758e559b40f63e82cc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::transformQProgToQuil(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine)

Quantum program transform to quil instruction set interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QuantumMachine\*

		- quantum machine pointer



.. rubric:: Returns:

std::string instruction set



.. rubric:: See also:

.. ref-code-block:: cpp

	  init();
	  QProg prog;
	  auto qvec = qAllocMany(4);
	  auto cvec = cAllocMany(4);
	
	  prog << X(qvec[0])
	  << Y(qvec[1])
	  << H(qvec[0])
	  << RX(qvec[0], 3.14)
	  << Measure(qvec[1], cvec[0])
	  ;
	extern QuantumMachine* global_quantum_machine;
	transformQProgToQuil(prog, global_quantum_machine)
	  finalize();

.. index:: pair: function; convert_qprog_to_quil
.. _doxid-group___utilities_1ga6ba609a5a9659c9247464add93496ccb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::convert_qprog_to_quil(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm)

Quantum program transform to quil instruction set interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QuantumMachine\*

		- quantum machine pointer



.. rubric:: Returns:

std::string instruction set

.. index:: pair: function; transformQRunesToQProg
.. _doxid-group___utilities_1ga1f9755f387cd30e9ac65ea502269f908:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> QPanda::transformQRunesToQProg(std::string, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*)

QRunes instruction set transform to quantum program interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- empty quantum program



.. rubric:: Returns:

void

.. index:: pair: function; arbitraryRotationMetadataValidity
.. _doxid-group___utilities_1ga785ac4c99106792eb8c00392e5576104:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::arbitraryRotationMetadataValidity(
		std::vector<std::string>& gates,
		std::vector<std::string>& valid_gates
		)

Judge if the metadata's type is arbitrary rotation.



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

Return the style of metadata validity

.. index:: pair: function; doubleContinuousMetadataValidity
.. _doxid-group___utilities_1gac4ba5476ec612a6f63122f9c33ccfbd8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::doubleContinuousMetadataValidity(
		std::vector<std::string>& gates,
		std::vector<std::string>& valid_gates
		)

Judge if the metadata's type is double continuous.



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

Return the style of metadata validity

.. index:: pair: function; singleContinuousAndDiscreteMetadataValidity
.. _doxid-group___utilities_1ga429a2bcbd0f51f6a5560bcb088c10e1e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::singleContinuousAndDiscreteMetadataValidity(
		std::vector<std::string>& gates,
		std::vector<std::string>& valid_gates
		)

Judge if the metadata's type is single continuous and discrete.



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

Return the style of metadata validity

.. index:: pair: function; doubleDiscreteMetadataValidity
.. _doxid-group___utilities_1ga5534bc47fbbbf2ccd5bd994feeebfd6a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::doubleDiscreteMetadataValidity(
		std::vector<std::string>& gates,
		std::vector<std::string>& valid_gates
		)

Judge if the metadata's type is double discrete.



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

Return the style of metadata validity

.. index:: pair: function; doubleGateMetadataValidity
.. _doxid-group___utilities_1gaceaea9db4f27bd09e4930b2ffa2fdfb5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::doubleGateMetadataValidity(
		std::vector<std::string>& gates,
		std::vector<std::string>& valid_gates
		)

Judge double gate type.



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

Return the style of metadata validity

.. index:: pair: function; validateSingleQGateType
.. _doxid-group___utilities_1ga0d5aad0edcc57eae1140ca91bf50bb5e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::validateSingleQGateType(
		std::vector<std::string>& gates,
		std::vector<std::string>& valid_gates
		)

Verify the validity of single quantum gates.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<std::string>&

		- gates vertor

	*
		- std::vector<std::string>&

		- output the valid gates



.. rubric:: Returns:

int single quantum gate type

.. index:: pair: function; isMatchTopology
.. _doxid-group___utilities_1ga459114e3940a2ff0128cf51ca92f98ca:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::isMatchTopology(
		const :ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate,
		const std::vector<std::vector<int>>& vecTopoSt
		)

judge the Qgate if match the target topologic structure of quantum circuit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vector<vector<int>>&

		- the target topologic structure of quantum circuit



.. rubric:: Returns:

if the Qgate match the target topologic structure return true, or else return false



.. rubric:: See also:

:ref:`XmlConfigParam::readAdjacentMatrix(TiXmlElement \*, int&, std::vector\<std::vector\<int>>&) <doxid-group___utilities_1ga4e141809ff97965ba3dee77eb8e198fa>`

.. index:: pair: function; getAdjacentQGateType
.. _doxid-group___utilities_1ga0adcec3f1d6e1cb173e5afadc3aac5ab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::getAdjacentQGateType(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr,
		std::vector<:ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`>& adjacentNodes
		)

get the adjacent quantum gates's(the front one and the back one) type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- nodeItr

		- the specialed :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

	*
		- std::vector<NodeInfo>&

		- adjacentNodes the front node and the back node



.. rubric:: Returns:

result string.



.. rubric:: See also:

.. index:: pair: function; isSwappable
.. _doxid-group___utilities_1ga18c8e4e48c21b6901eb93bd05e40ea30:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::isSwappable(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr1, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr2)

judge the specialed two NodeIters whether can be exchanged



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- nodeItr1

		- the first :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

	*
		- nodeItr2

		- the second :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`



.. rubric:: Returns:

if the two NodeIters can be exchanged, return true, otherwise retuen false.



.. rubric:: See also:

.. index:: pair: function; isSupportedGateType
.. _doxid-group___utilities_1ga28afe2b7d347e24df633c81ebb0d8ff1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::isSupportedGateType(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr)

judge if the target node is a base :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` type



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- nodeItr

		- the target :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`



.. rubric:: Returns:

if the target node is a base :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` type, return true, otherwise retuen false.



.. rubric:: See also:

.. index:: pair: function; getCircuitMatrix
.. _doxid-group___utilities_1gaecf3d5fffaaa40080b612fed1cd9d975:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` QPanda::getCircuitMatrix(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` srcProg,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrStart = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrEnd = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`()
		)

get the target matrix between the input two Nodeiters



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- nodeItrStart

		- the start :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

	*
		- nodeItrEnd

		- the end :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`



.. rubric:: Returns:

the target matrix include all the :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` 's matrix (multiply).



.. rubric:: See also:

.. index:: pair: function; pickUpNode
.. _doxid-group___utilities_1ga8484fc54a5cab80edc24654cc68201e1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::pickUpNode(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& outPutProg,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& srcProg,
		const std::vector<:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`> reject_node_types,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrStart = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` nodeItrEnd = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		bool bDagger = false
		)

pick up the nodes of srcProg between nodeItrStart and nodeItrEnd to outPutProg



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- outPutProg

		- the output prog

	*
		- srcProg

		- The source prog

	*
		- nodeItrStart

		- The start pos of source prog

	*
		- nodeItrEnd

		- The end pos of source prog

	*
		- reject_node_types

		- vector of the reject node types.

	*
		- bDagger

		- daggger flag @ Note: If there are any Qif/Qwhile nodes between nodeItrStart and nodeItrEnd, Or the nodeItrStart and the nodeItrEnd are in different sub-circuit, an exception will be throw.

.. index:: pair: function; get_all_used_qubits
.. _doxid-group___utilities_1ga60e9de7c80e617edb5f326689625a0c5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::get_all_used_qubits(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, std::vector<int>& vecQuBitsInUse)

Get all the used quantum bits in the input prog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prog

		- the input prog

	*
		- vecQuBitsInUse

		- The vector of used quantum bits @ Note: All the Qif/Qwhile or other sub-circuit nodes in the input prog will be ignored.

.. index:: pair: function; get_all_used_class_bits
.. _doxid-group___utilities_1gaaf010d547364709f49981078bf40cfae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::get_all_used_class_bits(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, std::vector<int>& vecClBitsInUse)

Get all the used class bits in the input prog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prog

		- the input prog

	*
		- vecClBitsInUse

		- The vector of used class bits @ Note: All the Qif/Qwhile or other sub-circuit nodes in the input prog will be ignored.

.. index:: pair: function; printAllNodeType
.. _doxid-group___utilities_1gae41e9802e11fe16be10a56819e6c6709:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::printAllNodeType(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

output all the node type of the target prog



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- the

		- target prog



.. rubric:: Returns:

return the output string

.. index:: pair: function; get_gate_parameter
.. _doxid-group___utilities_1ga79406ec5a5ba912ce1675534c4ed9366:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::get_gate_parameter(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> pGate, std::string& para_str)

get gate parameter



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- pGate

		- the target gate pointer

	*
		- para_str

		- parameter string



.. rubric:: Returns:

.. index:: pair: function; getQGateNum
.. _doxid-group___utilities_1gaa2167d6194906299c48b50228436f367:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty>
	size_t QPanda::getQGateNum(_Ty& node)

Count quantum gate num under quantum program, quantum circuit, quantum while, quantum if.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty&

		- quantum program, quantum circuit, quantum while or quantum if



.. rubric:: Returns:

size_t Quantum gate num



.. rubric:: See also:

.. ref-code-block:: cpp

	init();
	auto qubits = qAllocMany(4);
	auto cbits = cAllocMany(4);
	
	auto circuit = CreateEmptyCircuit();
	circuit << H(qubits[0]) << X(qubits[1]) << S(qubits[2])
	<< iSWAP(qubits[1], qubits[2]) << RX(qubits[3], PI/4);
	auto count = getQGateNumber(&circuit);
	std::cout << "QCircuit count: " << count << std::endl;
	
	finalize();

.. index:: pair: function; getQProgClockCycle
.. _doxid-group___utilities_1ga002a279e27f4843dbadd82c19553cdc1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t QPanda::getQProgClockCycle(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm)

Get quantum program clock cycle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- & quantum program

	*
		- QuantumMachine\*

		- quantum machine pointer



.. rubric:: See also:

.. ref-code-block:: cpp

	init();
	auto qubits = qAllocMany(4);
	auto prog = CreateEmptyQProg();
	prog << H(qubits[0]) << CNOT(qubits[0], qubits[1])
	        << iSWAP(qubits[1], qubits[2]) << RX(qubits[3], PI/4);
	extern QuantumMachine* global_quantum_machine;
	auto time = getQProgClockCycle(prog,global_quantum_machine );
	std::cout << "clockCycle : " << time << std::endl;
	
	finalize();

.. index:: pair: function; draw_qprog
.. _doxid-group___utilities_1ga5b68a36676155a7e2413fa1f2c3c02d2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::draw_qprog(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_start = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_end = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`()
		)

output a quantum prog/circuit to console by text-pic(UTF-8 code), and will save the text-pic in file named QCircuitTextPic.txt in the same time in current path.

All the output characters are UTF-8 code.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prog

		- the source prog

	*
		- itr_start

		- The start pos, default is the first node of the prog

	*
		- itr_end

		- The end pos, default is the end node of the prog



.. rubric:: Returns:

the output string

.. index:: pair: function; draw_qprog_with_clock
.. _doxid-group___utilities_1ga9729586010920bb1c7035ab3b207f119:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::draw_qprog_with_clock(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_start = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`(),
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` itr_end = :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`()
		)

output a quantum prog/circuit by time sequence to console by text-pic(UTF-8 code), and will save the text-pic in file named QCircuitTextPic.txt in the same time in current path.

All the output characters are UTF-8 code.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prog

		- the source prog

	*
		- itr_start

		- The start pos, default is the first node of the prog

	*
		- itr_end

		- The end pos, default is the end node of the prog



.. rubric:: Returns:

the output string

.. index:: pair: function; operator<<
.. _doxid-group___utilities_1gae4df8ff2e43a6a8ad196b3fe1ab31208:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::ostream& QPanda::operator << (std::ostream& out, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog)

Overload operator <<.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::ostream&

		- ostream

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- quantum program



.. rubric:: Returns:

std::ostream

.. index:: pair: function; graph_query_replace
.. _doxid-group___utilities_1gaa5d7f420dbaf504df35d77e11dc27313:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty1, typename _Ty2, typename _Ty3>
	void QPanda::graph_query_replace(
		_Ty1& graph_node,
		_Ty2& query_node,
		_Ty3& replace_node,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
		)

graph query and replace



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty1

		- & graph_node

	*
		- _Ty2

		- & query_node

	*
		- _Ty3

		- & replace_node

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- & prog

	*
		- :ref:`QuantumMachine <doxid-class_q_panda_1_1_quantum_machine>`

		- \* qvm



.. rubric:: Returns:

void

.. index:: pair: function; graph_query
.. _doxid-group___utilities_1gae94b1400c910547de03936bc91a94214:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty1, typename _Ty2>
	bool QPanda::graph_query(
		_Ty1& graph_node,
		_Ty2& query_node,
		:ref:`ResultVector<doxid-namespace_q_panda_1a960ac3f5e928f3a42f4d2f2191320897>`& query_result
		)

graph query



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty1

		- & graph_node

	*
		- _Ty2

		- & query_node

	*
		- ResultVector

		- & query_result



.. rubric:: Returns:

bool true or false

.. index:: pair: function; cast_qprog_qcircuit
.. _doxid-group___utilities_1gab6fa6a562c8f53d3e1a07ceae99c46d1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool QPanda::cast_qprog_qcircuit(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit)

Cast Quantum Program To Quantum Circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- quantum program

	*
		- QCircuit&

		- quantum progCircuitram



.. rubric:: Returns:

bool

.. index:: pair: function; cast_qprog_qgate
.. _doxid-group___utilities_1gafe6ca010315b8926648f71f591e04e6c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` QPanda::cast_qprog_qgate(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog)

Cast Quantum Program To Quantum Gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- quantum program



.. rubric:: Returns:

:ref:`QGate <doxid-class_q_panda_1_1_q_gate>` quantum gate

.. index:: pair: function; cast_qprog_qmeasure
.. _doxid-group___utilities_1gaeca0972f111c64634cafdffb628dcbed:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` QPanda::cast_qprog_qmeasure(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog)

Cast Quantum Program To Quantum Measure.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- quantum program



.. rubric:: Returns:

:ref:`QMeasure <doxid-class_q_panda_1_1_q_measure>` quantum measure

.. index:: pair: function; topology_match
.. _doxid-group___utilities_1ga378f5da8f88411621aa9f364db018746:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::topology_match(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine, :ref:`SwapQubitsMethod<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73>` method = :ref:`CNOT_GATE_METHOD<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73af0fd6c0d21b2b49d98160f724cff9cbe>`, :ref:`ArchType<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2a>` arch_type = :ref:`IBM_QX5_ARCH<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2aa1d998a495737ef4502e83b080f3dada0>`)

QProg/QCircuit matches the topology of the physical qubits.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prog

		- quantum program

	*
		- machine

		- quantum machine

	*
		- method

		- swap qubits by CNOT/CZ/SWAP/iSWAP gate

	*
		- arch_type

		- architectures type



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>` mapped quantum program

.. index:: pair: function; fill_qprog_by_I
.. _doxid-group___utilities_1ga44d0898c5b799ae5d5a61885bb843019:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::fill_qprog_by_I(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& input_prog)

Fill the input :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` by I gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- The

		- input Qprog



.. rubric:: Returns:

the filled :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`



.. rubric:: See also:

.. index:: pair: function; flatten
.. _doxid-group___utilities_1ga997126df699b036f29971b65d91f7720:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::flatten(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

Flatten Quantum Program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

void

.. index:: pair: function; flatten
.. _doxid-group___utilities_1ga4ec2bd572ad776b199ed47e9c21ac049:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::flatten(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit)

Flatten Quantum Circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QCircuit&

		- circuit program



.. rubric:: Returns:

void

.. index:: pair: function; full_flatten
.. _doxid-group___utilities_1gafbdb42f53bdf318319bbc3b2ff2dce46:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::full_flatten(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

Full Flatten Quantum Program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

void

.. index:: pair: function; partition
.. _doxid-group___utilities_1ga34e90d38e9f219c3633ddba0d1ca5b8f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::partition(
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& srcMatrix,
		int partitionRowNum,
		int partitionColumnNum,
		:ref:`blockedMatrix_t<doxid-namespace_q_panda_1a8f8db55e468baa3e5febdb847979eadc>`& blockedMat
		)

partition matrix by the input partitionRowNum and partitionColumnNum



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- srcMatrix

		- the source matrix

	*
		- partitionRowNum

		- Specify how many blocks to separated horizontally

	*
		- partitionColumnNum

		- Specify how many blocks to separated in the vertical direction

	*
		- blockedMat

		- The separated matrix



.. rubric:: Returns:

Execution successfully returns 0, otherwise returns to other.

.. index:: pair: function; blockMultip
.. _doxid-group___utilities_1ga332ecf657ba1ac5c4817ce9abf280557:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int QPanda::blockMultip(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& leftMatrix, const :ref:`blockedMatrix_t<doxid-namespace_q_panda_1a8f8db55e468baa3e5febdb847979eadc>`& blockedMat, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& resultMatrix)

Block Multiplication of Matrix.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- leftMatrix

		- the left input matrix

	*
		- blockedMat

		- The matrix blocks

	*
		- resultMatrix

		- The result of Block Multiplication



.. rubric:: Returns:

Execution successfully returns 0, otherwise returns to other.

.. index:: pair: function; dagger
.. _doxid-group___utilities_1gad7d29837687e202f654217bdc72c861e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::dagger(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& srcMat)

Getting the Inverted Conjugate Matrix of the target Matrix.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- srcMat

		- the target matrix



.. rubric:: Returns:

.. index:: pair: function; tensor
.. _doxid-group___utilities_1ga89e38fe6a988250608482e752ca15853:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` QPanda::tensor(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& leftMatrix, const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& rightMatrix)

Tensor Multiplication.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- leftMatrix

		- the left input matrix

	*
		- rightMatrix

		- the right input matrix



.. rubric:: Returns:

Tensor Product of input Left Matrix and Right Matrix.

.. index:: pair: function; matrix_to_string
.. _doxid-group___utilities_1ga4ade7ce8fa33b32b51559cd3689a6459:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::matrix_to_string(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& mat)

output matrix information to consol



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- mat

		- the target matrix



.. rubric:: Returns:

the matrix string

.. index:: pair: function; parityCheckCircuit
.. _doxid-group___utilities_1ga45bce8581a43de45a3bbf5b3c7cbafcd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::parityCheckCircuit(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> qubit_vec)

CNOT all qubits (except last) with the last qubit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<Qubit\*>

		- qubit vector



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; apply_QGate
.. _doxid-group___utilities_1ga296d3416ba243601d3939bb960284d97:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::apply_QGate(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubits, std::function<:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)> gate)

Apply Quantum Gate on a series of :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- qubit vector

	*
		- std::function<QGate(Qubit\*)>

		- :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` function



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; Toffoli
.. _doxid-group___utilities_1ga360ff2641ae0d9229ff920de8050fadf:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` QPanda::Toffoli(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qc1, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qc2, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target)

Toffoli Quantum Gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- first control qubit

	*
		- Qubit\*

		- second control qubit

	*
		- Qubit\*

		- target qubit



.. rubric:: Returns:

:ref:`QGate <doxid-class_q_panda_1_1_q_gate>`

.. index:: pair: function; split
.. _doxid-group___utilities_1gad46a951a6cfb7b6339415f05686a80f4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> QPanda::split(
		const std::string& str,
		const std::string& delim
		)

Splits the string by symbol.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- string

	*
		- std::string&

		- delim



.. rubric:: Returns:

std::vector<std::string>

.. index:: pair: function; str2int
.. _doxid-group___utilities_1ga5ea0e3dbc8f13d4acf35ae04e30633c6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::str2int(std::string s, long long& num)

cast string to int



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- string

	*
		- long

		- long& number



.. rubric:: Returns:

bool

.. index:: pair: function; str2double
.. _doxid-group___utilities_1gab6004f2bad15ec13d4f40d3ab35c3979:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::str2double(std::string s, double& num)

cast string to double



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- string

	*
		- double&

		- number



.. rubric:: Returns:

bool

.. index:: pair: function; ll2str
.. _doxid-group___utilities_1ga94d1661951a9556739e9c890275c421b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::ll2str(long long num)

cast long long to string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- long

		- long number



.. rubric:: Returns:

std::string

.. index:: pair: function; int2str
.. _doxid-group___utilities_1ga4ba82eb2f8ee44b6bbe7387295f47e46:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::int2str(int num)

cast int to string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- number



.. rubric:: Returns:

std::string

.. index:: pair: function; double2str
.. _doxid-group___utilities_1gabcdf63fbfaf0af391fbce6dca1a932c7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::double2str(double num)

cast double to string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- number



.. rubric:: Returns:

std::string

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
		- UnsignedIntegralType&

		- number

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
		- UnsignedIntegralType&

		- number



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
		- UnsignedIntegralType&

		- num1

	*
		- UnsignedIntegralType&

		- num2

	*
		- std::vector<size_t>

		- qvec

	*
		- size_t

		- binary string length



.. rubric:: Returns:

Unsigned Integral Type

