.. index:: pair: class; QPanda::OriginCOBYLA
.. _doxid-class_q_panda_1_1_origin_c_o_b_y_l_a:

class QPanda::OriginCOBYLA
==========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Minimization of scalar function of one or more variables using the COBYLA algorithm. :ref:`More...<details-class_q_panda_1_1_origin_c_o_b_y_l_a>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginCOBYLA.h>
	
	class OriginCOBYLA: public :ref:`QPanda::AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`
	{
	public:
		// construction
	
		:ref:`OriginCOBYLA<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1a558f3b14f931de122674494e3f4b1644>`();
		:target:`OriginCOBYLA<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1a1c2deadf2d751b7ffadea867c616d337>`(const OriginCOBYLA&);

		// methods
	
		OriginCOBYLA& :target:`operator =<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1ac1cd1865f30b57d6afaa08ed69010771>` (const OriginCOBYLA&);
		virtual void :ref:`exec<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1a7cb88c43e6043e7eb879f7158d031e10>`();
	
		void :target:`set_lower_and_upper_bounds<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1af44403696cae39169457d319edb54593>`(
			vector_d& lower_bound,
			vector_d& upper
			);
	
		void :target:`add_equality_constraint<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1a6161cae516b61f21c78f1547b1759224>`(QOptFunc func);
		void :target:`add_inequality_constraint<doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1a8e2b51d62969c806a55387458fa9feca>`(QOptFunc func);
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

.. _details-class_q_panda_1_1_origin_c_o_b_y_l_a:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Minimization of scalar function of one or more variables using the COBYLA algorithm.

Construction
------------

.. index:: pair: function; OriginCOBYLA
.. _doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1a558f3b14f931de122674494e3f4b1644:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginCOBYLA()

Constructor of :ref:`OriginCOBYLA <doxid-class_q_panda_1_1_origin_c_o_b_y_l_a>`.

Methods
-------

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_origin_c_o_b_y_l_a_1a7cb88c43e6043e7eb879f7158d031e10:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void exec()

execute optimization

