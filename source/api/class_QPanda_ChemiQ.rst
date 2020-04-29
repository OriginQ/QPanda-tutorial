.. index:: pair: class; QPanda::ChemiQ
.. _doxid-class_q_panda_1_1_chemi_q:

class QPanda::ChemiQ
====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

:ref:`ChemiQ <doxid-class_q_panda_1_1_chemi_q>` Algorithm class. :ref:`More...<details-class_q_panda_1_1_chemi_q>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ChemiQ.h>
	
	class ChemiQ
	{
	public:
		// methods
	
		void :ref:`initialize<doxid-class_q_panda_1_1_chemi_q_1a2d2dc70b75af2482fc5154f299da6c22>`(const std::string& dir);
		void :ref:`finalize<doxid-class_q_panda_1_1_chemi_q_1a27e2646211fce4c8c5f1cbef36aca229>`();
		void :ref:`setMolecule<doxid-class_q_panda_1_1_chemi_q_1a11e633fa9a7fcaad161dadd7a091ee08>`(const std::string& molecule);
		void :ref:`setMolecules<doxid-class_q_panda_1_1_chemi_q_1af3b7557f42a6e360848a8e1e8d1f5306>`(const :ref:`vector_s<doxid-namespace_q_panda_1a81f654d5e024b7b9de5b4a14ded7b164>`& molecules);
		void :ref:`setMultiplicity<doxid-class_q_panda_1_1_chemi_q_1a1db396aaf62d2c5031bf7b98429d6db4>`(int multiplicity);
		void :ref:`setCharge<doxid-class_q_panda_1_1_chemi_q_1a6d1f8e61fea5b0e7b30a9ff76c5acc5e>`(int charge);
		void :ref:`setBasis<doxid-class_q_panda_1_1_chemi_q_1a29b0287c1714758b49a68bb1f5a60800>`(const std::string& basis);
		void :ref:`setTransformType<doxid-class_q_panda_1_1_chemi_q_1a1c462e3c09456f7b3a3a86a4e6ac90e7>`(:ref:`TransFormType<doxid-namespace_q_panda_1a5f9863b9f685c15e539744e808edde8b>` type);
		void :ref:`setUccType<doxid-class_q_panda_1_1_chemi_q_1ac63601f2596eecfdfea5417e06d7f7da>`(:ref:`UccType<doxid-namespace_q_panda_1a7f68ed9ecff5c30e9105f9cf9ac259ba>` ucc_type);
		void :ref:`setOptimizerType<doxid-class_q_panda_1_1_chemi_q_1abfe4046f374fd4e12fa68bcc673985d5>`(:ref:`OptimizerType<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>` optimizer_type);
		void :ref:`setOptimizerIterNum<doxid-class_q_panda_1_1_chemi_q_1af78b0025cccea20ed13e058dc7f21d96>`(size_t iter_num);
		void :ref:`setOptimizerFuncCallNum<doxid-class_q_panda_1_1_chemi_q_1a18b677842018ec420c225812cd9e1c4a>`(size_t num);
		void :ref:`setOptimizerXatol<doxid-class_q_panda_1_1_chemi_q_1a1a0e764d73d6a36cc8c47911cd935c53>`(double value);
		void :ref:`setOptimizerFatol<doxid-class_q_panda_1_1_chemi_q_1a76755a1f887854da230c2991832092ab>`(double value);
		void :ref:`setOptimizerDisp<doxid-class_q_panda_1_1_chemi_q_1a1115fc776f274398507703eb4136622e>`(bool enable);
		void :ref:`setLearningRate<doxid-class_q_panda_1_1_chemi_q_1a37a3a0e918f49b6f21397589f57ee837>`(double learning_rate);
		void :ref:`setEvolutionTime<doxid-class_q_panda_1_1_chemi_q_1a846d3d54cc27fe053a1c2f0ab694773e>`(double t);
		void :ref:`setHamiltonianSimulationSlices<doxid-class_q_panda_1_1_chemi_q_1a13f59e19cba9a52efdc8775c3cb1be1d>`(size_t slices);
		void :ref:`setSaveDataDir<doxid-class_q_panda_1_1_chemi_q_1adce16410ebe6fd90f37c91dbcdc77c36>`(const std::string dir);
		void :ref:`setQuantumMachineType<doxid-class_q_panda_1_1_chemi_q_1a626a5cd97a4480d4c10bc3d85744196b>`(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type);
		void :ref:`setRandomPara<doxid-class_q_panda_1_1_chemi_q_1a46632ee24b1a5a78f66f73f8c42eab04>`(bool enable);
		void :ref:`setDefaultOptimizedPara<doxid-class_q_panda_1_1_chemi_q_1ad07f4220ad29a22469bf529155524114>`(const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para);
		void :ref:`setToGetHamiltonianFromFile<doxid-class_q_panda_1_1_chemi_q_1a2f536c623c736765fd4711fe7863b08e>`(bool enable);
		void :ref:`setHamiltonianGenerationOnly<doxid-class_q_panda_1_1_chemi_q_1aa36eef0e1cc8d6a4468ad64e06888696>`(bool enable);
		bool :ref:`exec<doxid-class_q_panda_1_1_chemi_q_1abe3afde6547e50fa5def76bf054ea2a9>`();
		std::string :ref:`getLastError<doxid-class_q_panda_1_1_chemi_q_1aba638f57282939c23115bf48c638c9db>`() const;
		:ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>` :ref:`getEnergies<doxid-class_q_panda_1_1_chemi_q_1a76202acce7ecce62923f7b63906ac729>`() const;
	};
