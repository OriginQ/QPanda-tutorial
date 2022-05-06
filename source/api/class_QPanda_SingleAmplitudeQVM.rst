.. index:: pair: class; QPanda::SingleAmplitudeQVM
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m:

class QPanda::SingleAmplitudeQVM
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum machine for single amplitude simulation. :ref:`More...<details-class_q_panda_1_1_single_amplitude_q_v_m>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <SingleAmplitudeQVM.h>
	
	class SingleAmplitudeQVM:
	    public :ref:`QPanda::QVM<doxid-class_q_panda_1_1_q_v_m>`,
	    public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		virtual void :ref:`init<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1ac0f906d961b7823a0ebf46d9811a0719>`();
		void :ref:`run<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a59317db84cdedfac78f9d45b8c172335>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, size_t max_rank = 30, size_t alloted_time = 5);
		void :ref:`run<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a1667931ed1725b4e03cd77d3c7a5d06d>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, size_t max_rank, const std::vector<:ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`>& sequences);
		size_t :ref:`getSequence<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1ae201333b87affa9de36b5f7832d8ef93>`(const std::vector<size_t>& quickbb_vertice, std::vector<:ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`>& sequence_vec);
		void :target:`getQuickMapVertice<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a1c0658ec67bc19c0961e66dadf0c504e>`(std::vector<std::pair<size_t, size_t>>& map_vector);
		:ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>` :ref:`pMeasureBinindex<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a88a7e83db80d771fee56fd89a885ac1d>`(std::string index);
		:ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>` :ref:`pMeasureDecindex<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1adab416607edb0b2191fcf88052590a39>`(std::string index);
		:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`getProbDict<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a98fb346bd3ee3bf0e6d93a905fc3d456>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qlist);
		:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`probRunDict<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1aee0d2c0faaa3ebe70cb250f2fad7d339>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qlist);
		:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :target:`getProbDict<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a7eae02e799312ac458fbfadf9f735a22>`(const std::vector<int>& qaddrs_list);
	
		:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :target:`probRunDict<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1abc2d3da5648b012284bd343dd1b19ae3>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			const std::vector<int>& qaddrs_list
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a792c67343653b64a2872e373822e55cc>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool& is_dagger
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a7ae8a4bfb4e2f8fcacd855075f6f8698>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool& is_dagger
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a3b7ee8f5583ae328b35540d9f9eff7dc>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool& is_dagger
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a3e20d19aac30b79d0c93e182a7d007d1>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool& is_dagger
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a3c37ada05f25ecca32dc70e8073866bd>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool& is_dagger
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1aefd949c3fdb34bf1229e00f0d8bd20be>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool& is_dagger
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a83535579fe520d392dde29f6b7d79fff>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool& is_dagger
			);
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

.. _details-class_q_panda_1_1_single_amplitude_q_v_m:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum machine for single amplitude simulation.



.. rubric:: See also:

:ref:`QuantumMachine <doxid-class_q_panda_1_1_quantum_machine>`

Methods
-------

.. index:: pair: function; init
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1ac0f906d961b7823a0ebf46d9811a0719:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void init()

init



.. rubric:: Returns:

void

.. index:: pair: function; run
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a59317db84cdedfac78f9d45b8c172335:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void run(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, size_t max_rank = 30, size_t alloted_time = 5)

run



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QVec&

		- qubits vector

	*
		- size_t

		- rank number

	*
		- size_t

		- run :ref:`QuickBB <doxid-class_quick_b_b>` alloted time

.. index:: pair: function; run
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a1667931ed1725b4e03cd77d3c7a5d06d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void run(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, size_t max_rank, const std::vector<:ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`>& sequences)

run



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QVec&

		- qubits vector

	*
		- size_t

		- rank number

	*
		- size_t

		- quantum program contraction sequence

.. index:: pair: function; getSequence
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1ae201333b87affa9de36b5f7832d8ef93:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t getSequence(
		const std::vector<size_t>& quickbb_vertice,
		std::vector<:ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`>& sequence_vec
		)

get quantum program contraction sequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- std::vector<size_t>& quickbb vertice

	*
		- std::vector<qprog_sequence_t>&

		- quantum program contraction sequence



.. rubric:: Returns:

size_t sequence number

.. index:: pair: function; pMeasureBinindex
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a88a7e83db80d771fee56fd89a885ac1d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>` pMeasureBinindex(std::string index)

PMeasure by binary index.

example: pMeasureBinindex("0000000000")



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- binary index



.. rubric:: Returns:

qstate_type double

.. index:: pair: function; pMeasureDecindex
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1adab416607edb0b2191fcf88052590a39:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`qstate_type<doxid-_q_panda_namespace_8h_1ad41e917590ba0a7303522998805aaa9f>` pMeasureDecindex(std::string index)

PMeasure by decimal index.

example: pMeasureDecindex("1")



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- decimal index



.. rubric:: Returns:

qstate_type double

.. index:: pair: function; getProbDict
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1a98fb346bd3ee3bf0e6d93a905fc3d456:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` getProbDict(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qlist)

get probability by qubits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>` & qubits vector



.. rubric:: Returns:

prob_dict

.. index:: pair: function; probRunDict
.. _doxid-class_q_panda_1_1_single_amplitude_q_v_m_1aee0d2c0faaa3ebe70cb250f2fad7d339:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` probRunDict(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qlist)

get probability by qubits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program

	*
		- QVec&

		- qubits vector



.. rubric:: Returns:

prob_dict

