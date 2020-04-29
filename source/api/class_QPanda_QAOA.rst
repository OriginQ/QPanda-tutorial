.. index:: pair: class; QPanda::QAOA
.. _doxid-class_q_panda_1_1_q_a_o_a:

class QPanda::QAOA
==================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum Approximate Optimization Algorithm. :ref:`More...<details-class_q_panda_1_1_q_a_o_a>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QAOA.h>
	
	class QAOA
	{
	public:
		// construction
	
		:ref:`QAOA<doxid-class_q_panda_1_1_q_a_o_a_1ad05b9d3cb30f291a29578ed5eaf1bda5>`(:ref:`OptimizerType<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>` optimizer = :ref:`OptimizerType::NELDER_MEAD<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1eaaf17589bbef521816776475a5399abae>`);
		:target:`QAOA<doxid-class_q_panda_1_1_q_a_o_a_1ab55d6227721ecf4e24119954018e87e0>`(const std::string& optimizer);
		:target:`QAOA<doxid-class_q_panda_1_1_q_a_o_a_1ae6a1471b20fea4f65a43f425a114863a>`(QAOA&);

		// methods
	
		QAOA& :target:`operator =<doxid-class_q_panda_1_1_q_a_o_a_1a24e6bda674f15a893fca84cda63460da>` (QAOA&);
		void :ref:`setHamiltonian<doxid-class_q_panda_1_1_q_a_o_a_1aa976d6ffca836d28f8bedf413f2720c1>`(const :ref:`QPauliMap<doxid-namespace_q_panda_1a34d536a170f46858ef57b8b4bc2e85d1>`& pauli_map);
		void :ref:`setDeltaT<doxid-class_q_panda_1_1_q_a_o_a_1a1124a0fc817e55cf852307e9067227e6>`(double delta_t);
		void :ref:`setStep<doxid-class_q_panda_1_1_q_a_o_a_1a48dfd33e533f28a3e3e130c0c6e7f813>`(size_t step);
		size_t :ref:`step<doxid-class_q_panda_1_1_q_a_o_a_1a61d47f5ccb9ba40d78e37b58f9f104af>`();
		void :ref:`setShots<doxid-class_q_panda_1_1_q_a_o_a_1a78343e397190da28372f24222274e094>`(size_t shots);
		void :ref:`regiestUserDefinedFunc<doxid-class_q_panda_1_1_q_a_o_a_1a5b74e0b78bfe1e6bcf605912402398df>`(const :ref:`QUserDefinedFunc<doxid-namespace_q_panda_1a70bd7af3a5b6b5650c425d3aa9f52774>`& func);
		void :ref:`setDefaultOptimizePara<doxid-class_q_panda_1_1_q_a_o_a_1a220cc868ee9cf4d48c1cc2d9a5e36295>`(const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para);
		void :ref:`enableLog<doxid-class_q_panda_1_1_q_a_o_a_1a85654d77c41cbfa3e0e311f536fadac9>`(bool enabled, std::string filename = "");
		:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`* :ref:`getOptimizer<doxid-class_q_panda_1_1_q_a_o_a_1a69bee1b08dfebea0a40c3f5a5ea8d4ef>`();
		bool :ref:`exec<doxid-class_q_panda_1_1_q_a_o_a_1a4dfc951abaf4977d7812cba2ec0270e4>`();
		:ref:`QOptimizationResult<doxid-struct_q_panda_1_1_q_optimization_result>` :ref:`getOptimizerResult<doxid-class_q_panda_1_1_q_a_o_a_1adee39f76d7bd61f3df6b67776598aee0>`();
		bool :ref:`scan2Para<doxid-class_q_panda_1_1_q_a_o_a_1a37105eafb00e0c3e049eca7cb64556e3>`(const :ref:`QScanPara<doxid-struct_q_panda_1_1_q_scan_para>`& data);
	};
.. _details-class_q_panda_1_1_q_a_o_a:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum Approximate Optimization Algorithm.

Construction
------------

