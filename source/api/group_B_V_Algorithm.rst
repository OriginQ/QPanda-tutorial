.. index:: pair: group; B_V_Algorithm
.. _doxid-group___b___v___algorithm:

B_V_Algorithm
=============

.. toctree::
	:hidden:

Overview
~~~~~~~~

Bernstein-Vazirani algorithm. :ref:`More...<details-group___b___v___algorithm>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::bernsteinVaziraniAlgorithm<doxid-group___b___v___algorithm_1ga9fddd471931a1b3590405d5caf32151f>`(std::string stra, bool b, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`BV_Oracle<doxid-namespace_q_panda_1ae77eda567be203be8fc4bbe4102358f0>` oracle);

.. _details-group___b___v___algorithm:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Bernstein-Vazirani algorithm.

Global Functions
----------------

.. index:: pair: function; bernsteinVaziraniAlgorithm
.. _doxid-group___b___v___algorithm_1ga9fddd471931a1b3590405d5caf32151f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::bernsteinVaziraniAlgorithm(std::string stra, bool b, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`BV_Oracle<doxid-namespace_q_panda_1ae77eda567be203be8fc4bbe4102358f0>` oracle)

Bernstein Vazirani algorithm.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- Hidden string, is equal of "a" in "f(x)=a\*x+b"

	*
		- bool

		- is equal of "b" in "f(x)=a\*x+b"

	*
		- QuantumMachine\*

		- Quantum machine ptr

	*
		- BV_Oracle

		- Deutsch Jozsa algorithm oracle



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

