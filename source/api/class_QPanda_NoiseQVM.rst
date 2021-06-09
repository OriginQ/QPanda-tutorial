.. index:: pair: class; QPanda::NoiseQVM
.. _doxid-class_q_panda_1_1_noise_q_v_m:

class QPanda::NoiseQVM
======================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class NoiseQVM: public :ref:`QPanda::QVM<doxid-class_q_panda_1_1_q_v_m>`
	{
	public:
		// methods
	
		virtual void :ref:`init<doxid-class_q_panda_1_1_noise_q_v_m_1a46b2fc848827943ea96124536ffa4c74>`();
		void :target:`init<doxid-class_q_panda_1_1_noise_q_v_m_1ac73472754a26126d378511f354ed1435>`(rapidjson::Document&);
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_noise_q_v_m_1a5aa290e2ecd98bce296a84b670856bf1>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, rapidjson::Document&);
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_noise_q_v_m_1a47bd3329930f053b06a2c0c1510f9fbc>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, int);
	
		virtual std::map<std::string, size_t> :target:`runWithConfiguration<doxid-class_q_panda_1_1_noise_q_v_m_1acd6754f579938a1008758d3281427d70>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			std::vector<int>&,
			int
			);
	
		virtual std::map<std::string, bool> :ref:`directlyRun<doxid-class_q_panda_1_1_noise_q_v_m_1ae7139fbb84abe1884c339b1e2ffae85d>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg);
		virtual void :target:`run<doxid-class_q_panda_1_1_noise_q_v_m_1ab29826af029b3726c63110aa7e7d03e7>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_q_v_m_1a7cc9be56d4600a7060a016fced0eb0ca>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			double prob
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_q_v_m_1ab6c5e77d4fc7e5c5854144b0980ea8c3>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			double prob,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_q_v_m_1a992214bee3f77d49752425c8752e97a1>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			double prob,
			const std::vector<:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`>& qubits
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_q_v_m_1a8fab38d199d0a624a9531783bcc5582c>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			double T1,
			double T2,
			double t_gate
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_q_v_m_1a568c2c0e1cc650c51e5e1606c88d65e2>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			double T1,
			double T2,
			double t_gate,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits
			);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_noise_q_v_m_1a3d25495967d1b36b81d77f241efa4a7b>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			double T1,
			double T2,
			double t_gate,
			const std::vector<:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`>& qubits
			);
	
		void :target:`set_measure_error<doxid-class_q_panda_1_1_noise_q_v_m_1a1f3f56f688ca874e62582d74ebc33c0a>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			double prob,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits = {}
			);
	
		void :target:`set_measure_error<doxid-class_q_panda_1_1_noise_q_v_m_1a67c90ea8eace86efef2fe1c5a3d9fd63>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			double T1,
			double T2,
			double t_gate,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits = {}
			);
	
		void :target:`set_mixed_unitary_error<doxid-class_q_panda_1_1_noise_q_v_m_1a6052511c9d987ef42b7da920607c94df>`(
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices,
			const std::vector<double>& probs
			);
	
		void :target:`set_mixed_unitary_error<doxid-class_q_panda_1_1_noise_q_v_m_1a645d427d3e93300f03dae8033cb31de8>`(
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices,
			const std::vector<double>& probs,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits
			);
	
		void :target:`set_mixed_unitary_error<doxid-class_q_panda_1_1_noise_q_v_m_1a60eac75ac49a2c25598537a5ad962a49>`(
			const :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`& type,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices,
			const std::vector<double>& probs,
			const std::vector<:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`>& qubits
			);
	
		void :target:`set_reset_error<doxid-class_q_panda_1_1_noise_q_v_m_1a466bb40518e57cb3892572c9690e1277>`(
			double p0,
			double p1,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits = {}
			);
	
		void :target:`set_readout_error<doxid-class_q_panda_1_1_noise_q_v_m_1a743d72cfc2da340b490cbccf9bdcd8bb>`(
			const std::vector<std::vector<double>>& probs_list,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits = {}
			);
	
		void :ref:`set_rotation_error<doxid-class_q_panda_1_1_noise_q_v_m_1a1d5a75aad44fd7fdd33c0842e7f3c2fb>`(double error);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_quantum_machine_1a732d439bfb76b74edb3d2404568a1900>`(size_t) = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_quantum_machine_1a2352ae1e515dad9a445a59069a42161e>`(size_t) = 0;
		virtual void :ref:`init<doxid-class_q_panda_1_1_quantum_machine_1ac2ebbb77482669f310f9b5d0b6f30fa1>`() = 0;
		virtual :ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* :ref:`getStatus<doxid-class_q_panda_1_1_quantum_machine_1a29299cd9882a2f5016971121a58fa679>`() const = 0;
		virtual std::map<std::string, bool> :ref:`directlyRun<doxid-class_q_panda_1_1_quantum_machine_1a77357644931b71be480590764df59451>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg) = 0;
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_quantum_machine_1a7dded3823353840ab733abdc3fb999b2>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, rapidjson::Document&) = 0;
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_quantum_machine_1af49fc4f7b7b608fed6327bcde3d28226>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, int) = 0;
		virtual std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t> :ref:`getGateTimeMap<doxid-class_q_panda_1_1_quantum_machine_1a9caf6ddc2d278e222db50b78ff6d5a03>`() const = 0;
		virtual void :ref:`finalize<doxid-class_q_panda_1_1_quantum_machine_1a2aff067ba64013dce87814dfdfbdc176>`() = 0;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_panda_1_1_quantum_machine_1aee285b6b7f5cd7936491f2b304501167>`() const = 0;
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_quantum_machine_1ae01f52fad0cde4e96dbc4945e3f6f93f>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const = 0;
		virtual bool :ref:`swapQubitPhysicalAddress<doxid-class_q_panda_1_1_quantum_machine_1a8f444f30f7675ee5e1e2c7db53264b7d>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual void :ref:`setConfig<doxid-class_q_panda_1_1_quantum_machine_1a1f32aa1b5d33961b1a33a7a5c5c61be5>`(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`&) = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubit<doxid-class_q_panda_1_1_quantum_machine_1a0b8228ea18d362fba29ff5fcdded60b4>`() = 0;
		virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`allocateQubits<doxid-class_q_panda_1_1_quantum_machine_1a190cd3e9af3aa1a34420b91e2f60f60a>`(size_t) = 0;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`allocateCBit<doxid-class_q_panda_1_1_quantum_machine_1a944298196e0c6dbf6e641395af82f4c9>`() = 0;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`allocateCBit<doxid-class_q_panda_1_1_quantum_machine_1a1c95eb9d941db948d60767a460aa20d0>`(size_t) = 0;
		virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`allocateCBits<doxid-class_q_panda_1_1_quantum_machine_1a5ab5745be7c1c4fc44a928fdbf1c87e1>`(size_t) = 0;
		virtual void :ref:`Free_Qubit<doxid-class_q_panda_1_1_quantum_machine_1a480d3b51048e1e8923bef9325d5f524d>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual void :ref:`Free_Qubits<doxid-class_q_panda_1_1_quantum_machine_1a933fe5bcb93118dfad9d096676885eb7>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual void :ref:`Free_CBit<doxid-class_q_panda_1_1_quantum_machine_1a42f5901a2104eefe29e9ff276076eb08>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&) = 0;
		virtual void :ref:`Free_CBits<doxid-class_q_panda_1_1_quantum_machine_1a331c9a57d8af8769f8c6332529b7b043>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0;
		virtual size_t :ref:`getAllocateQubit<doxid-class_q_panda_1_1_quantum_machine_1a98784101fb0ae8d98d1fd311a39689b8>`() = 0;
		virtual size_t :ref:`getAllocateCMem<doxid-class_q_panda_1_1_quantum_machine_1aabf896ec46e67498900467a38ddaee7c>`() = 0;
		virtual void :ref:`setConfigure<doxid-class_q_panda_1_1_quantum_machine_1a2e780aea11e55ee381c0ae983f65291d>`(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`&) = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`qAlloc<doxid-class_q_panda_1_1_quantum_machine_1a8d41c197973a4c544928facdd9b80e05>`() = 0;
		virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`qAllocMany<doxid-class_q_panda_1_1_quantum_machine_1ae1ed8d4a83d8167a111992245016f6e8>`(size_t qubit_count) = 0;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`cAlloc<doxid-class_q_panda_1_1_quantum_machine_1aa6e93c19e315072799915d4f9b02223f>`() = 0;
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`cAlloc<doxid-class_q_panda_1_1_quantum_machine_1ad7ebf59186a299d850ddf4ac3eeebaf1>`(size_t) = 0;
		virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`cAllocMany<doxid-class_q_panda_1_1_quantum_machine_1a0aeb0517f0dc84b9b9bbb100c87430dc>`(size_t) = 0;
		virtual void :ref:`qFree<doxid-class_q_panda_1_1_quantum_machine_1a5a61e36151d84476f64d66337435a2c1>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual void :ref:`qFreeAll<doxid-class_q_panda_1_1_quantum_machine_1afc3c5771b37a13c0ebd65a940029c9fb>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual void :ref:`cFree<doxid-class_q_panda_1_1_quantum_machine_1a3d96ab037bdfe79a6cd32d394d51c3b0>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&) = 0;
		virtual void :ref:`cFreeAll<doxid-class_q_panda_1_1_quantum_machine_1a2912a9f37c8600d8d0fc875eeca402d5>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0;
		virtual size_t :ref:`getAllocateQubitNum<doxid-class_q_panda_1_1_quantum_machine_1a66fe7b76e261cde0b4571fc796107fcc>`() = 0;
		virtual size_t :ref:`getAllocateCMemNum<doxid-class_q_panda_1_1_quantum_machine_1ac49cf7c186b153bc277e2505efce9344>`() = 0;
		virtual void :ref:`initState<doxid-class_q_panda_1_1_quantum_machine_1ad8c9c37bd0aa2f8e3d2aaa0f0468de86>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& state = {}, const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qlist = {}) = 0;
		virtual size_t :ref:`get_allocate_qubits<doxid-class_q_panda_1_1_quantum_machine_1af4601428256d3511b0004d3c7def733f>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual size_t :ref:`get_allocate_cbits<doxid-class_q_panda_1_1_quantum_machine_1a2c5e32ecb79ce0dbaabf03412d01e50a>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0;
		virtual double :ref:`get_expectation<doxid-class_q_panda_1_1_quantum_machine_1a36e280b887f9cf99498403897233811c>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`, const QHamiltonian&, const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual double :ref:`get_expectation<doxid-class_q_panda_1_1_quantum_machine_1a9f12409d33e4e66a7fd9c8e7eedb76ef>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`, const QHamiltonian&, const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int) = 0;
		virtual void :ref:`initState<doxid-class_q_panda_1_1_q_v_m_1ab0b60d46e7207275274ad09314023ee1>`(const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& state = {}, const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qlist = {});
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_q_v_m_1af3506b5b2b35451a8aae7364193f2843>`(size_t);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_q_v_m_1ae1f3ad0f3880eaada1101df5f6cc14f6>`(size_t);
		virtual :ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* :ref:`getStatus<doxid-class_q_panda_1_1_q_v_m_1a2fbdc658f90b541abd43934c93257b10>`() const;
		virtual :ref:`QResult<doxid-class_q_panda_1_1_q_result>`* :ref:`getResult<doxid-class_q_panda_1_1_q_v_m_1acd345a3ebac094ceb9e685971672fa81>`();
		virtual std::map<std::string, bool> :ref:`getResultMap<doxid-class_q_panda_1_1_q_v_m_1aea2b65cd9c75d21d6c3201ab9c7deb3c>`();
		virtual void :ref:`finalize<doxid-class_q_panda_1_1_q_v_m_1ae1fdcd040b4c6612bbe684a606668453>`();
		virtual std::map<std::string, bool> :ref:`directlyRun<doxid-class_q_panda_1_1_q_v_m_1adcf36345640beff726ad3fc6bb49c15b>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg);
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_q_v_m_1a72948f788f8630b0eeffd987cf475a46>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, rapidjson::Document&);
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_q_v_m_1a153f1460b033c11151e5ff3d35777f6e>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, int);
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_q_v_m_1a5a1e732b9903509586937a9d46cb4010>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<int>&, int);
		virtual std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t> :ref:`getGateTimeMap<doxid-class_q_panda_1_1_q_v_m_1ab5b2509d10ba71c908190eb8b5ef5385>`() const;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_panda_1_1_q_v_m_1a8b2d34ed071e6c9a2450a692e80fc855>`() const;
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_q_v_m_1a741a08893001a17609839f50a71f9535>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const;
		virtual bool :ref:`swapQubitPhysicalAddress<doxid-class_q_panda_1_1_q_v_m_1a4b9d45dc4072ea7dc4e507fbcf6e5567>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual void :ref:`set_random_engine<doxid-class_q_panda_1_1_q_v_m_1afb372ab384b1ec6791addc1af36d8ad5>`(:ref:`RandomEngine<doxid-class_random_engine>`* rng);
		virtual void :ref:`setConfig<doxid-class_q_panda_1_1_q_v_m_1a3a098815442fa6dc4b322e58b8e2bdc6>`(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`& config);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubit<doxid-class_q_panda_1_1_q_v_m_1ab42756f84764948ff31b4d87c79d3e43>`();
		virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`allocateQubits<doxid-class_q_panda_1_1_q_v_m_1a1dd87950e34b38f83452e98f3a548f05>`(size_t);
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`allocateCBit<doxid-class_q_panda_1_1_q_v_m_1a5379b3b9ed124ae76e5b365429132304>`();
		virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`allocateCBits<doxid-class_q_panda_1_1_q_v_m_1a9907e505e82030f4af78c2fce231fd4b>`(size_t);
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`allocateCBit<doxid-class_q_panda_1_1_q_v_m_1ac9cfc237aaa20194ae4a6afc8095da8a>`(size_t);
		virtual size_t :ref:`getAllocateQubit<doxid-class_q_panda_1_1_q_v_m_1aac63304751354d973d150466936ef5b5>`();
		virtual size_t :ref:`getAllocateCMem<doxid-class_q_panda_1_1_q_v_m_1af9a55a93940aade484f02cbd9831f769>`();
		virtual void :ref:`Free_Qubit<doxid-class_q_panda_1_1_q_v_m_1a9938820e903ad8944ac18e8fc12d10bd>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual void :ref:`Free_Qubits<doxid-class_q_panda_1_1_q_v_m_1abc0663c135f5227d694bc4f20a982531>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual void :ref:`Free_CBit<doxid-class_q_panda_1_1_q_v_m_1a8d3af5eafe432611cfcadf3319a674af>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&);
		virtual void :ref:`Free_CBits<doxid-class_q_panda_1_1_q_v_m_1a50dc95283f276e7de241ae4a95d55988>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&);
		virtual void :ref:`setConfigure<doxid-class_q_panda_1_1_q_v_m_1ad344c02cad43a5d3d451d55853d378a2>`(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`&);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`qAlloc<doxid-class_q_panda_1_1_q_v_m_1ad9de2e6468b65d4e5f97ece36498a7c9>`();
		virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`qAllocMany<doxid-class_q_panda_1_1_q_v_m_1ab1c3644b4253ca991421b2e0c90a94e7>`(size_t qubit_count);
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`cAlloc<doxid-class_q_panda_1_1_q_v_m_1a0cf8de6f2957639bd4d66ab2f148d295>`();
		virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`cAlloc<doxid-class_q_panda_1_1_q_v_m_1a698dbdafc368dbb092b51b565f03f63d>`(size_t);
		virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`cAllocMany<doxid-class_q_panda_1_1_q_v_m_1ad0d83c214ff3c53aa15e929e61d23665>`(size_t);
		virtual void :ref:`qFree<doxid-class_q_panda_1_1_q_v_m_1af00ee41c463d9c45d1148d94c5b721f3>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual void :ref:`qFreeAll<doxid-class_q_panda_1_1_q_v_m_1a265c6b00fa422d5dea5f02c0a06ff085>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual void :ref:`cFree<doxid-class_q_panda_1_1_q_v_m_1a9d1b31118208791c67e5bd799877f175>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&);
		virtual void :ref:`cFreeAll<doxid-class_q_panda_1_1_q_v_m_1a9b9e59e08e47272d70f10681fb380fa1>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&);
		virtual size_t :ref:`getAllocateQubitNum<doxid-class_q_panda_1_1_q_v_m_1a268030f1c16325f7496f0eef3efb5533>`();
		virtual size_t :ref:`getAllocateCMemNum<doxid-class_q_panda_1_1_q_v_m_1aba6a435098a6e9d1c6d50948f3f7cbdb>`();
		virtual size_t :ref:`get_allocate_qubits<doxid-class_q_panda_1_1_q_v_m_1a7115e91d4095a93ba7d0807a8f39fe02>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual size_t :ref:`get_allocate_cbits<doxid-class_q_panda_1_1_q_v_m_1af59b74befd842fd5efad2eb01421d6a9>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&);
		virtual double :ref:`get_expectation<doxid-class_q_panda_1_1_q_v_m_1a35e982022b6f057a6d704b9f2c8dd0b4>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`, const QHamiltonian&, const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual double :ref:`get_expectation<doxid-class_q_panda_1_1_q_v_m_1ac1a962a1f59c5f2ab29f632d5cabb8a9>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`, const QHamiltonian&, const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int);

