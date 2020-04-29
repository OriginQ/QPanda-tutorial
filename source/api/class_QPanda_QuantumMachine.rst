.. index:: pair: class; QPanda::QuantumMachine
.. _doxid-class_q_panda_1_1_quantum_machine:

class QPanda::QuantumMachine
============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Abstract quantum machine base classes. :ref:`More...<details-class_q_panda_1_1_quantum_machine>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMachineInterface.h>
	
	class QuantumMachine
	{
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
		virtual void :target:`setConfig<doxid-class_q_panda_1_1_quantum_machine_1a1f32aa1b5d33961b1a33a7a5c5c61be5>`(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`&) = 0;
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
	};

	// direct descendants

	class :ref:`QVM<doxid-class_q_panda_1_1_q_v_m>`;
.. _details-class_q_panda_1_1_quantum_machine:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Abstract quantum machine base classes.

Methods
-------

.. index:: pair: function; allocateQubitThroughPhyAddress
.. _doxid-class_q_panda_1_1_quantum_machine_1a732d439bfb76b74edb3d2404568a1900:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughPhyAddress(size_t) = 0

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
.. _doxid-class_q_panda_1_1_quantum_machine_1a2352ae1e515dad9a445a59069a42161e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughVirAddress(size_t) = 0

allocateQubitThroughVirAddress



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- address



.. rubric:: Returns:

:ref:`QPanda::Qubit <doxid-class_q_panda_1_1_qubit>` \* qubit

.. index:: pair: function; init
.. _doxid-class_q_panda_1_1_quantum_machine_1ac2ebbb77482669f310f9b5d0b6f30fa1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void init() = 0

init



.. rubric:: Returns:

void

.. index:: pair: function; getStatus
.. _doxid-class_q_panda_1_1_quantum_machine_1a29299cd9882a2f5016971121a58fa679:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* getStatus() const = 0

getStatus



.. rubric:: Returns:

:ref:`QPanda::QMachineStatus <doxid-class_q_panda_1_1_q_machine_status>` \*

.. index:: pair: function; directlyRun
.. _doxid-class_q_panda_1_1_quantum_machine_1a77357644931b71be480590764df59451:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, bool> directlyRun(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg) = 0

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
.. _doxid-class_q_panda_1_1_quantum_machine_1a7dded3823353840ab733abdc3fb999b2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<std::string, size_t> runWithConfiguration(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&,
		rapidjson::Document&
		) = 0

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
.. _doxid-class_q_panda_1_1_quantum_machine_1a9caf6ddc2d278e222db50b78ff6d5a03:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, size_t> getGateTimeMap() const = 0

getGateTimeMap



.. rubric:: Returns:

std::map<GateType, Eigen::size_t>

.. index:: pair: function; finalize
.. _doxid-class_q_panda_1_1_quantum_machine_1a2aff067ba64013dce87814dfdfbdc176:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void finalize() = 0

finalize



.. rubric:: Returns:

void

.. index:: pair: function; getQState
.. _doxid-class_q_panda_1_1_quantum_machine_1aee285b6b7f5cd7936491f2b304501167:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getQState() const = 0

getQState



.. rubric:: Returns:

QStat

