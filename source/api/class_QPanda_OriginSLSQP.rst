.. index:: pair: class; QPanda::OriginSLSQP
.. _doxid-class_q_panda_1_1_origin_s_l_s_q_p:

class QPanda::OriginSLSQP
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Minimization of scalar function of one or more variables using the COBYLA algorithm. :ref:`More...<details-class_q_panda_1_1_origin_s_l_s_q_p>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginSLSQP.h>
	
	class OriginSLSQP: public :ref:`QPanda::AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`
	{
	public:
		// construction
	
		:ref:`OriginSLSQP<doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a6b443504b92d66d9606884aefd1481f1>`();
		:target:`OriginSLSQP<doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a013ecb0588ce2f633bf51221bdc87e80>`(const OriginSLSQP&);

		// methods
	
		OriginSLSQP& :target:`operator =<doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a29613563947fe479104fd001948a7107>` (const OriginSLSQP&);
		virtual void :ref:`exec<doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a045363828d278f45973680908261a455>`();
	
		void :target:`set_lower_and_upper_bounds<doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a72950507440fedb0770d02685ba50a78>`(
			vector_d& lower_bound,
			vector_d& upper
			);
	
		void :target:`add_equality_constraint<doxid-class_q_panda_1_1_origin_s_l_s_q_p_1ae7516e62179f98dbb050d144449ad77a>`(QOptFunc func);
		void :target:`add_inequality_constraint<doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a89781738409f6d84c9a2a2867cb9a113>`(QOptFunc func);
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

.. _details-class_q_panda_1_1_origin_s_l_s_q_p:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Minimization of scalar function of one or more variables using the COBYLA algorithm.

Construction
------------

.. index:: pair: function; OriginSLSQP
.. _doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a6b443504b92d66d9606884aefd1481f1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginSLSQP()

Constructor of :ref:`OriginSLSQP <doxid-class_q_panda_1_1_origin_s_l_s_q_p>`.

Methods
-------

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_origin_s_l_s_q_p_1a045363828d278f45973680908261a455:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void exec()

execute optimization

