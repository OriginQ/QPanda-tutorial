.. index:: pair: class; QPanda::QITE
.. _doxid-class_q_panda_1_1_q_i_t_e:

class QPanda::QITE
==================

.. toctree::
	:hidden:

	enum_QPanda_QITE_UpdateMode.rst

Overview
~~~~~~~~

:ref:`Variational <doxid-namespace_q_panda_1_1_variational>` Quantum Imagine Time Evolution Algorithem Class. :ref:`More...<details-class_q_panda_1_1_q_i_t_e>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QITE.h>
	
	class QITE
	{
	public:
		// enums
	
		enum :ref:`UpdateMode<doxid-class_q_panda_1_1_q_i_t_e_1a19cb8b9b7c459e61edafc61188645a07>`;

		// methods
	
		void :ref:`setHamiltonian<doxid-class_q_panda_1_1_q_i_t_e_1a5967d9eadddbc3f389d9bd40bc22414a>`(const :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`& h);
		void :ref:`setAnsatzGate<doxid-class_q_panda_1_1_q_i_t_e_1ae07c92b60de3ae0370d06b3cde41fe3c>`(const std::vector<AnsatzGate>& ansatz_gate);
		void :ref:`setDeltaTau<doxid-class_q_panda_1_1_q_i_t_e_1a0c2c34cca9e10bd5d529da18271eb4d0>`(double delta_tau);
		void :ref:`setIterNum<doxid-class_q_panda_1_1_q_i_t_e_1aeb3b8b32c79df6bdd34e2d5a1788375d>`(size_t num);
		void :ref:`setParaUpdateMode<doxid-class_q_panda_1_1_q_i_t_e_1a2e39c206d73f79a3bef8033ea45a215e>`(:ref:`UpdateMode<doxid-class_q_panda_1_1_q_i_t_e_1a19cb8b9b7c459e61edafc61188645a07>` mode);
		void :ref:`setUpthrowNum<doxid-class_q_panda_1_1_q_i_t_e_1ae0cd1a011dca3c593af663c591260fce>`(size_t num);
		void :ref:`setConvergenceFactorQ<doxid-class_q_panda_1_1_q_i_t_e_1ab5edffb56533e232b64c4c5205709b42>`(double value);
		void :ref:`setQuantumMachineType<doxid-class_q_panda_1_1_q_i_t_e_1a8f0d197fa9b63185fa47dcb335eb593d>`(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type);
		void :ref:`setLogFile<doxid-class_q_panda_1_1_q_i_t_e_1a004aa244453ecd20497f3becfcb8c68c>`(const std::string& filename);
		void :ref:`setArbitaryCofficient<doxid-class_q_panda_1_1_q_i_t_e_1af5f53190a82f774ea7a0048478543566>`(double arbitary_cofficient);
		int :ref:`exec<doxid-class_q_panda_1_1_q_i_t_e_1a27bd9b60cb032844d9be42b61b266d12>`();
		:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :ref:`getResult<doxid-class_q_panda_1_1_q_i_t_e_1a6aeeb4d1143a6a854a1f0c6220f529c2>`();
	};
.. _details-class_q_panda_1_1_q_i_t_e:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Variational <doxid-namespace_q_panda_1_1_variational>` Quantum Imagine Time Evolution Algorithem Class.

Methods
-------

.. index:: pair: function; setHamiltonian
.. _doxid-class_q_panda_1_1_q_i_t_e_1a5967d9eadddbc3f389d9bd40bc22414a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setHamiltonian(const :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`& h)

Set problem hamitonian.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- PauliOperator& problem hamiltoinan



.. rubric:: See also:

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; setAnsatzGate
.. _doxid-class_q_panda_1_1_q_i_t_e_1ae07c92b60de3ae0370d06b3cde41fe3c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setAnsatzGate(const std::vector<AnsatzGate>& ansatz_gate)

Set ansatz gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- std::vector<AnsatzGate>& ansatz gate vector



.. rubric:: See also:

AnsatzGate

.. index:: pair: function; setDeltaTau
.. _doxid-class_q_panda_1_1_q_i_t_e_1a0c2c34cca9e10bd5d529da18271eb4d0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDeltaTau(double delta_tau)

Set delta tau value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- delta tau value

.. index:: pair: function; setIterNum
.. _doxid-class_q_panda_1_1_q_i_t_e_1aeb3b8b32c79df6bdd34e2d5a1788375d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setIterNum(size_t num)

Set iteration number.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- iteration number

.. index:: pair: function; setParaUpdateMode
.. _doxid-class_q_panda_1_1_q_i_t_e_1a2e39c206d73f79a3bef8033ea45a215e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setParaUpdateMode(:ref:`UpdateMode<doxid-class_q_panda_1_1_q_i_t_e_1a19cb8b9b7c459e61edafc61188645a07>` mode)

Set parameters update mode.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- UpdateMode

		- parameters update mode



.. rubric:: See also:

:ref:`UpdateMode <doxid-class_q_panda_1_1_q_i_t_e_1a19cb8b9b7c459e61edafc61188645a07>`

.. index:: pair: function; setUpthrowNum
.. _doxid-class_q_panda_1_1_q_i_t_e_1ae0cd1a011dca3c593af663c591260fce:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setUpthrowNum(size_t num)

Set upthrow number.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- upthrow number

.. index:: pair: function; setConvergenceFactorQ
.. _doxid-class_q_panda_1_1_q_i_t_e_1ab5edffb56533e232b64c4c5205709b42:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setConvergenceFactorQ(double value)

Set convergence factor Q.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- convergence factor Q

.. index:: pair: function; setQuantumMachineType
.. _doxid-class_q_panda_1_1_q_i_t_e_1a8f0d197fa9b63185fa47dcb335eb593d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setQuantumMachineType(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type)

Set the quantum machine type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QMachineType

		- quantum machine type



.. rubric:: See also:

:ref:`QMachineType <doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>`

.. index:: pair: function; setLogFile
.. _doxid-class_q_panda_1_1_q_i_t_e_1a004aa244453ecd20497f3becfcb8c68c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLogFile(const std::string& filename)

Set log file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- std::string& log file name

.. index:: pair: function; setArbitaryCofficient
.. _doxid-class_q_panda_1_1_q_i_t_e_1af5f53190a82f774ea7a0048478543566:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setArbitaryCofficient(double arbitary_cofficient)

Set arbitary cofficient.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- arbitary cofficient

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_q_i_t_e_1a27bd9b60cb032844d9be42b61b266d12:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int exec()

Execute algorithem.



.. rubric:: Returns:

int success flag, 0: success, -1: fail

.. index:: pair: function; getResult
.. _doxid-class_q_panda_1_1_q_i_t_e_1a6aeeb4d1143a6a854a1f0c6220f529c2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` getResult()

Get calculation result of the algorithem.



.. rubric:: Returns:

prob_tuple calculation result

