.. index:: pair: class; QPanda::ShorAlg
.. _doxid-class_q_panda_1_1_shor_alg:

class QPanda::ShorAlg
=====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Shor Algorthm. :ref:`More...<details-class_q_panda_1_1_shor_alg>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Shor.h>
	
	class ShorAlg
	{
	public:
		// construction
	
		:ref:`ShorAlg<doxid-class_q_panda_1_1_shor_alg_1a3e45b7ce101a0ba9d0986fd45e134086>`(int target);

		// methods
	
		void :ref:`set_decomposition_starter<doxid-class_q_panda_1_1_shor_alg_1a41601192a3c1aa9d0b69d2d3dce8ef47>`(int smallest_base);
		bool :ref:`exec<doxid-class_q_panda_1_1_shor_alg_1a25353ef36abf4bde6279dfd9a025616c>`();
		std::pair<int, int> :ref:`get_results<doxid-class_q_panda_1_1_shor_alg_1a430a43bd66f9dac565beac8835ffb4a8>`();
	};
.. _details-class_q_panda_1_1_shor_alg:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Shor Algorthm.

Construction
------------

.. index:: pair: function; ShorAlg
.. _doxid-class_q_panda_1_1_shor_alg_1a3e45b7ce101a0ba9d0986fd45e134086:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ShorAlg(int target)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- target

		- the number to initialize the large number

Methods
-------

.. index:: pair: function; set_decomposition_starter
.. _doxid-class_q_panda_1_1_shor_alg_1a41601192a3c1aa9d0b69d2d3dce8ef47:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void set_decomposition_starter(int smallest_base)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- set

		- the smallest base, default = 2

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_shor_alg_1a25353ef36abf4bde6279dfd9a025616c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool exec()

execute the prime factorization for target number



.. rubric:: Returns:

whether the process succeed

.. index:: pair: function; get_results
.. _doxid-class_q_panda_1_1_shor_alg_1a430a43bd66f9dac565beac8835ffb4a8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::pair<int, int> get_results()

get the decomposition result



.. rubric:: Returns:

get the decomposition result

