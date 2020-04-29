.. index:: pair: group; DJ_Algorithm
.. _doxid-group___d_j___algorithm:

DJ_Algorithm
============

.. toctree::
	:hidden:

Overview
~~~~~~~~

Deutsch Jozsa algorithm. :ref:`More...<details-group___d_j___algorithm>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::deutschJozsaAlgorithm<doxid-group___d_j___algorithm_1ga5ee04d03753fbd09dffd803716552f58>`(std::vector<bool> boolean_function, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`DJ_Oracle<doxid-namespace_q_panda_1a128c4092d904b9f5b0ee5b6fc6e25a95>` oracle);

.. _details-group___d_j___algorithm:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Deutsch Jozsa algorithm.

Global Functions
----------------

.. index:: pair: function; deutschJozsaAlgorithm
.. _doxid-group___d_j___algorithm_1ga5ee04d03753fbd09dffd803716552f58:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::deutschJozsaAlgorithm(
		std::vector<bool> boolean_function,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm,
		:ref:`DJ_Oracle<doxid-namespace_q_panda_1a128c4092d904b9f5b0ee5b6fc6e25a95>` oracle
		)

Deutsch Jozsa algorithm.

In the Deutsch-Jozsa problem, we are given a black box quantum computer known as an oracle that implements some function f:{0,1}^{n}->{0,1}. The function takes n-digit binary values as input and produces either a 0 or a 1 as output for each such value. We are promised that the function is either constant (0 on all outputs or 1 on all outputs) or balanced (returns 1 for half of the input domain and 0 for the other half); the task then is to determine if f is constant or balanced by using the oracle.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<bool>

		- boolean_function{f(0)= (0/1)?, f(1)=(0/1)?}

	*
		- QuantumMachine\*

		- Quantum machine ptr

	*
		- DJ_Oracle

		- Deutsch Jozsa algorithm oracle



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

