.. index:: pair: class; QPanda::NoiseSimulator
.. _doxid-class_q_panda_1_1_noise_simulator:

class QPanda::NoiseSimulator
============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NoiseSimulator.h>
	
	class NoiseSimulator: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		bool :target:`has_quantum_error<doxid-class_q_panda_1_1_noise_simulator_1ab73ed0e5310eb2c21a635b5370a810b3>`();
		void :target:`set_rotation_error<doxid-class_q_panda_1_1_noise_simulator_1a01a5c929e17a21ef2c10f150d777cf09>`(double);
	
		void :target:`set_measure_error<doxid-class_q_panda_1_1_noise_simulator_1a1ec80489e4a4a7758acec29ab2018200>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			double param
			);
	
		void :target:`set_measure_error<doxid-class_q_panda_1_1_noise_simulator_1a349b071bf1f58758fc329a059d812cdc>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			double param,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits_vec
			);
	
		void :target:`set_measure_error<doxid-class_q_panda_1_1_noise_simulator_1a1a1f8fb8b0b145a7a45f5c8340784105>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			double T1,
			double T2,
			double time_param
			);
	
		void :target:`set_measure_error<doxid-class_q_panda_1_1_noise_simulator_1a9e451d94d88554d14102f88606926b64>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			double T1,
			double T2,
			double time_param,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits_vec
			);
	
		void :target:`set_reset_error<doxid-class_q_panda_1_1_noise_simulator_1a9c73ec4b9a32f0035459524891a3e370>`(
			double,
			double
			);
	
		void :target:`set_readout_error<doxid-class_q_panda_1_1_noise_simulator_1a18100ce979b7a44b96d388c49037d6dc>`(
			const std::vector<std::vector<double>>& readout_params,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits
			);
	
		void :target:`set_combining_error<doxid-class_q_panda_1_1_noise_simulator_1ac055129b46d7175d78ced139ca6de739>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			const :ref:`KarusError<doxid-class_q_panda_1_1_karus_error>`& karus_error,
			const std::vector<:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`>& qubits_vecs
			);
	
		void :target:`set_mixed_unitary_error<doxid-class_q_panda_1_1_noise_simulator_1a0a2f5edc62d1beb328c5a6cd97efe3e9>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& karus_matrices
			);
	
		void :target:`set_mixed_unitary_error<doxid-class_q_panda_1_1_noise_simulator_1aaf96487f1340c0789a05c2f9ec1fa4cc>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices,
			const std::vector<double>& probs_vec
			);
	
		void :target:`set_mixed_unitary_error<doxid-class_q_panda_1_1_noise_simulator_1ac9770463ad07bf56bcefe765949aa35c>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& karus_matrices,
			const std::vector<:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`>& qubits_vecs
			);
	
		void :target:`set_mixed_unitary_error<doxid-class_q_panda_1_1_noise_simulator_1ae186e8920a7a06a20eb9c6a9165a97fd>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices,
			const std::vector<double>& probs_vec,
			const std::vector<:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`>& qubits_vecs
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_simulator_1a1679408bca739487beb7ea967b739ca8>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			double param
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_simulator_1a4da22d143431e1f622a442328e03b4e4>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			double param,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits_vec
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_simulator_1adf6570746fde24b54d030b41bc1cca7b>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			double param,
			const std::vector<:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`>& qubits_vecs
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_simulator_1a5a9aa24f8b25118f28f80ac021a1d4dc>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			double T1,
			double T2,
			double time_param
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_simulator_1a5bfbb14037359dd654b7c102ee90cae5>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			double T1,
			double T2,
			double time_param,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits_vecs
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_simulator_1a404db5adc417e7e3c014e41d53320aed>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate_type,
			double T1,
			double T2,
			double time_param,
			const std::vector<:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`>& qubits_vecs
			);
	
		void :target:`set_mps_qpu_and_result<doxid-class_q_panda_1_1_noise_simulator_1ad2ba82379203954fe7255310689a277f>`(
			std::shared_ptr<:ref:`MPSImplQPU<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u>`> mps_qpu,
			:ref:`QResult<doxid-class_q_panda_1_1_q_result>`* result
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_noise_simulator_1a4c43a1189f1393d2aeb81e43863623ce>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QCircuitConfig<doxid-struct_q_panda_1_1_q_circuit_config>`& config
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_noise_simulator_1a93c0dfc43fe2d3dd45e21ba67e4466be>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QCircuitConfig<doxid-struct_q_panda_1_1_q_circuit_config>`& config
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_noise_simulator_1a7c916a53bdf9475ea1beb41700785882>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QCircuitConfig<doxid-struct_q_panda_1_1_q_circuit_config>`& config
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_noise_simulator_1a25aae0f091d017e5f6de486e0e82f423>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QCircuitConfig<doxid-struct_q_panda_1_1_q_circuit_config>`& config
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_noise_simulator_1a1b9b36976a4f1e01c20c596eae6ef72c>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QCircuitConfig<doxid-struct_q_panda_1_1_q_circuit_config>`& config
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_noise_simulator_1a45a7cf8c17fd3ae0e7437e94c3161682>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QCircuitConfig<doxid-struct_q_panda_1_1_q_circuit_config>`& config
			);
	
		void :target:`execute<doxid-class_q_panda_1_1_noise_simulator_1a87a547f20eb1f1042240cdf80d260763>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`>,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>,
			:ref:`QCircuitConfig<doxid-struct_q_panda_1_1_q_circuit_config>`& config
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1adb53e4c20d48a0efd6e377680d7f0988>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aed584073b781c9a5c6441b08b14afc3d>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aadbf69a810033196de1790d3f362ef7a>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aab65fda71b8e1f719bc4b7bdd70a10e7>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1ab452f71d25eb3354d46346694ff82db7>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a4e97902dc8b42d5f5f50d790d11f1517>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aa311fe1c6abc46d84d90d6f412be063a>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);

