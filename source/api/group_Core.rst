.. index:: pair: group; Core
.. _doxid-group___core:

Core
====

.. toctree::
	:hidden:

	group_QuantumCircuit.rst
	group_QuantumMachine.rst
	group_Utilities.rst
	group_Variational.rst
	group_VirtualQuantumProcessor.rst

Overview
~~~~~~~~

QPanda2 Core Group. :ref:`More...<details-group___core>`

|	:ref:`QuantumCircuit<doxid-group___quantum_circuit>`
|	:ref:`QuantumMachine<doxid-group___quantum_machine>`
|	:ref:`Utilities<doxid-group___utilities>`
|	:ref:`Variational<doxid-group___variational>`
|	:ref:`VirtualQuantumProcessor<doxid-group___virtual_quantum_processor>`



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	bool :ref:`QPanda::init<doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>`(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type = :ref:`CPU<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13aea39cfc1ace612a8e2c4da2c62ae5659>`);
	void :ref:`QPanda::finalize<doxid-group___core_1gacd2f5cfc79160543f03c5bef34d27185>`();
	:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`QPanda::qAlloc<doxid-group___core_1ga9a81705d142b143260f86f742adf0d86>`();
	:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`QPanda::qAlloc<doxid-group___core_1ga2a307b5ad8cdee51c52bdbf0d299e509>`(size_t stQubitAddr);
	std::map<std::string, bool> :ref:`QPanda::directlyRun<doxid-group___core_1ga65ef685dd053d017b2f9e48f38c03370>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg);
	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`QPanda::qAllocMany<doxid-group___core_1ga9dcf62b20ef64d5b561e7919e7903a97>`(size_t stQubitNumber);
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`QPanda::cAlloc<doxid-group___core_1ga5fcf81bd208ecf4ba4e53249599fdb4d>`();
	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` :ref:`QPanda::cAlloc<doxid-group___core_1ga792cdfc228747df979116019ab869dca>`(size_t stCBitaddr);
	std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :ref:`QPanda::cAllocMany<doxid-group___core_1ga820833650151100c4a29aafc2f345863>`(size_t stCBitNumber);
	void :ref:`QPanda::cFree<doxid-group___core_1ga95bc1fb6ac649bd590680a2676e71ea6>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&);
	void :ref:`QPanda::cFreeAll<doxid-group___core_1gaa438f340325085ab44936e0413c2d40d>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> vCBit);
	:ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* :ref:`QPanda::getstat<doxid-group___core_1ga2dcbb445a1e5c3b5cdec9b44e1325096>`();
	size_t :ref:`QPanda::getAllocateQubitNum<doxid-group___core_1ga9f99c54c66e54057d1f635b0bf4ed26e>`();
	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`QPanda::getProbTupleList<doxid-group___core_1ga9f7eb33268e651402871173ad289f201>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`QPanda::getProbList<doxid-group___core_1ga37ce2c0c342a9dce0293c31412179e56>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`QPanda::getProbDict<doxid-group___core_1gac7d6f9130bb14da46068f669cbeb786f>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`QPanda::probRunTupleList<doxid-group___core_1ga940377aac8c4e06aa93b6d9ad1ca44c6>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`QPanda::probRunList<doxid-group___core_1ga8b769442bdd06bce0bd573dfa0b86125>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :ref:`QPanda::probRunDict<doxid-group___core_1gaad2d0834f62ae9c4b18573c7e8a50922>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1);
	std::map<std::string, size_t> :ref:`QPanda::runWithConfiguration<doxid-group___core_1gaac240d65f6c9c0e955a583b7d7a7735b>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&, int);
	std::map<std::string, size_t> :ref:`QPanda::quickMeasure<doxid-group___core_1gaaaf64d793f51d39ead7ceba1cf7d6d01>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`QPanda::accumulateProbability<doxid-group___core_1gab7fa40c4a3d8d4b6c9dc5a5bf389162f>`(:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& prob_list);

	std::map<std::string, size_t> :ref:`QPanda::quick_measure<doxid-group___core_1gabbf7eea831182a82092f70285c027d42>`(
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector,
		int shots,
		:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& accumulate_probabilites
		);

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`QPanda::getQState<doxid-group___core_1gacaafce8fec4c04e15a492fb695176bb1>`();
	:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* :ref:`QPanda::initQuantumMachine<doxid-group___core_1gab28a403fe4f2894e330ccd90e01295e4>`(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type = :ref:`CPU<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13aea39cfc1ace612a8e2c4da2c62ae5659>`);
	void :ref:`QPanda::destroyQuantumMachine<doxid-group___core_1ga40086744d5e1d0ee04381ebd63ae40c7>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm);
	:ref:`QPanda::QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::MeasureAll<doxid-group___core_1ga5d448b1c38b2b3a13022c5c3a3587b40>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>);
	size_t :ref:`QPanda::getAllocateCMemNum<doxid-group___core_1gaa455e0e99622f5f997c6931981bb33ea>`();
	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`QPanda::pMeasure<doxid-group___core_1ga3c19a648c8c21b9b8819b1c8180f20c0>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector, int select_max);
	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :ref:`QPanda::pMeasureNoIndex<doxid-group___core_1ga44c86a2a14f084483580f898a70e6a20>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector);
	:ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` :ref:`QPanda::Measure<doxid-group___core_1ga15b15ba85d24d7355880ad63fd4c2107>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`);

.. _details-group___core:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPanda2 Core Group.

Global Functions
----------------

.. index:: pair: function; init
.. _doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool QPanda::init(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type = :ref:`CPU<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13aea39cfc1ace612a8e2c4da2c62ae5659>`)

Init the environment.

Use this at the beginning



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QMachineType

		- Quantum machine type



.. rubric:: Returns:

bool



.. rubric:: See also:

:ref:`QMachineType <doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>`

.. index:: pair: function; finalize
.. _doxid-group___core_1gacd2f5cfc79160543f03c5bef34d27185:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::finalize()

Finalize the environment.

Use this at the end



.. rubric:: Returns:

void

.. index:: pair: function; qAlloc
.. _doxid-group___core_1ga9a81705d142b143260f86f742adf0d86:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* QPanda::qAlloc()

Allocate a qubit.

Call :ref:`init() <doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>` before you use this



.. rubric:: Returns:

void

.. index:: pair: function; qAlloc
.. _doxid-group___core_1ga2a307b5ad8cdee51c52bdbf0d299e509:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* QPanda::qAlloc(size_t stQubitAddr)

Allocate a qubit.

Call :ref:`init() <doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>` before you use this



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- set qubit address



.. rubric:: Returns:

void

.. index:: pair: function; directlyRun
.. _doxid-group___core_1ga65ef685dd053d017b2f9e48f38c03370:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, bool> QPanda::directlyRun(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& qProg)

Directly run a quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- Quantum program



.. rubric:: Returns:

std::map<std::string, bool> result

.. index:: pair: function; qAllocMany
.. _doxid-group___core_1ga9dcf62b20ef64d5b561e7919e7903a97:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` QPanda::qAllocMany(size_t stQubitNumber)