.. _details-class_q_panda_1_1_noise_q_v_m:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; init
.. _doxid-class_q_panda_1_1_noise_q_v_m_1a46b2fc848827943ea96124536ffa4c74:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void init()

init



.. rubric:: Returns:

void

.. index:: pair: function; runWithConfiguration
.. _doxid-class_q_panda_1_1_noise_q_v_m_1a5aa290e2ecd98bce296a84b670856bf1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, size_t> runWithConfiguration(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&,
		rapidjson::Document&
		)

runWithConfiguration



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- std::vector<ClassicalCondition>&

		- 

	*
		- rapidjson::Document&

		- 



.. rubric:: Returns:

std::map<std::string, Eigen::size_t>

.. index:: pair: function; runWithConfiguration
.. _doxid-class_q_panda_1_1_noise_q_v_m_1a47bd3329930f053b06a2c0c1510f9fbc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, size_t> runWithConfiguration(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&,
		int
		)

runWithConfiguration



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- std::vector<ClassicalCondition>&

		- 

	*
		- int

		- 



.. rubric:: Returns:

std::map<std::string, Eigen::size_t>

.. index:: pair: function; directlyRun
.. _doxid-class_q_panda_1_1_noise_q_v_m_1ae7139fbb84abe1884c339b1e2ffae85d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, bool> directlyRun(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg)

directlyRun



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

std::map<std::string, bool>

.. index:: pair: function; set_rotation_error
.. _doxid-class_q_panda_1_1_noise_q_v_m_1a1d5a75aad44fd7fdd33c0842e7f3c2fb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_rotation_error(double error)

set :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` rotation angle errors



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- rotation angle errors



.. rubric:: Returns:

void



.. rubric:: See also:

:ref:`QNode <doxid-class_q_panda_1_1_q_node>`

