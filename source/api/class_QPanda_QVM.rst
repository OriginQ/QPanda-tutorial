.. index:: pair: class; QPanda::QVM
.. _doxid-class_q_panda_1_1_q_v_m:

class QPanda::QVM
=================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class QVM: public :ref:`QPanda::QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`
	{
	public:
		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_q_v_m_1af3506b5b2b35451a8aae7364193f2843>`(size_t);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_q_v_m_1ae1f3ad0f3880eaada1101df5f6cc14f6>`(size_t);
		virtual :ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* :ref:`getStatus<doxid-class_q_panda_1_1_q_v_m_1a2fbdc658f90b541abd43934c93257b10>`() const;
		virtual :ref:`QResult<doxid-class_q_panda_1_1_q_result>`* :target:`getResult<doxid-class_q_panda_1_1_q_v_m_1acd345a3ebac094ceb9e685971672fa81>`();
		virtual std::map<std::string, bool> :target:`getResultMap<doxid-class_q_panda_1_1_q_v_m_1aea2b65cd9c75d21d6c3201ab9c7deb3c>`();
		virtual void :ref:`finalize<doxid-class_q_panda_1_1_q_v_m_1ae1fdcd040b4c6612bbe684a606668453>`();
		virtual std::map<std::string, bool> :ref:`directlyRun<doxid-class_q_panda_1_1_q_v_m_1adcf36345640beff726ad3fc6bb49c15b>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg);
		virtual std::map<std::string, size_t> :ref:`runWithConfiguration<doxid-class_q_panda_1_1_q_v_m_1a72948f788f8630b0eeffd987cf475a46>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, rapidjson::Document&);
		virtual std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t> :ref:`getGateTimeMap<doxid-class_q_panda_1_1_q_v_m_1ab5b2509d10ba71c908190eb8b5ef5385>`() const;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_panda_1_1_q_v_m_1a8b2d34ed071e6c9a2450a692e80fc855>`() const;
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_q_v_m_1a741a08893001a17609839f50a71f9535>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const;
		virtual bool :ref:`swapQubitPhysicalAddress<doxid-class_q_panda_1_1_q_v_m_1a4b9d45dc4072ea7dc4e507fbcf6e5567>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual void :target:`set_random_engine<doxid-class_q_panda_1_1_q_v_m_1afb372ab384b1ec6791addc1af36d8ad5>`(:ref:`RandomEngine<doxid-class_random_engine>`* rng);
		virtual void :target:`setConfig<doxid-class_q_panda_1_1_q_v_m_1a3a098815442fa6dc4b322e58b8e2bdc6>`(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`& config);
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
	};

	// direct descendants

	class :ref:`IdealQVM<doxid-class_q_panda_1_1_ideal_q_v_m>`;
	class :ref:`NoiseQVM<doxid-class_q_panda_1_1_noise_q_v_m>`;
	class :ref:`PartialAmplitudeQVM<doxid-class_q_panda_1_1_partial_amplitude_q_v_m>`;
	class :ref:`SingleAmplitudeQVM<doxid-class_q_panda_1_1_single_amplitude_q_v_m>`;

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

.. _details-class_q_panda_1_1_q_v_m:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; allocateQubitThroughPhyAddress
.. _doxid-class_q_panda_1_1_q_v_m_1af3506b5b2b35451a8aae7364193f2843:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughPhyAddress(size_t)

allocateQubitThroughPhyAddress



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- address



.. rubric:: Returns:

:ref:`QPanda::Qubit <doxid-class_q_panda_1_1_qubit>` \* qubit

.. index:: pair: function; allocateQubitThroughVirAddress
.. _doxid-class_q_panda_1_1_q_v_m_1ae1f3ad0f3880eaada1101df5f6cc14f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughVirAddress(size_t)

allocateQubitThroughVirAddress



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- address



.. rubric:: Returns:

:ref:`QPanda::Qubit <doxid-class_q_panda_1_1_qubit>` \* qubit

.. index:: pair: function; getStatus
.. _doxid-class_q_panda_1_1_q_v_m_1a2fbdc658f90b541abd43934c93257b10:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* getStatus() const

getStatus



.. rubric:: Returns:

:ref:`QPanda::QMachineStatus <doxid-class_q_panda_1_1_q_machine_status>` \*

.. index:: pair: function; finalize
.. _doxid-class_q_panda_1_1_q_v_m_1ae1fdcd040b4c6612bbe684a606668453:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void finalize()

finalize



.. rubric:: Returns:

void

.. index:: pair: function; directlyRun
.. _doxid-class_q_panda_1_1_q_v_m_1adcf36345640beff726ad3fc6bb49c15b:

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

.. index:: pair: function; runWithConfiguration
.. _doxid-class_q_panda_1_1_q_v_m_1a72948f788f8630b0eeffd987cf475a46:

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

.. index:: pair: function; getGateTimeMap
.. _doxid-class_q_panda_1_1_q_v_m_1ab5b2509d10ba71c908190eb8b5ef5385:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t> getGateTimeMap() const

getGateTimeMap



.. rubric:: Returns:

std::map<GateType, Eigen::size_t>

.. index:: pair: function; getQState
.. _doxid-class_q_panda_1_1_q_v_m_1a8b2d34ed071e6c9a2450a692e80fc855:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getQState() const

getQState



.. rubric:: Returns:

QStat

.. index:: pair: function; getVirtualQubitAddress
.. _doxid-class_q_panda_1_1_q_v_m_1a741a08893001a17609839f50a71f9535:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getVirtualQubitAddress(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const

getVirtualQubitAddress



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- qubit



.. rubric:: Returns:

Eigen::size_t

.. index:: pair: function; swapQubitPhysicalAddress
.. _doxid-class_q_panda_1_1_q_v_m_1a4b9d45dc4072ea7dc4e507fbcf6e5567:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool swapQubitPhysicalAddress(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

swapQubitPhysicalAddress



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- qubit

	*
		- Qubit\*

		- qubit



.. rubric:: Returns:

bool

.. index:: pair: function; allocateQubit
.. _doxid-class_q_panda_1_1_q_v_m_1ab42756f84764948ff31b4d87c79d3e43:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubit()

To initialize the quantum machine.

.. index:: pair: function; allocateQubits
.. _doxid-class_q_panda_1_1_q_v_m_1a1dd87950e34b38f83452e98f3a548f05:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` allocateQubits(size_t)

Allocate and return a qubit.

.. index:: pair: function; allocateCBit
.. _doxid-class_q_panda_1_1_q_v_m_1a5379b3b9ed124ae76e5b365429132304:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` allocateCBit()

allocateQubits

.. index:: pair: function; allocateCBits
.. _doxid-class_q_panda_1_1_q_v_m_1a9907e505e82030f4af78c2fce231fd4b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> allocateCBits(size_t)

Allocate and run a cbit.

.. index:: pair: function; allocateCBit
.. _doxid-class_q_panda_1_1_q_v_m_1ac9cfc237aaa20194ae4a6afc8095da8a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` allocateCBit(size_t)

Allocate and run a cbit.

.. index:: pair: function; getAllocateQubit
.. _doxid-class_q_panda_1_1_q_v_m_1aac63304751354d973d150466936ef5b5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateQubit()

Gree a list of CBits.

.. index:: pair: function; getAllocateCMem
.. _doxid-class_q_panda_1_1_q_v_m_1af9a55a93940aade484f02cbd9831f769:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateCMem()

getAllocateQubit

.. index:: pair: function; Free_Qubit
.. _doxid-class_q_panda_1_1_q_v_m_1a9938820e903ad8944ac18e8fc12d10bd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

Allocate and return a list of cbits.

.. index:: pair: function; Free_Qubits
.. _doxid-class_q_panda_1_1_q_v_m_1abc0663c135f5227d694bc4f20a982531:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubits(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&)

Free a qubit.

.. index:: pair: function; Free_CBit
.. _doxid-class_q_panda_1_1_q_v_m_1a8d3af5eafe432611cfcadf3319a674af:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_CBit(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&)

Gree a list of qubits.

.. index:: pair: function; Free_CBits
.. _doxid-class_q_panda_1_1_q_v_m_1a50dc95283f276e7de241ae4a95d55988:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_CBits(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&)

Gree a cbit.

.. index:: pair: function; setConfigure
.. _doxid-class_q_panda_1_1_q_v_m_1ad344c02cad43a5d3d451d55853d378a2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setConfigure(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`&)

getAllocateCMem

setConfigure



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- :ref:`Configuration <doxid-struct_q_panda_1_1_configuration>` & config



.. rubric:: Returns:

void

.. index:: pair: function; qAlloc
.. _doxid-class_q_panda_1_1_q_v_m_1ad9de2e6468b65d4e5f97ece36498a7c9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qAlloc()

To initialize the quantum machine.

.. index:: pair: function; qAllocMany
.. _doxid-class_q_panda_1_1_q_v_m_1ab1c3644b4253ca991421b2e0c90a94e7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qAllocMany(size_t qubit_count)

Allocate and return a qubit.

.. index:: pair: function; cAlloc
.. _doxid-class_q_panda_1_1_q_v_m_1a0cf8de6f2957639bd4d66ab2f148d295:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` cAlloc()

allocateQubits

.. index:: pair: function; cAlloc
.. _doxid-class_q_panda_1_1_q_v_m_1a698dbdafc368dbb092b51b565f03f63d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` cAlloc(size_t)

Allocate and run a cbit.

.. index:: pair: function; cAllocMany
.. _doxid-class_q_panda_1_1_q_v_m_1ad0d83c214ff3c53aa15e929e61d23665:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> cAllocMany(size_t)

Allocate and run a cbit.

.. index:: pair: function; qFree
.. _doxid-class_q_panda_1_1_q_v_m_1af00ee41c463d9c45d1148d94c5b721f3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void qFree(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

Allocate and return a list of cbits.

.. index:: pair: function; qFreeAll
.. _doxid-class_q_panda_1_1_q_v_m_1a265c6b00fa422d5dea5f02c0a06ff085:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void qFreeAll(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&)

Free a qubit.

.. index:: pair: function; cFree
.. _doxid-class_q_panda_1_1_q_v_m_1a9d1b31118208791c67e5bd799877f175:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void cFree(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&)

Gree a list of qubits.

.. index:: pair: function; cFreeAll
.. _doxid-class_q_panda_1_1_q_v_m_1a9b9e59e08e47272d70f10681fb380fa1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void cFreeAll(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&)

Gree a cbit.

.. index:: pair: function; getAllocateQubitNum
.. _doxid-class_q_panda_1_1_q_v_m_1a268030f1c16325f7496f0eef3efb5533:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateQubitNum()

Gree a list of CBits.

.. index:: pair: function; getAllocateCMemNum
.. _doxid-class_q_panda_1_1_q_v_m_1aba6a435098a6e9d1c6d50948f3f7cbdb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateCMemNum()

getAllocateQubit

