.. index:: pair: group; HamiltonianSimulation
.. _doxid-group___hamiltonian_simulation:

HamiltonianSimulation
=====================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::simulateZTerm<doxid-group___hamiltonian_simulation_1ga366679393b4da372cae09336afd5bd85>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, double coef, double t);

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::simulateOneTerm<doxid-group___hamiltonian_simulation_1ga671d3f9e4f7405c92a4dd67e2caefa09>`(
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec,
		const :ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`& hamiltonian_term,
		double coef,
		double t
		);

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::simulateHamiltonian<doxid-group___hamiltonian_simulation_1ga45d2c199bcacd1c45488aba60b4f294e>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>`& hamiltonian, double t, size_t slices);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::simulatePauliZHamiltonian<doxid-group___hamiltonian_simulation_1gaee4eac1151b17cb8cbcba893284087bd>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>`& hamiltonian, double t);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::applySingleGateToAll<doxid-group___hamiltonian_simulation_1ga16d8ca96691e3f00aa30436cede022b7>`(const std::string& gate, const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec);
	void :ref:`QPanda::applySingleGateToAll<doxid-group___hamiltonian_simulation_1ga5d07ddf5202fafc04e5682f77bf29b72>`(const std::string& gate, const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::ising_model<doxid-group___hamiltonian_simulation_1ga6d49c4b9b3a175a3f2645ababc7258f9>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`QGraph<doxid-namespace_q_panda_1ae453b3fa92a6aec65ebb5c554d47f1e5>`& graph, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& gamma);
	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`QPanda::pauliX_model<doxid-group___hamiltonian_simulation_1ga92c972b836c6e0d2168656608437988b>`(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& beta);

.. _details-group___hamiltonian_simulation:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. index:: pair: function; simulateZTerm
.. _doxid-group___hamiltonian_simulation_1ga366679393b4da372cae09336afd5bd85:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::simulateZTerm(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, double coef, double t)

Simulating z-only term like H=coef \* (Z0..Zn-1) U=exp(-iHt)

Z-Hamiltonian spreads over the qubit_vec



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<Qubit\*>&

		- the qubit needed to simulate the Hamiltonian

	*
		- double

		- the coefficient of hamiltonian

	*
		- double

		- time



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; simulateOneTerm
.. _doxid-group___hamiltonian_simulation_1ga671d3f9e4f7405c92a4dd67e2caefa09:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::simulateOneTerm(
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec,
		const :ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`& hamiltonian_term,
		double coef,
		double t
		)

Simulate a single term of Hamilonian like "X0 Y1 Z2" with coefficient and time. U=exp(-it\*coef\*H)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<Qubit\*>&

		- the qubit needed to simulate the Hamiltonian

	*
		- QTerm&

		- hamiltonian_term: string like "X0 Y1 Z2"

	*
		- double

		- coef: the coefficient of hamiltonian

	*
		- double

		- t time



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; simulateHamiltonian
.. _doxid-group___hamiltonian_simulation_1ga45d2c199bcacd1c45488aba60b4f294e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::simulateHamiltonian(
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec,
		const :ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>`& hamiltonian,
		double t,
		size_t slices
		)

Simulate a general case of hamiltonian by Trotter-Suzuki approximation. U=exp(-iHt)=(exp(-i H1 t/n)\*exp(-i H2 t/n))^n.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<Qubit\*>&

		- qubit_vec: the qubit needed to simulate the Hamiltonian

	*
		- QHamiltonian&

		- hamiltonian: Hamiltonian

	*
		- double

		- t: time

	*
		- size_t

		- slices: the approximate slices



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; simulatePauliZHamiltonian
.. _doxid-group___hamiltonian_simulation_1gaee4eac1151b17cb8cbcba893284087bd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::simulatePauliZHamiltonian(
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec,
		const :ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>`& hamiltonian,
		double t
		)

Simulate hamiltonian consists of pauli-Z operators.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<Qubit\*>&

		- qubit_vec: the qubit needed to simulate the Hamiltonian

	*
		- QHamiltonian&

		- hamiltonian: Hamiltonian

	*
		- double

		- t: time



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; applySingleGateToAll
.. _doxid-group___hamiltonian_simulation_1ga16d8ca96691e3f00aa30436cede022b7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::applySingleGateToAll(
		const std::string& gate,
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec
		)

Apply single gates to all qubits in qubit_list.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- gate: single gate name.

	*
		- std::vector<Qubit\*>&

		- qubit_vec: qubit vector



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; applySingleGateToAll
.. _doxid-group___hamiltonian_simulation_1ga5d07ddf5202fafc04e5682f77bf29b72:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::applySingleGateToAll(
		const std::string& gate,
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

Apply single gates to all qubits in qubit_list and insert into circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- gate: single gate name.

	*
		- std::vector<Qubit\*>&

		- qubit_vec: qubit vector

	*
		- QCircuit&

		- circuit: operated circuit.



.. rubric:: Returns:

.. index:: pair: function; ising_model
.. _doxid-group___hamiltonian_simulation_1ga6d49c4b9b3a175a3f2645ababc7258f9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::ising_model(
		const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec,
		const :ref:`QGraph<doxid-namespace_q_panda_1ae453b3fa92a6aec65ebb5c554d47f1e5>`& graph,
		const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& gamma
		)

Ising model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<Qubit\*>&

		- qubit_vec: qubit vector

	*
		- QGraph&

		- graph: the problem graph

	*
		- vector_d&

		- gamma: model para



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

.. index:: pair: function; pauliX_model
.. _doxid-group___hamiltonian_simulation_1ga92c972b836c6e0d2168656608437988b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` QPanda::pauliX_model(const std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& qubit_vec, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& beta)

pauli X model



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<Qubit\*>&

		- qubit_vec: qubit vector

	*
		- vector_d&

		- beta: model para



.. rubric:: Returns:

:ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

