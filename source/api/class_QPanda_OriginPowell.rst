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
		virtual QOptimizationResult :ref:`getResult<doxid-class_q_panda_1_1_origin_powell_1adff011899d8983e833ba4ee5e2d246eb>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`& :ref:`operator =<doxid-class_q_panda_1_1_abstract_optimizer_1a44ebaa3a5368a589cd730a41a018e235>` (const :ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`&);
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

	virtual QOptimizationResult getResult()

get optimization result



.. rubric:: Returns:

QOptimizationResult optimization result

