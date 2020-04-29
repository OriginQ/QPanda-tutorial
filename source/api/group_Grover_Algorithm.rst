.. index:: pair: group; Grover_Algorithm
.. _doxid-group___grover___algorithm:

Grover_Algorithm
================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Grover Algorithm. :ref:`More...<details-group___grover___algorithm>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`QPanda::groverAlgorithm<doxid-group___grover___algorithm_1gaca53d0d6f02da195f90cf87f4f7c1a05>`(size_t target, size_t search_range, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`grover_oracle<doxid-namespace_q_panda_1a11c0bf85de02b818d471d9dc2997ad30>` oracle);

.. _details-group___grover___algorithm:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Grover Algorithm.

Global Functions
----------------

.. index:: pair: function; groverAlgorithm
.. _doxid-group___grover___algorithm_1gaca53d0d6f02da195f90cf87f4f7c1a05:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` QPanda::groverAlgorithm(size_t target, size_t search_range, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm, :ref:`grover_oracle<doxid-namespace_q_panda_1a11c0bf85de02b818d471d9dc2997ad30>` oracle)

Grover Algorithm.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- target number

	*
		- size_t

		- search range

	*
		- QuantumMachine\*

		- Quantum machine ptr

	*
		- grover_oracle

		- Grover Algorithm oracle



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

