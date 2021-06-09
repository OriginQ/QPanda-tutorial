.. index:: pair: class; QPanda::OriginLBFGSB
.. _doxid-class_q_panda_1_1_origin_l_b_f_g_s_b:

class QPanda::OriginLBFGSB
==========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Minimization of scalar function of one or more variables using the COBYLA algorithm. :ref:`More...<details-class_q_panda_1_1_origin_l_b_f_g_s_b>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginLBFGSB.h>
	
	class OriginLBFGSB: public :ref:`QPanda::AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`
	{
	public:
		// construction
	
		:ref:`OriginLBFGSB<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1aa5bd1b511dd79e416f23f7e480ab3041>`();
		:target:`OriginLBFGSB<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1a1b71ea321e2ffcd032da8bb8e1db1b2e>`(const OriginLBFGSB&);

		// methods
	
		OriginLBFGSB& :target:`operator =<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1a7f48d42a65a630919b718387481920f5>` (const OriginLBFGSB&);
		virtual void :ref:`exec<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1a0a58b59aad6255df5476bb4b10cbc8fa>`();
	
		void :target:`set_lower_and_upper_bounds<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1a0831b135e3aad8b55c2c22d3c112808c>`(
			vector_d& lower_bound,
			vector_d& upper
			);
	
		void :target:`add_equality_constraint<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1a03d9075b9c372a925ef9735c29fd0678>`(QOptFunc func);
		void :target:`add_inequality_constraint<doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1a0c82a335367ad7608e5ea1c70302e253>`(QOptFunc func);
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

.. _details-class_q_panda_1_1_origin_l_b_f_g_s_b:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Minimization of scalar function of one or more variables using the COBYLA algorithm.

Construction
------------

.. index:: pair: function; OriginLBFGSB
.. _doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1aa5bd1b511dd79e416f23f7e480ab3041:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginLBFGSB()

Constructor of :ref:`OriginLBFGSB <doxid-class_q_panda_1_1_origin_l_b_f_g_s_b>`.

Methods
-------

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_origin_l_b_f_g_s_b_1a0a58b59aad6255df5476bb4b10cbc8fa:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void exec()

execute optimization

