.. index:: pair: class; QPanda::OriginPowell
.. _doxid-class_q_panda_1_1_origin_powell:

class QPanda::OriginPowell
==========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Minimization of scalar function of one or more variables using the Powell algorithm. :ref:`More...<details-class_q_panda_1_1_origin_powell>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginPowell.h>
	
	class OriginPowell: public :ref:`QPanda::AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`
	{
	public:
		// construction
	
		:ref:`OriginPowell<doxid-class_q_panda_1_1_origin_powell_1aceb22f18adb7bec27fee6d4b232b8960>`();
		:target:`OriginPowell<doxid-class_q_panda_1_1_origin_powell_1aa2396293ad7da7b6a78f9597eb993e4b>`(const OriginPowell&);

		// methods
	
		OriginPowell& :target:`operator =<doxid-class_q_panda_1_1_origin_powell_1a9cf21be52753e7410708f81a88194e8e>` (const OriginPowell&);
		virtual void :ref:`exec<doxid-class_q_panda_1_1_origin_powell_1a8480d37fef8b764aa487ece24b92aa2d>`();
		virtual :ref:`QOptimizationResult<doxid-struct_q_panda_1_1_q_optimization_result>` :ref:`getResult<doxid-class_q_panda_1_1_origin_powell_1adff011899d8983e833ba4ee5e2d246eb>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`& :ref:`operator =<doxid-class_q_panda_1_1_abstract_optimizer_1a44ebaa3a5368a589cd730a41a018e235>` (const :ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`&);
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

.. _details-class_q_panda_1_1_origin_powell:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Minimization of scalar function of one or more variables using the Powell algorithm.

Construction
------------

.. index:: pair: function; OriginPowell
.. _doxid-class_q_panda_1_1_origin_powell_1aceb22f18adb7bec27fee6d4b232b8960:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginPowell()

Constructor of :ref:`OriginPowell <doxid-class_q_panda_1_1_origin_powell>`.

Methods
-------

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_origin_powell_1a8480d37fef8b764aa487ece24b92aa2d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void exec()

execute optimization

.. index:: pair: function; getResult
.. _doxid-class_q_panda_1_1_origin_powell_1adff011899d8983e833ba4ee5e2d246eb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QOptimizationResult<doxid-struct_q_panda_1_1_q_optimization_result>` getResult()

get optimization result



.. rubric:: Returns:

:ref:`QOptimizationResult <doxid-struct_q_panda_1_1_q_optimization_result>` optimization result

