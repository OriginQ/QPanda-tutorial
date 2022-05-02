.. index:: pair: class; QPanda::QCloudMachine
.. _doxid-class_q_panda_1_1_q_cloud_machine:

class QPanda::QCloudMachine
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCloudMachine.h>
	
	class QCloudMachine: public :ref:`QPanda::QVM<doxid-class_q_panda_1_1_q_v_m>`
	{
	public:
		// methods
	
		void :ref:`init<doxid-class_q_panda_1_1_q_cloud_machine_1a3544a8e3d897ae583bf2a1f34034efb2>`(std::string token);
		void :target:`set_compute_api<doxid-class_q_panda_1_1_q_cloud_machine_1a8beb064d6053c3a1e1bdf6c192421a13>`(std::string url);
		void :target:`set_inqure_api<doxid-class_q_panda_1_1_q_cloud_machine_1a10428100af7c23d8716c44623f2eeb67>`(std::string url);
	
		void :target:`set_noise_model<doxid-class_q_panda_1_1_q_cloud_machine_1a4a3ed3d01d7d4c34d325b3f2d0b1f70c>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` model,
			const std::vector<double> single_params,
			const std::vector<double> double_params
			);
	
		std::map<std::string, double> :ref:`noise_measure<doxid-class_q_panda_1_1_q_cloud_machine_1a7760a3c6412f9b37cdc2b1d508897314>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			int shot,
			std::string task_name = "Qurator Experiment"
			);
	
		std::map<std::string, double> :ref:`full_amplitude_measure<doxid-class_q_panda_1_1_q_cloud_machine_1a1c18bc917b46d97add7eba23f8faaa10>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			int shot,
			std::string task_name = "Qurator Experiment"
			);
	
		std::map<std::string, double> :ref:`full_amplitude_pmeasure<doxid-class_q_panda_1_1_q_cloud_machine_1a402a84489c778d58fd9e521a33fd04d8>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` qubit_vec,
			std::string task_name = "Qurator Experiment"
			);
	
		std::map<std::string, :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`> :ref:`partial_amplitude_pmeasure<doxid-class_q_panda_1_1_q_cloud_machine_1a9b0aa99970c003407ede312e35e9fe34>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			std::vector<std::string> amplitude_vec,
			std::string task_name = "Qurator Experiment"
			);
	
		:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` :ref:`single_amplitude_pmeasure<doxid-class_q_panda_1_1_q_cloud_machine_1a5aa5a65e1d212080bfa199293a1be130>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, std::string amplitude, std::string task_name = "Qurator Experiment");
	
		std::map<std::string, double> :ref:`real_chip_measure<doxid-class_q_panda_1_1_q_cloud_machine_1a8adc86c4b49fa08f668f1107a2a7bb0e>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			int shot,
			size_t chipid = 0,
			std::string task_name = "Qurator Experiment"
			);
	
		std::map<std::string, double> :ref:`real_chip_task<doxid-class_q_panda_1_1_q_cloud_machine_1a7705475bdf440a43a07c7258ec28ab06>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			int shot,
			bool mapping_flag,
			bool circuit_optimization,
			bool is_vip,
			size_t chipid = 0
			);
	
		std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`> :ref:`get_state_tomography_density<doxid-class_q_panda_1_1_q_cloud_machine_1aa47e1e5e32624ceb6c42acfc3012c0d1>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, int shot, size_t chipid = 0);
		std::string :ref:`get_result_json<doxid-class_q_panda_1_1_q_cloud_machine_1a32e95a44728a06c2aa2c24a17e31845c>`(std::string taskid, :ref:`CLOUD_QMACHINE_TYPE<doxid-namespace_q_panda_1abd0ad768e93ef08e8cfabd780d803863>` type);
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

.. _details-class_q_panda_1_1_q_cloud_machine:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; init
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a3544a8e3d897ae583bf2a1f34034efb2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void init(std::string token)

Init the quantum machine environment.

use this at the begin