.. _details-class_q_panda_1_1_chemi_q:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`ChemiQ <doxid-class_q_panda_1_1_chemi_q>` Algorithm class.

Methods
-------

.. index:: pair: function; initialize
.. _doxid-class_q_panda_1_1_chemi_q_1a2d2dc70b75af2482fc5154f299da6c22:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void initialize(const std::string& dir)

Initialize the quantum chemistry calculation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- The dir of the psi4 chemistry calculation package

.. index:: pair: function; finalize
.. _doxid-class_q_panda_1_1_chemi_q_1a27e2646211fce4c8c5f1cbef36aca229:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void finalize()

Finalize the quantum chemistry calculation.

.. index:: pair: function; setMolecule
.. _doxid-class_q_panda_1_1_chemi_q_1a11e633fa9a7fcaad161dadd7a091ee08:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMolecule(const std::string& molecule)

Set the molecular model to calculate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- molecule model

.. index:: pair: function; setMolecules
.. _doxid-class_q_panda_1_1_chemi_q_1af3b7557f42a6e360848a8e1e8d1f5306:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMolecules(const :ref:`vector_s<doxid-namespace_q_panda_1a81f654d5e024b7b9de5b4a14ded7b164>`& molecules)

Set the molecular model to calculate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vector_s

		- molecule model



.. rubric:: See also:

:ref:`vector_s <doxid-namespace_q_panda_1a81f654d5e024b7b9de5b4a14ded7b164>`

.. index:: pair: function; setMultiplicity
.. _doxid-class_q_panda_1_1_chemi_q_1a1db396aaf62d2c5031bf7b98429d6db4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMultiplicity(int multiplicity)

Set the multiplicity of the molecular model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- multiplicity

.. index:: pair: function; setCharge
.. _doxid-class_q_panda_1_1_chemi_q_1a6d1f8e61fea5b0e7b30a9ff76c5acc5e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setCharge(int charge)

Set the charge of the molecular model.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- charge

.. index:: pair: function; setBasis
.. _doxid-class_q_panda_1_1_chemi_q_1a29b0287c1714758b49a68bb1f5a60800:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setBasis(const std::string& basis)

Set the calculation basis.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- basis

.. index:: pair: function; setTransformType
.. _doxid-class_q_panda_1_1_chemi_q_1a1c462e3c09456f7b3a3a86a4e6ac90e7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setTransformType(:ref:`TransFormType<doxid-namespace_q_panda_1a5f9863b9f685c15e539744e808edde8b>` type)

Set the transform type from Fermion operator to Pauli operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- TransFormType

		- transform type



.. rubric:: See also:

:ref:`TransFormType <doxid-namespace_q_panda_1a5f9863b9f685c15e539744e808edde8b>`

.. index:: pair: function; setUccType
.. _doxid-class_q_panda_1_1_chemi_q_1ac63601f2596eecfdfea5417e06d7f7da:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setUccType(:ref:`UccType<doxid-namespace_q_panda_1a7f68ed9ecff5c30e9105f9cf9ac259ba>` ucc_type)

Set the ucc type to contruct the Fermion operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- UccType

		- ucc type



.. rubric:: See also:

:ref:`UccType <doxid-namespace_q_panda_1a7f68ed9ecff5c30e9105f9cf9ac259ba>`

.. index:: pair: function; setOptimizerType
.. _doxid-class_q_panda_1_1_chemi_q_1abfe4046f374fd4e12fa68bcc673985d5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setOptimizerType(:ref:`OptimizerType<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>` optimizer_type)

Set the optimizer type.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- OptimizerType

		- optimizer type



.. rubric:: See also:

:ref:`OptimizerType <doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>`