Allocate many qubits.

Call :ref:`init() <doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>` before you use this



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- set qubit number

.. index:: pair: function; cAlloc
.. _doxid-group___core_1ga5fcf81bd208ecf4ba4e53249599fdb4d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` QPanda::cAlloc()

Allocate a cbit.

Call :ref:`init() <doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>` before you use this



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` cbit

.. index:: pair: function; cAlloc
.. _doxid-group___core_1ga792cdfc228747df979116019ab869dca:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` QPanda::cAlloc(size_t stCBitaddr)

Allocate a cbit.

Call :ref:`init() <doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>` before you use this



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- set cbit address



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` Cbit

.. index:: pair: function; cAllocMany
.. _doxid-group___core_1ga820833650151100c4a29aafc2f345863:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> QPanda::cAllocMany(size_t stCBitNumber)

Allocate many cbits.

Call :ref:`init() <doxid-group___core_1gabc82d3c6d644397619115a284fd8fcc0>` before you use this



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- set cbit number

.. index:: pair: function; cFree
.. _doxid-group___core_1ga95bc1fb6ac649bd590680a2676e71ea6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::cFree(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&)

Free a cbit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ClassicalCondition&

		- a reference to a cbit



.. rubric:: Returns:

void

.. index:: pair: function; cFreeAll
.. _doxid-group___core_1gaa438f340325085ab44936e0413c2d40d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::cFreeAll(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> vCBit)

