.. index:: pair: class; QPanda::AbstractOptimizer
.. _doxid-class_q_panda_1_1_abstract_optimizer:

class QPanda::AbstractOptimizer
===============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Abstract Optimizer. :ref:`More...<details-class_q_panda_1_1_abstract_optimizer>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <AbstractOptimizer.h>
	
	class AbstractOptimizer
	{
	public:
		// construction
	
		:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer_1a93536bd7001913e634407d1b6d4b6856>`();
		:target:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer_1a7930a4854cb06274d03a034461d926e3>`(const AbstractOptimizer&);

		// methods
	
		AbstractOptimizer& :target:`operator =<doxid-class_q_panda_1_1_abstract_optimizer_1a44ebaa3a5368a589cd730a41a018e235>` (const AbstractOptimizer&);
		virtual void :ref:`registerFunc<doxid-class_q_panda_1_1_abstract_optimizer_1acf073a3a9e54bd6d71a042ee328f93ba>`(const QOptFunc& func, const vector_d& optimized_para);
		virtual void :ref:`setDisp<doxid-class_q_panda_1_1_abstract_optimizer_1ae5111a731d2b5f098f29d2c86a8dfb99>`(bool disp);
		virtual void :ref:`setAdaptive<doxid-class_q_panda_1_1_abstract_optimizer_1a7772fc41b0d6387b02be3deb40eb16af>`(bool adaptive);
		virtual void :ref:`setXatol<doxid-class_q_panda_1_1_abstract_optimizer_1a41b5a93c7e500e713fac80cea03fbc1f>`(double xatol);
		virtual void :ref:`setFatol<doxid-class_q_panda_1_1_abstract_optimizer_1a8c3a7273751a42e8cba1a45b124ad9da>`(double fatol);
		virtual void :ref:`setMaxFCalls<doxid-class_q_panda_1_1_abstract_optimizer_1a4c5b0472677a44e784a4b81afc6a6c54>`(size_t max_fcalls);
		virtual void :ref:`setMaxIter<doxid-class_q_panda_1_1_abstract_optimizer_1a026c2021dab5dfa3e37c9a7ee261218d>`(size_t max_iter);
		virtual void :ref:`setRestoreFromCacheFile<doxid-class_q_panda_1_1_abstract_optimizer_1aaf91bc143c9f6cfe9615eff624b531a1>`(bool restore);
		virtual void :ref:`setCacheFile<doxid-class_q_panda_1_1_abstract_optimizer_1a023c32761a08adea239a1b6f200aafe1>`(const std::string& cache_file);
		virtual void :ref:`setTestValueAndParaFile<doxid-class_q_panda_1_1_abstract_optimizer_1a2c6eace2948fcb457669e0869f184511>`(double test_value, const std::string& filename);
		virtual void :ref:`exec<doxid-class_q_panda_1_1_abstract_optimizer_1afdf16d72e9cdc016a19b0220240349f2>`() = 0;
		virtual QOptimizationResult :ref:`getResult<doxid-class_q_panda_1_1_abstract_optimizer_1a35a6001326f90ac86d91589c3dea747f>`();
	};

	// direct descendants

	class :ref:`OriginCOBYLA<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a>`;
	class :ref:`OriginLBFGSB<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b>`;
	class :ref:`OriginNelderMead<doxid-class_q_panda_1_1_origin_nelder_mead>`;
	class :ref:`OriginPowell<doxid-class_q_panda_1_1_origin_powell>`;
	class :ref:`OriginSLSQP<doxid-class_q_panda_1_1_origin_s_l_s_q_p>`;
.. _details-class_q_panda_1_1_abstract_optimizer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Abstract Optimizer.

Construction
------------

.. index:: pair: function; AbstractOptimizer
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a93536bd7001913e634407d1b6d4b6856:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	AbstractOptimizer()

Constructor of :ref:`AbstractOptimizer <doxid-class_q_panda_1_1_abstract_optimizer>` class.

Methods
-------

.. index:: pair: function; registerFunc
.. _doxid-class_q_panda_1_1_abstract_optimizer_1acf073a3a9e54bd6d71a042ee328f93ba:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void registerFunc(const QOptFunc& func, const vector_d& optimized_para)

register a user defined function and set some Optimizer parameters



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QFunc&

		- user defined function

	*
		- vector_d&

		- Optimizer parameters

.. index:: pair: function; setDisp
.. _doxid-class_q_panda_1_1_abstract_optimizer_1ae5111a731d2b5f098f29d2c86a8dfb99:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setDisp(bool disp)

whether or not display the log info



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; setAdaptive
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a7772fc41b0d6387b02be3deb40eb16af:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setAdaptive(bool adaptive)

whether or not use Para of Nelder-Mead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; setXatol
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a41b5a93c7e500e713fac80cea03fbc1f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setXatol(double xatol)

set absolute error in xopt between iterations that is acceptable for convergence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		-

.. index:: pair: function; setFatol
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a8c3a7273751a42e8cba1a45b124ad9da:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setFatol(double fatol)

set Absolute error in func(xopt) between iterations that is acceptable for convergence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		-

.. index:: pair: function; setMaxFCalls
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a4c5b0472677a44e784a4b81afc6a6c54:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setMaxFCalls(size_t max_fcalls)

set the max call times



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		-

.. index:: pair: function; setMaxIter
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a026c2021dab5dfa3e37c9a7ee261218d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setMaxIter(size_t max_iter)

set the max iter times



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		-

.. index:: pair: function; setRestoreFromCacheFile
.. _doxid-class_q_panda_1_1_abstract_optimizer_1aaf91bc143c9f6cfe9615eff624b531a1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setRestoreFromCacheFile(bool restore)

set whether or not restore from cache file



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; setCacheFile
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a023c32761a08adea239a1b6f200aafe1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setCacheFile(const std::string& cache_file)

set cache file



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- cache file name

.. index:: pair: function; setTestValueAndParaFile
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a2c6eace2948fcb457669e0869f184511:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setTestValueAndParaFile(
		double test_value,
		const std::string& filename
		)

only for test



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- test value

	*
		- std::string&

		- file name

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_abstract_optimizer_1afdf16d72e9cdc016a19b0220240349f2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void exec() = 0

execute optimization

.. index:: pair: function; getResult
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a35a6001326f90ac86d91589c3dea747f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual QOptimizationResult getResult()

get optimization result



.. rubric:: Returns:

QOptimizationResult optimization result

