.. index:: pair: class; QPanda::OriginNelderMead
.. _doxid-class_q_panda_1_1_origin_nelder_mead:

class QPanda::OriginNelderMead
==============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Minimization of scalar function of one or more variables using the Nelder-Mead algorithm. :ref:`More...<details-class_q_panda_1_1_origin_nelder_mead>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginNelderMead.h>
	
	class OriginNelderMead: public :ref:`QPanda::AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`
	{
	public:
		// construction
	
		:ref:`OriginNelderMead<doxid-class_q_panda_1_1_origin_nelder_mead_1a2c02be4d418b93c7385882667f08bf68>`();
		:target:`OriginNelderMead<doxid-class_q_panda_1_1_origin_nelder_mead_1a145985804d3a333a3fb552d1bc3a4ef7>`(const OriginNelderMead&);

		// methods
	
		OriginNelderMead& :target:`operator =<doxid-class_q_panda_1_1_origin_nelder_mead_1ad50d1bb1542db17e20015acf16a1a286>` (const OriginNelderMead&);
		virtual void :ref:`exec<doxid-class_q_panda_1_1_origin_nelder_mead_1ac8229e7676b0f807cdaaec05489ac4f2>`();
		virtual QOptimizationResult :ref:`getResult<doxid-class_q_panda_1_1_origin_nelder_mead_1a578610e64d3ffc7212942cc3f143f9d3>`();
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

.. _details-class_q_panda_1_1_origin_nelder_mead:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Minimization of scalar function of one or more variables using the Nelder-Mead algorithm.

Construction
------------

.. index:: pair: function; OriginNelderMead
.. _doxid-class_q_panda_1_1_origin_nelder_mead_1a2c02be4d418b93c7385882667f08bf68:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginNelderMead()

Constructor of :ref:`OriginNelderMead <doxid-class_q_panda_1_1_origin_nelder_mead>`.

Methods
-------

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_origin_nelder_mead_1ac8229e7676b0f807cdaaec05489ac4f2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void exec()

execute optimization

.. index:: pair: function; getResult
.. _doxid-class_q_panda_1_1_origin_nelder_mead_1a578610e64d3ffc7212942cc3f143f9d3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual QOptimizationResult getResult()

get optimization result



.. rubric:: Returns:

QOptimizationResult optimization result