.. index:: pair: function; getVirtualQubitAddress
.. _doxid-class_q_panda_1_1_quantum_machine_1ae01f52fad0cde4e96dbc4945e3f6f93f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getVirtualQubitAddress(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const = 0

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
.. _doxid-class_q_panda_1_1_quantum_machine_1a8f444f30f7675ee5e1e2c7db53264b7d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool swapQubitPhysicalAddress(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0

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
.. _doxid-class_q_panda_1_1_quantum_machine_1a0b8228ea18d362fba29ff5fcdded60b4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubit() = 0

To initialize the quantum machine.

.. index:: pair: function; allocateQubits
.. _doxid-class_q_panda_1_1_quantum_machine_1a190cd3e9af3aa1a34420b91e2f60f60a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` allocateQubits(size_t) = 0

Allocate and return a qubit.

.. index:: pair: function; allocateCBit
.. _doxid-class_q_panda_1_1_quantum_machine_1a944298196e0c6dbf6e641395af82f4c9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` allocateCBit() = 0

allocateQubits

.. index:: pair: function; allocateCBit
.. _doxid-class_q_panda_1_1_quantum_machine_1a1c95eb9d941db948d60767a460aa20d0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` allocateCBit(size_t) = 0

Allocate and run a cbit.

.. index:: pair: function; allocateCBits
.. _doxid-class_q_panda_1_1_quantum_machine_1a5ab5745be7c1c4fc44a928fdbf1c87e1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> allocateCBits(size_t) = 0

Allocate and run a cbit.

.. index:: pair: function; Free_Qubit
.. _doxid-class_q_panda_1_1_quantum_machine_1a480d3b51048e1e8923bef9325d5f524d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0

Allocate and return a list of cbits.

.. index:: pair: function; Free_Qubits
.. _doxid-class_q_panda_1_1_quantum_machine_1a933fe5bcb93118dfad9d096676885eb7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubits(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0

Free a qubit.

.. index:: pair: function; Free_CBit
.. _doxid-class_q_panda_1_1_quantum_machine_1a42f5901a2104eefe29e9ff276076eb08:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_CBit(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&) = 0

Gree a list of qubits.

.. index:: pair: function; Free_CBits
.. _doxid-class_q_panda_1_1_quantum_machine_1a331c9a57d8af8769f8c6332529b7b043:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_CBits(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0

Gree a cbit.

.. index:: pair: function; getAllocateQubit
.. _doxid-class_q_panda_1_1_quantum_machine_1a98784101fb0ae8d98d1fd311a39689b8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateQubit() = 0

Gree a list of CBits.

.. index:: pair: function; getAllocateCMem
.. _doxid-class_q_panda_1_1_quantum_machine_1aabf896ec46e67498900467a38ddaee7c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateCMem() = 0

getAllocateQubit

.. index:: pair: function; setConfigure
.. _doxid-class_q_panda_1_1_quantum_machine_1a2e780aea11e55ee381c0ae983f65291d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setConfigure(const :ref:`Configuration<doxid-struct_q_panda_1_1_configuration>`&) = 0

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
.. _doxid-class_q_panda_1_1_quantum_machine_1a8d41c197973a4c544928facdd9b80e05:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qAlloc() = 0

qAlloc



.. rubric:: Returns:

:ref:`QPanda::Qubit <doxid-class_q_panda_1_1_qubit>` \* qubit

.. index:: pair: function; qAllocMany
.. _doxid-class_q_panda_1_1_quantum_machine_1ae1ed8d4a83d8167a111992245016f6e8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qAllocMany(size_t qubit_count) = 0

qAllocMany



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit_count



.. rubric:: Returns:

:ref:`QPanda::QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; cAlloc
.. _doxid-class_q_panda_1_1_quantum_machine_1aa6e93c19e315072799915d4f9b02223f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` cAlloc() = 0

cAlloc



.. rubric:: Returns:

:ref:`QPanda::ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; cAlloc
.. _doxid-class_q_panda_1_1_quantum_machine_1ad7ebf59186a299d850ddf4ac3eeebaf1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` cAlloc(size_t) = 0

cAlloc



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- 



.. rubric:: Returns:

:ref:`QPanda::ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; cAllocMany
.. _doxid-class_q_panda_1_1_quantum_machine_1a0aeb0517f0dc84b9b9bbb100c87430dc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> cAllocMany(size_t) = 0

cAllocMany



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- count



.. rubric:: Returns:

std::vector<QPanda::ClassicalCondition> cbit_vec

.. index:: pair: function; qFree
.. _doxid-class_q_panda_1_1_quantum_machine_1a5a61e36151d84476f64d66337435a2c1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void qFree(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0

qFree



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- 



.. rubric:: Returns:

void

.. index:: pair: function; qFreeAll
.. _doxid-class_q_panda_1_1_quantum_machine_1afc3c5771b37a13c0ebd65a940029c9fb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void qFreeAll(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0

qFreeAll



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- 



.. rubric:: Returns:

void

.. index:: pair: function; cFree
.. _doxid-class_q_panda_1_1_quantum_machine_1a3d96ab037bdfe79a6cd32d394d51c3b0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void cFree(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&) = 0

cFree



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ClassicalCondition&

		- cbit



.. rubric:: Returns:

void

.. index:: pair: function; cFreeAll
.. _doxid-class_q_panda_1_1_quantum_machine_1a2912a9f37c8600d8d0fc875eeca402d5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void cFreeAll(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0

cFreeAll



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<ClassicalCondition

		- >& cbit_vec



.. rubric:: Returns:

void

.. index:: pair: function; getAllocateQubitNum
.. _doxid-class_q_panda_1_1_quantum_machine_1a66fe7b76e261cde0b4571fc796107fcc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateQubitNum() = 0

getAllocateQubitNum



.. rubric:: Returns:

Eigen::size_t count

.. index:: pair: function; getAllocateCMemNum
.. _doxid-class_q_panda_1_1_quantum_machine_1ac49cf7c186b153bc277e2505efce9344:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getAllocateCMemNum() = 0

getAllocateCMemNum



.. rubric:: Returns:

Eigen::size_t count