Free a list of cbits.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<ClassicalCondition>

		- a list of cbits



.. rubric:: Returns:

void

.. index:: pair: function; getstat
.. _doxid-group___core_1ga2dcbb445a1e5c3b5cdec9b44e1325096:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`* QPanda::getstat()

Get the status(ptr) of the Quantum machine.



.. rubric:: Returns:

:ref:`QPanda::QMachineStatus <doxid-class_q_panda_1_1_q_machine_status>` \* Quantum machine status(ptr)

.. index:: pair: function; getAllocateQubitNum
.. _doxid-group___core_1ga9f99c54c66e54057d1f635b0bf4ed26e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t QPanda::getAllocateQubitNum()

Get all allocate qubit num.



.. rubric:: Returns:

size_t :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` num

.. index:: pair: function; getProbTupleList
.. _doxid-group___core_1ga9f7eb33268e651402871173ad289f201:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` QPanda::getProbTupleList(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1)

Get pmeasure result as tuple list.

selectMax can not exceed (1ull << the size of qubits vector)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- pmeasure qubits vector

	*
		- int

		- Selectmax:the returned value num



.. rubric:: Returns:

std::vector<std::pair<size_t, double>> result

.. index:: pair: function; getProbList
.. _doxid-group___core_1ga37ce2c0c342a9dce0293c31412179e56:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` QPanda::getProbList(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1)

Get pmeasure result as list.

SelectMax can not exceed (1ull << the size of qubits vector)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- pmeasure qubits vector

	*
		- int

		- Selectmax:the returned value num



.. rubric:: Returns:

prob_vec result

.. index:: pair: function; getProbDict
.. _doxid-group___core_1gac7d6f9130bb14da46068f669cbeb786f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` QPanda::getProbDict(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1)

Get pmeasure result as dict.

SelectMax can not exceed (1ull << the size of qubits vector)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- pmeasure qubits vector

	*
		- int

		- Selectmax:the returned value num



.. rubric:: Returns:

std::map<std::string, double> result

.. index:: pair: function; probRunTupleList
.. _doxid-group___core_1ga940377aac8c4e06aa93b6d9ad1ca44c6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` QPanda::probRunTupleList(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1)

Get pmeasure result as dict.

SelectMax can not exceed (1ull << the size of qubits vector)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- Quantum program

	*
		- QVec&

		- pmeasure qubits vector

	*
		- int

		- Selectmax:the returned value num



.. rubric:: Returns:

std::vector<std::pair<size_t, double>> result

.. index:: pair: function; probRunList
.. _doxid-group___core_1ga8b769442bdd06bce0bd573dfa0b86125:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` QPanda::probRunList(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1)

Get pmeasure result as list.

SelectMax can not exceed (1ull << the size of qubits vector)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- Quantum program

	*
		- QVec&

		- Pmeasure qubits vector

	*
		- int

		- selectmax:the returned value num



.. rubric:: Returns:

prob_vec result

.. index:: pair: function; probRunDict
.. _doxid-group___core_1gaad2d0834f62ae9c4b18573c7e8a50922:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` QPanda::probRunDict(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int selectMax = -1)

Get pmeasure result as dict.

SelectMax can not exceed (1ull << the size of qubits vector)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- Quantum program

	*
		- QVec&

		- pmeasure qubits vector

	*
		- int

		- Selectmax:the returned value num



.. rubric:: Returns:

std::map<std::string, double> result

.. index:: pair: function; runWithConfiguration
.. _doxid-group___core_1gaac240d65f6c9c0e955a583b7d7a7735b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, size_t> QPanda::runWithConfiguration(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&,
		int
		)

Measure run with configuration.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- Quantum program

	*
		- std::vector<ClassicalCondition>&

		- cbits vector

	*
		- int

		- Shots:the repeat num of measure operate



