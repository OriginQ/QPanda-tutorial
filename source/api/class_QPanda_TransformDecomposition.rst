.. index:: pair: class; QPanda::TransformDecomposition
.. _doxid-class_q_panda_1_1_transform_decomposition:

class QPanda::TransformDecomposition
====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Transform and decompose qprog. :ref:`More...<details-class_q_panda_1_1_transform_decomposition>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TransformDecomposition.h>
	
	class TransformDecomposition
	{
	public:
		// construction
	
		:target:`TransformDecomposition<doxid-class_q_panda_1_1_transform_decomposition_1a5713c4cb73adb1503ebbd392b2f48892>`(
			std::vector<std::vector<std::string>>& ValidQGateMatrix,
			std::vector<std::vector<std::string>>& QGateMatrix,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine,
			const std::string& config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`
			);

		// methods
	
		void :target:`TraversalOptimizationMerge<doxid-class_q_panda_1_1_transform_decomposition_1a6db62c47a3c03a00a750e4f6fa1b8df8>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
		void :ref:`merge_continue_single_gate_to_u3<doxid-group___utilities_1ga18dd1caea3c42a65cab4cb3a45fad041>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	
		void :target:`decompose_double_qgate<doxid-class_q_panda_1_1_transform_decomposition_1a75934e51b762b6d70ab1dd806f70a573>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			bool b_decompose_multiple_gate = true
			);
	
		void :target:`meta_gate_transform<doxid-class_q_panda_1_1_transform_decomposition_1ab49959d4b5e48e5b66927c26d45c551a>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	};
.. _details-class_q_panda_1_1_transform_decomposition:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Transform and decompose qprog.

Methods
-------

.. index:: pair: function; merge_continue_single_gate_to_u3
.. _doxid-group___utilities_1ga18dd1caea3c42a65cab4cb3a45fad041:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void merge_continue_single_gate_to_u3(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

merge continue single gate to u3 gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the source prog



.. rubric:: Returns:

