.. index:: pair: struct; QPanda::QOptimizationResult
.. _doxid-struct_q_panda_1_1_q_optimization_result:

struct QPanda::QOptimizationResult
==================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

optimization result structure :ref:`More...<details-struct_q_panda_1_1_q_optimization_result>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <DataStruct.h>
	
	struct QOptimizationResult
	{
		// fields
	
		std::string :target:`message<doxid-struct_q_panda_1_1_q_optimization_result_1a3a590b2aea0f322716fd708934e238a4>`;
		size_t :ref:`iters<doxid-struct_q_panda_1_1_q_optimization_result_1ab61e06837bf8dfa672e705fd6e002b0e>`;
		size_t :ref:`fcalls<doxid-struct_q_panda_1_1_q_optimization_result_1a49d680440b6391f472311da958f6a164>`;
		std::string :ref:`key<doxid-struct_q_panda_1_1_q_optimization_result_1ab48bbff8397d5efc1f151d864940c79d>`;
		double :ref:`fun_val<doxid-struct_q_panda_1_1_q_optimization_result_1a032435437ecec51a12e3203039ca2e2b>`;
		:ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>` :ref:`para<doxid-struct_q_panda_1_1_q_optimization_result_1a44a1477004a0051cc6f16b4d5dcb866d>`;
	};
.. _details-struct_q_panda_1_1_q_optimization_result:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

optimization result structure

Fields
------

.. index:: pair: variable; iters
.. _doxid-struct_q_panda_1_1_q_optimization_result_1ab61e06837bf8dfa672e705fd6e002b0e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t iters

iteration count.

.. index:: pair: variable; fcalls
.. _doxid-struct_q_panda_1_1_q_optimization_result_1a49d680440b6391f472311da958f6a164:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t fcalls

function call count.

.. index:: pair: variable; key
.. _doxid-struct_q_panda_1_1_q_optimization_result_1ab48bbff8397d5efc1f151d864940c79d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string key

problem solution.

.. index:: pair: variable; fun_val
.. _doxid-struct_q_panda_1_1_q_optimization_result_1a032435437ecec51a12e3203039ca2e2b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	double fun_val

minimun value of the problem.

.. index:: pair: variable; para
.. _doxid-struct_q_panda_1_1_q_optimization_result_1a44a1477004a0051cc6f16b4d5dcb866d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>` para

optimized para

