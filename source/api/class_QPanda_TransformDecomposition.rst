.. index:: pair: class; QPanda::TransformDecomposition
.. _doxid-class_q_panda_1_1_transform_decomposition:

class QPanda::TransformDecomposition
====================================

.. toctree::
	:hidden:

Transform and decompose qprog.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TransformDecomposition.h>
	
	class TransformDecomposition
	{
	public:
		// construction
	
		:target:`TransformDecomposition<doxid-class_q_panda_1_1_transform_decomposition_1ae31b38f36cff8c3010ac048658e26d3a>`(
			std::vector<std::vector<std::string>>& ValidQGateMatrix,
			std::vector<std::vector<std::string>>& QGateMatrix,
			std::vector<std::vector<int>>& vAdjacentMatrix,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine
			);

		// methods
	
		void :target:`TraversalOptimizationMerge<doxid-class_q_panda_1_1_transform_decomposition_1a6db62c47a3c03a00a750e4f6fa1b8df8>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	};