.. index:: pair: function; QAOA
.. _doxid-class_q_panda_1_1_q_a_o_a_1ad05b9d3cb30f291a29578ed5eaf1bda5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QAOA(:ref:`OptimizerType<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>` optimizer = :ref:`OptimizerType::NELDER_MEAD<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1eaaf17589bbef521816776475a5399abae>`)

Constructor of :ref:`ChemiQ <doxid-class_q_panda_1_1_chemi_q>`.

Methods
-------

.. index:: pair: function; setHamiltonian
.. _doxid-class_q_panda_1_1_q_a_o_a_1aa976d6ffca836d28f8bedf413f2720c1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setHamiltonian(const :ref:`QPauliMap<doxid-namespace_q_panda_1a34d536a170f46858ef57b8b4bc2e85d1>`& pauli_map)

set Hamiltonian



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QPauliMap&

		- pauli map

.. index:: pair: function; setDeltaT
.. _doxid-class_q_panda_1_1_q_a_o_a_1a1124a0fc817e55cf852307e9067227e6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDeltaT(double delta_t)

set val of Delta T



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- the val of Delta T

.. index:: pair: function; setStep
.. _doxid-class_q_panda_1_1_q_a_o_a_1a48dfd33e533f28a3e3e130c0c6e7f813:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setStep(size_t step)

set step



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- the val of step

.. index:: pair: function; step
.. _doxid-class_q_panda_1_1_q_a_o_a_1a61d47f5ccb9ba40d78e37b58f9f104af:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t step()

get step



.. rubric:: Returns:

return the val of step

.. index:: pair: function; setShots
.. _doxid-class_q_panda_1_1_q_a_o_a_1a78343e397190da28372f24222274e094:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setShots(size_t shots)

set Shots val



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- the val of Shots

.. index:: pair: function; regiestUserDefinedFunc
.. _doxid-class_q_panda_1_1_q_a_o_a_1a5b74e0b78bfe1e6bcf605912402398df:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void regiestUserDefinedFunc(const :ref:`QUserDefinedFunc<doxid-namespace_q_panda_1a70bd7af3a5b6b5650c425d3aa9f52774>`& func)

regiest user defined functional



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QUserDefinedFunc&

		- the user defined functional

.. index:: pair: function; setDefaultOptimizePara
.. _doxid-class_q_panda_1_1_q_a_o_a_1a220cc868ee9cf4d48c1cc2d9a5e36295:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDefaultOptimizePara(const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para)

set default optimize parameter



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vector_d&

		- the default optimize parameters

.. index:: pair: function; enableLog
.. _doxid-class_q_panda_1_1_q_a_o_a_1a85654d77c41cbfa3e0e311f536fadac9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void enableLog(bool enabled, std::string filename = "")

whether or not enable the log file



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- whether or not

	*
		- string

		- filename log file name

.. index:: pair: function; getOptimizer
.. _doxid-class_q_panda_1_1_q_a_o_a_1a69bee1b08dfebea0a40c3f5a5ea8d4ef:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`* getOptimizer()

get optimizer object



.. rubric:: Returns:

AbstractOptimizer\* the optimizer object ptr

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_q_a_o_a_1a4dfc951abaf4977d7812cba2ec0270e4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool exec()

execute optimizer



.. rubric:: Returns:

return true on success, or else return false

.. index:: pair: function; getOptimizerResult
.. _doxid-class_q_panda_1_1_q_a_o_a_1adee39f76d7bd61f3df6b67776598aee0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QOptimizationResult<doxid-struct_q_panda_1_1_q_optimization_result>` getOptimizerResult()

get optimizer result



.. rubric:: Returns:

return :ref:`QOptimizationResult <doxid-struct_q_panda_1_1_q_optimization_result>`

.. index:: pair: function; scan2Para
.. _doxid-class_q_panda_1_1_q_a_o_a_1a37105eafb00e0c3e049eca7cb64556e3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool scan2Para(const :ref:`QScanPara<doxid-struct_q_panda_1_1_q_scan_para>`& data)

scan Para to file



.. rubric:: Returns:

return true on success, or else return false

