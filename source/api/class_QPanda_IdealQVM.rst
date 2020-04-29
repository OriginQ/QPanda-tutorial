.. index:: pair: class; QPanda::IdealQVM
.. _doxid-class_q_panda_1_1_ideal_q_v_m:

class QPanda::IdealQVM
======================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class IdealQVM:
	    public :ref:`QPanda::QVM<doxid-class_q_panda_1_1_q_v_m>`,
	    public :ref:`QPanda::IdealMachineInterface<doxid-class_q_panda_1_1_ideal_machine_interface>`
	{
	public:
		// methods
	
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`getProbTupleList<doxid-class_q_panda_1_1_ideal_q_v_m_1ac277981f90de32016cf5f4ada862a22f>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			);
	
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`getProbList<doxid-class_q_panda_1_1_ideal_q_v_m_1a6fdd9de59267900ba56d2f69537fbe74>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			);
	
		virtual :ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :target:`getProbDict<doxid-class_q_panda_1_1_ideal_q_v_m_1ad8e41ae0d67884720745c0685a21b443>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			);
	
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`probRunTupleList<doxid-class_q_panda_1_1_ideal_q_v_m_1aaef23e9ba96e0d0235070c496db189c4>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			);
	
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`probRunList<doxid-class_q_panda_1_1_ideal_q_v_m_1a11f2f3f0a8f6cff471437634ae49c524>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			);
	
		virtual :ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :target:`probRunDict<doxid-class_q_panda_1_1_ideal_q_v_m_1a94298c6fa0e874c67a0c857692120841>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			);
	
		virtual std::map<std::string, size_t> :target:`quickMeasure<doxid-class_q_panda_1_1_ideal_q_v_m_1a18ea01f604d592b31452f2315a315b39>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			size_t
			);
	
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`getQStat<doxid-class_q_panda_1_1_ideal_q_v_m_1a788fc57dd756d9571a708846f7a28bc5>`();
	
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`PMeasure<doxid-class_q_panda_1_1_ideal_q_v_m_1affe243c1304a0265d680eb9f7752fc6e>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector,
			int select_max
			);
	
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`PMeasure_no_index<doxid-class_q_panda_1_1_ideal_q_v_m_1a38e04d19c75140763c31793fc6156a8d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector);
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`getQState<doxid-class_q_panda_1_1_ideal_q_v_m_1a9cb74f452d905bbf1cde7dc566afee89>`();
	
		:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`pMeasure<doxid-class_q_panda_1_1_ideal_q_v_m_1a8f572abda4a7a6d988ba007f17e941e6>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector,
			int select_max
			);
	
		:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`pMeasureNoIndex<doxid-class_q_panda_1_1_ideal_q_v_m_1a3081b22d10660711d49f00e92d31ff2b>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector);
	};

	// direct descendants

	class :ref:`CPUQVM<doxid-class_q_panda_1_1_c_p_u_q_v_m>`;
	class :ref:`CPUSingleThreadQVM<doxid-class_q_panda_1_1_c_p_u_single_thread_q_v_m>`;
	class :ref:`GPUQVM<doxid-class_q_panda_1_1_g_p_u_q_v_m>`;

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
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_q_v_m_1af3506b5b2b35451a8aae7364193f2843>`(size_t);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_q_v_m_1ae1f3ad0f3880eaada1101df5f6cc14f6>`(size_t);
		virtual :ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* :ref:`getStatus<doxid-class_q_panda_1_1_q_v_m_1a2fbdc658f90b541abd43934c93257b10>`() const;
		virtual :ref:`QResult<doxid-class_q_panda_1_1_q_result>`* :ref:`getResult<doxid-class_q_panda_1_1_q_v_m_1acd345a3ebac094ceb9e685971672fa81>`();
		virtual std::map<std::string, bool> :ref:`getResultMap<doxid-class_q_panda_1_1_q_v_m_1aea2b65cd9c75d21d6c3201ab9c7deb3c>`();
		virtual void :ref:`finalize<doxid-class_q_panda_1_1_q_v_m_1ae1fdcd040b4c6612bbe684a606668453>`();
		virtual std::map<std::string, bool> :ref:`directlyRun<doxid-class_q_panda_1_1_q_v_m_1adcf36345640beff726ad3fc6bb49c15b>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg);
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_q_v_m_1a72948f788f8630b0eeffd987cf475a46>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, rapidjson::Document&);
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
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`PMeasure_no_index<doxid-class_q_panda_1_1_ideal_machine_interface_1aa1908bd072b61280a985f26369d574e5>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector) = 0;
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`getProbTupleList<doxid-class_q_panda_1_1_ideal_machine_interface_1a0d5e3fdae0eebcf046081eb1557f418c>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, int) = 0;
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`getProbList<doxid-class_q_panda_1_1_ideal_machine_interface_1a4d3b351174020e7d36fdc6b3af805052>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, int) = 0;
		virtual :ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`getProbDict<doxid-class_q_panda_1_1_ideal_machine_interface_1a10941c69eb843f04949bff4ac272751f>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, int) = 0;
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`probRunTupleList<doxid-class_q_panda_1_1_ideal_machine_interface_1ad54eae1ebb20721628bdfebfd0cd732e>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, int) = 0;
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`probRunList<doxid-class_q_panda_1_1_ideal_machine_interface_1a9cc21ede35f892116f87e6697f2f4034>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, int) = 0;
		virtual :ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`probRunDict<doxid-class_q_panda_1_1_ideal_machine_interface_1a26484905dcc5faafa905c30246c7231f>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, int) = 0;
		virtual std::map<std::string, size_t> :ref:`quickMeasure<doxid-class_q_panda_1_1_ideal_machine_interface_1adb5cf9a4ee37f1d74dc38ceee26a5033>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, size_t) = 0;
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`PMeasure<doxid-class_q_panda_1_1_ideal_machine_interface_1ad0519fea1275272071948226776df69b>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector, int select_max) = 0;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQStat<doxid-class_q_panda_1_1_ideal_machine_interface_1ac83e01310fc24e27ce7b1c6fac41138b>`() = 0;

