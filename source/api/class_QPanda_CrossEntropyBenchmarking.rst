.. index:: pair: class; QPanda::CrossEntropyBenchmarking
.. _doxid-class_q_panda_1_1_cross_entropy_benchmarking:

class QPanda::CrossEntropyBenchmarking
======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

use cross entropy benchmarking (XEB) to calibrate general single- and two-qubit gates :ref:`More...<details-class_q_panda_1_1_cross_entropy_benchmarking>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CrossEntropyBenchmarking.h>
	
	class CrossEntropyBenchmarking
	{
	public:
		// typedefs
	
		typedef std::vector<std::vector<std::vector<double>>> :target:`ProbsDict<doxid-class_q_panda_1_1_cross_entropy_benchmarking_1a91d2884b5d2aa36e87131dfe9ab1885a>`;

		// construction
	
		:target:`CrossEntropyBenchmarking<doxid-class_q_panda_1_1_cross_entropy_benchmarking_1afad02dfae6a29b17bf8d0e55f13d4dd3>`(
			:ref:`MeasureQVMType<doxid-namespace_q_panda_1a8cf0cf019f194f7d9d0172bf3afd108a>` type,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);

		// methods
	
		std::map<int, double> :ref:`calculate_xeb_fidelity<doxid-class_q_panda_1_1_cross_entropy_benchmarking_1a89d403574af963bef2856af5562fb845>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gt,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qbit0,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qbit1,
			const std::vector<int>& cycle_range,
			int num_circuits,
			int shots
			);
	};
.. _details-class_q_panda_1_1_cross_entropy_benchmarking:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

use cross entropy benchmarking (XEB) to calibrate general single- and two-qubit gates

Methods
-------

.. index:: pair: function; calculate_xeb_fidelity
.. _doxid-class_q_panda_1_1_cross_entropy_benchmarking_1a89d403574af963bef2856af5562fb845:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<int, double> calculate_xeb_fidelity(
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gt,
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qbit0,
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qbit1,
		const std::vector<int>& cycle_range,
		int num_circuits,
		int shots
		)

calculate xeb fidelity



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- GateType

		- gate type for calculating fidelity, must be double gate

	*
		- Qubit\*

		- qubit0

	*
		- Qubit\*

		- qubit1 , Must be adjacent to qubit0

	*
		- const

		- std::vector<int>& the size of each layer

	*
		- int

		- number of circuits of each layer

	*
		- int

		- measure shot number



.. rubric:: Returns:

std::map<int, double> xeb result of each layer