.. index:: pair: function; setOptimizerIterNum
.. _doxid-class_q_panda_1_1_chemi_q_1af78b0025cccea20ed13e058dc7f21d96:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setOptimizerIterNum(size_t iter_num)

Set the optimizer iteration number.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- iteration number

.. index:: pair: function; setOptimizerFuncCallNum
.. _doxid-class_q_panda_1_1_chemi_q_1a18b677842018ec420c225812cd9e1c4a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setOptimizerFuncCallNum(size_t num)

Set the optimizer function callback number.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- function callback number

.. index:: pair: function; setOptimizerXatol
.. _doxid-class_q_panda_1_1_chemi_q_1a1a0e764d73d6a36cc8c47911cd935c53:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setOptimizerXatol(double value)

Set the optimizer xatol.It is the Absolute error in xopt between iterations that is acceptable for convergence.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- absolute error between iterations

.. index:: pair: function; setOptimizerFatol
.. _doxid-class_q_panda_1_1_chemi_q_1a76755a1f887854da230c2991832092ab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setOptimizerFatol(double value)

Set the optimizer fatol.It is the Absolute error in func(xopt) between iterations that is acceptable for convergence.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- absolute error between func(xopt)

.. index:: pair: function; setOptimizerDisp
.. _doxid-class_q_panda_1_1_chemi_q_1a1115fc776f274398507703eb4136622e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setOptimizerDisp(bool enable)

Whether to print the optimized log to the terminal.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- enable

.. index:: pair: function; setLearningRate
.. _doxid-class_q_panda_1_1_chemi_q_1a37a3a0e918f49b6f21397589f57ee837:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLearningRate(double learning_rate)

Set the learing rate when using Gradient optimizer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- learing rate

.. index:: pair: function; setEvolutionTime
.. _doxid-class_q_panda_1_1_chemi_q_1a846d3d54cc27fe053a1c2f0ab694773e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setEvolutionTime(double t)

Set the evolution time when doing hamiltonian simulation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- evolution time

.. index:: pair: function; setHamiltonianSimulationSlices
.. _doxid-class_q_panda_1_1_chemi_q_1a13f59e19cba9a52efdc8775c3cb1be1d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setHamiltonianSimulationSlices(size_t slices)

Set the hamiltonian simulation slices (e^iAt/n\*e^iBt/n)^n, n is the slices.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- hamiltonian simulation slices

.. index:: pair: function; setSaveDataDir
.. _doxid-class_q_panda_1_1_chemi_q_1adce16410ebe6fd90f37c91dbcdc77c36:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setSaveDataDir(const std::string dir)

Set the directory to save the calculated data. If it's a not exist dir data will not be saved.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- dir

.. index:: pair: function; setQuantumMachineType
.. _doxid-class_q_panda_1_1_chemi_q_1a626a5cd97a4480d4c10bc3d85744196b:

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

.. index:: pair: function; setRandomPara
.. _doxid-class_q_panda_1_1_chemi_q_1a46632ee24b1a5a78f66f73f8c42eab04:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setRandomPara(bool enable)

Set random default optimizer paramter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- enable

.. index:: pair: function; setDefaultOptimizedPara
.. _doxid-class_q_panda_1_1_chemi_q_1ad07f4220ad29a22469bf529155524114:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDefaultOptimizedPara(const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para)

Set the default optimizer paramter by the given paramter.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vecotr_d

		- default paramter



.. rubric:: See also:

:ref:`vector_d <doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`

.. index:: pair: function; setToGetHamiltonianFromFile
.. _doxid-class_q_panda_1_1_chemi_q_1a2f536c623c736765fd4711fe7863b08e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setToGetHamiltonianFromFile(bool enable)

Set to get hamiltonian from file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- enable

.. index:: pair: function; setHamiltonianGenerationOnly
.. _doxid-class_q_panda_1_1_chemi_q_1aa36eef0e1cc8d6a4468ad64e06888696:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setHamiltonianGenerationOnly(bool enable)

Set hamiltonian generation only.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- enable

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_chemi_q_1abe3afde6547e50fa5def76bf054ea2a9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool exec()

exec molecule calculate.



.. rubric:: Returns:

bool true:success; false:failed

.. index:: pair: function; getLastError
.. _doxid-class_q_panda_1_1_chemi_q_1aba638f57282939c23115bf48c638c9db:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getLastError() const

get last error.



.. rubric:: Returns:

std::string last error

.. index:: pair: function; getEnergies
.. _doxid-class_q_panda_1_1_chemi_q_1a76202acce7ecce62923f7b63906ac729:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>` getEnergies() const

get calculated energies of the molecules.



.. rubric:: Returns:

vector_d energies