.. rubric:: Returns:

void

.. index:: pair: function; noise_measure
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a7760a3c6412f9b37cdc2b1d508897314:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, double> noise_measure(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		int shot,
		std::string task_name = "Qurator Experiment"
		)

run a measure quantum program



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- int&

		- shot

	*
		- std::map<std::string

		- 

	*
		- double>

		- 



.. rubric:: Returns:

measure result

.. index:: pair: function; full_amplitude_measure
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a1c18bc917b46d97add7eba23f8faaa10:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, double> full_amplitude_measure(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		int shot,
		std::string task_name = "Qurator Experiment"
		)

run a measure quantum program



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- int&

		- shot

	*
		- std::map<std::string

		- 

	*
		- double>

		- 



.. rubric:: Returns:

measure result

.. index:: pair: function; full_amplitude_pmeasure
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a402a84489c778d58fd9e521a33fd04d8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, double> full_amplitude_pmeasure(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` qubit_vec,
		std::string task_name = "Qurator Experiment"
		)

run a pmeasure quantum program



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- Qnum

		- & qubit address vector

	*
		- std::map<std::string

		- 

	*
		- double>

		- 



.. rubric:: Returns:

pmeasure result

.. index:: pair: function; partial_amplitude_pmeasure
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a9b0aa99970c003407ede312e35e9fe34:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, :ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>`> partial_amplitude_pmeasure(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		std::vector<std::string> amplitude_vec,
		std::string task_name = "Qurator Experiment"
		)

run a pmeasure quantum program with partial amplitude backend



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- std::vector<std::string>

		- & amplitude subset

	*
		- std::map<std::string

		- 

	*
		- qcomplex_t>

		- 



.. rubric:: Returns:

pmeasure result

.. index:: pair: function; single_amplitude_pmeasure
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a5aa5a65e1d212080bfa199293a1be130:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` single_amplitude_pmeasure(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
		std::string amplitude,
		std::string task_name = "Qurator Experiment"
		)

run a pmeasure quantum program with single amplitude backend



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- std::string

		- amplitude

	*
		- qcomplex_t

		- 



.. rubric:: Returns:

pmeasure result

.. index:: pair: function; real_chip_measure
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a8adc86c4b49fa08f668f1107a2a7bb0e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, double> real_chip_measure(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		int shot,
		size_t chipid = 0,
		std::string task_name = "Qurator Experiment"
		)

run a measure quantum program



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- int&

		- shot

	*
		- std::map<std::string

		- 

	*
		- double>

		- 



.. rubric:: Returns:

measure result

.. index:: pair: function; real_chip_task
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a7705475bdf440a43a07c7258ec28ab06:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, double> real_chip_task(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		int shot,
		bool mapping_flag,
		bool circuit_optimization,
		bool is_vip,
		size_t chipid = 0
		)

run a measure quantum program



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- int&

		- shot

	*
		- std::map<std::string

		- 

	*
		- double>

		- 



.. rubric:: Returns:

measure result

.. index:: pair: function; get_state_tomography_density
.. _doxid-class_q_panda_1_1_q_cloud_machine_1aa47e1e5e32624ceb6c42acfc3012c0d1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`> get_state_tomography_density(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, int shot, size_t chipid = 0)

get real chip qst matrix



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the reference to a quantum program

	*
		- int&

		- shot

	*
		- QStat

		- matrix



.. rubric:: Returns:

matrix

.. index:: pair: function; get_result_json
.. _doxid-class_q_panda_1_1_q_cloud_machine_1a32e95a44728a06c2aa2c24a17e31845c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string get_result_json(std::string taskid, :ref:`CLOUD_QMACHINE_TYPE<doxid-namespace_q_panda_1abd0ad768e93ef08e8cfabd780d803863>` type)

get task result



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- taskid

	*
		- CLOUD_QMACHINE_TYPE

		- type

	*
		- std::string&

		- empty taskid



.. rubric:: Returns:

string