.. rubric:: Returns:

std::map<std::string, size_t> result

.. index:: pair: function; quickMeasure
.. _doxid-group___core_1gaaaf64d793f51d39ead7ceba1cf7d6d01:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, size_t> QPanda::quickMeasure(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&, int)

Quick measure operate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubits vector

	*
		- int

		- Shots:the repeat num of measure operate



.. rubric:: Returns:

std::map<std::string,size_t> result

.. index:: pair: function; accumulateProbability
.. _doxid-group___core_1gab7fa40c4a3d8d4b6c9dc5a5bf389162f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` QPanda::accumulateProbability(:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& prob_list)

AccumulateProbability.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- prob_vec

		- & prob_list Abstract Quantum program pointer



.. rubric:: Returns:

prob_vec

.. index:: pair: function; quick_measure
.. _doxid-group___core_1gabbf7eea831182a82092f70285c027d42:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, size_t> QPanda::quick_measure(
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector,
		int shots,
		:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& accumulate_probabilites
		)

Quick measure.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubits vector

	*
		- int

		- Shots:the repeat num of measure operate

	*
		- prob_vec&

		- accumulate Probabilites



.. rubric:: Returns:

std::map<std::string,size_t> Results

.. index:: pair: function; getQState
.. _doxid-group___core_1gacaafce8fec4c04e15a492fb695176bb1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` QPanda::getQState()

Get quantum state.



.. rubric:: Returns:

qstat Quantum state vector

.. index:: pair: function; initQuantumMachine
.. _doxid-group___core_1gab28a403fe4f2894e330ccd90e01295e4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* QPanda::initQuantumMachine(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type = :ref:`CPU<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13aea39cfc1ace612a8e2c4da2c62ae5659>`)

Init a Quantum machine.

default Quantum machine type :cpu



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QMachineType

		- 



.. rubric:: Returns:

:ref:`QPanda::QuantumMachine <doxid-class_q_panda_1_1_quantum_machine>` \* Quantum machine pointer



.. rubric:: See also:

:ref:`QMachineType <doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>`

.. index:: pair: function; destroyQuantumMachine
.. _doxid-group___core_1ga40086744d5e1d0ee04381ebd63ae40c7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::destroyQuantumMachine(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm)

Destroy Quantum machine.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QuantumMachine\*

		- Quantum machine pointer



.. rubric:: Returns:

void

.. index:: pair: function; MeasureAll
.. _doxid-group___core_1ga5d448b1c38b2b3a13022c5c3a3587b40:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QPanda::QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::MeasureAll(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`, std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>)

Measure All :ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubits vector

	*
		- std::vector<ClassicalCondition>&

		- Cbits vector



.. rubric:: Returns:

:ref:`QPanda::QProg <doxid-class_q_panda_1_1_q_prog>` Quantum program

.. index:: pair: function; getAllocateCMemNum
.. _doxid-group___core_1gaa455e0e99622f5f997c6931981bb33ea:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t QPanda::getAllocateCMemNum()

Get allocate cbit number.



.. rubric:: Returns:

size_t Cbit number

.. index:: pair: function; pMeasure
.. _doxid-group___core_1ga3c19a648c8c21b9b8819b1c8180f20c0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` QPanda::pMeasure(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector, int select_max)

pMeasure



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubit vector

	*
		- int

		- Selectmax:the returned value num



.. rubric:: Returns:

std::vector<std::pair<size_t, double>> result

.. index:: pair: function; pMeasureNoIndex
.. _doxid-group___core_1ga44c86a2a14f084483580f898a70e6a20:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` QPanda::pMeasureNoIndex(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vector)

pMeasure only return result with no index



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubit vector



.. rubric:: Returns:

prob_vec result

.. index:: pair: function; Measure
.. _doxid-group___core_1ga15b15ba85d24d7355880ad63fd4c2107:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>` QPanda::Measure(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`)

QPanda2 basic interface for creating a quantum measure node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- qubit address

	*
		- :ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

		- cbit



.. rubric:: Returns:

:ref:`QPanda::QMeasure <doxid-class_q_panda_1_1_q_measure>` quantum measure node

