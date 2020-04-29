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
		void :ref:`registerFunc<doxid-class_q_panda_1_1_abstract_optimizer_1a1e90b30337c0d5e26bfe33c9596bbe51>`(const :ref:`QFunc<doxid-namespace_q_panda_1a801c623e7ed0e99219b7e63e3f27d4e1>`& func, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& optimized_para);
		void :ref:`setDisp<doxid-class_q_panda_1_1_abstract_optimizer_1af61e5da153321f023ed69e31016174f9>`(bool disp);
		void :ref:`setAdaptive<doxid-class_q_panda_1_1_abstract_optimizer_1a894005fa51a011846484385f6d6d8e97>`(bool adaptive);
		void :ref:`setXatol<doxid-class_q_panda_1_1_abstract_optimizer_1ab82b0d90ef6d9006057f24ced0d795b2>`(double xatol);
		void :ref:`setFatol<doxid-class_q_panda_1_1_abstract_optimizer_1ade33e598b97dd1e3bd694037b9413b55>`(double fatol);
		void :ref:`setMaxFCalls<doxid-class_q_panda_1_1_abstract_optimizer_1a028f06a48020af8394249e6eb8aa639a>`(size_t max_fcalls);
		void :ref:`setMaxIter<doxid-class_q_panda_1_1_abstract_optimizer_1a633e6b3481a698316ffeccbe5c14175f>`(size_t max_iter);
		void :ref:`setRestoreFromCacheFile<doxid-class_q_panda_1_1_abstract_optimizer_1a28961fca175832a48db7baa6792a8c41>`(bool restore);
		void :ref:`setCacheFile<doxid-class_q_panda_1_1_abstract_optimizer_1a93b3081816a73f1bae887709003074f6>`(const std::string& cache_file);
		void :ref:`setTestValueAndParaFile<doxid-class_q_panda_1_1_abstract_optimizer_1a842032fdf0491bb5e95e208826971913>`(double test_value, const std::string& filename);
		virtual void :ref:`exec<doxid-class_q_panda_1_1_abstract_optimizer_1afdf16d72e9cdc016a19b0220240349f2>`() = 0;
		virtual :ref:`QOptimizationResult<doxid-struct_q_panda_1_1_q_optimization_result>` :ref:`getResult<doxid-class_q_panda_1_1_abstract_optimizer_1a35a6001326f90ac86d91589c3dea747f>`();
	};

	// direct descendants

	class :ref:`OriginNelderMead<doxid-class_q_panda_1_1_origin_nelder_mead>`;
	class :ref:`OriginPowell<doxid-class_q_panda_1_1_origin_powell>`;
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
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a1e90b30337c0d5e26bfe33c9596bbe51:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void registerFunc(const :ref:`QFunc<doxid-namespace_q_panda_1a801c623e7ed0e99219b7e63e3f27d4e1>`& func, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& optimized_para)

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
.. _doxid-class_q_panda_1_1_abstract_optimizer_1af61e5da153321f023ed69e31016174f9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setDisp(bool disp)

whether or not display the log info



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; setAdaptive
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a894005fa51a011846484385f6d6d8e97:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setAdaptive(bool adaptive)

whether or not use Para of Nelder-Mead



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; setXatol
.. _doxid-class_q_panda_1_1_abstract_optimizer_1ab82b0d90ef6d9006057f24ced0d795b2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setXatol(double xatol)

set absolute error in xopt between iterations that is acceptable for convergence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		-

.. index:: pair: function; setFatol
.. _doxid-class_q_panda_1_1_abstract_optimizer_1ade33e598b97dd1e3bd694037b9413b55:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setFatol(double fatol)

set Absolute error in func(xopt) between iterations that is acceptable for convergence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		-

.. index:: pair: function; setMaxFCalls
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a028f06a48020af8394249e6eb8aa639a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMaxFCalls(size_t max_fcalls)

set the max call times



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		-

.. index:: pair: function; setMaxIter
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a633e6b3481a698316ffeccbe5c14175f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMaxIter(size_t max_iter)

set the max iter times



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		-

.. index:: pair: function; setRestoreFromCacheFile
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a28961fca175832a48db7baa6792a8c41:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setRestoreFromCacheFile(bool restore)

set whether or not restore from cache file



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; setCacheFile
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a93b3081816a73f1bae887709003074f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setCacheFile(const std::string& cache_file)

set cache file



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- cache file name

.. index:: pair: function; setTestValueAndParaFile
.. _doxid-class_q_panda_1_1_abstract_optimizer_1a842032fdf0491bb5e95e208826971913:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setTestValueAndParaFile(double test_value, const std::string& filename)

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

	virtual :ref:`QOptimizationResult<doxid-struct_q_panda_1_1_q_optimization_result>` getResult()

get optimization result



.. rubric:: Returns:

:ref:`QOptimizationResult <doxid-struct_q_panda_1_1_q_optimization_result>` optimization result

