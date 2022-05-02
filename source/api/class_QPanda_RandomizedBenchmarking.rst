.. index:: pair: class; QPanda::RandomizedBenchmarking
.. _doxid-class_q_panda_1_1_randomized_benchmarking:

class QPanda::RandomizedBenchmarking
====================================

.. toctree::
	:hidden:

	struct_QPanda_RandomizedBenchmarking_Cliffords.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <RandomizedBenchmarking.h>
	
	class RandomizedBenchmarking
	{
	public:
		// typedefs
	
		typedef std::vector<std::vector<std::shared_ptr<:ref:`RBGate<doxid-class_q_panda_1_1_r_b_gate>`>>> :target:`CliffordsSeq<doxid-class_q_panda_1_1_randomized_benchmarking_1a12c81616e5322c828ae41eae4dcaf4fe>`;

		// structs
	
		struct :ref:`Cliffords<doxid-struct_q_panda_1_1_randomized_benchmarking_1_1_cliffords>`;

		// construction
	
		:target:`RandomizedBenchmarking<doxid-class_q_panda_1_1_randomized_benchmarking_1ae081b7293ad2f353f271d96adc579846>`(
			:ref:`MeasureQVMType<doxid-namespace_q_panda_1a8cf0cf019f194f7d9d0172bf3afd108a>` type,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);

		// methods
	
		std::map<int, double> :target:`single_qubit_rb<doxid-class_q_panda_1_1_randomized_benchmarking_1a79c28721cb7b9a9beb4fd18a3c20b8f0>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qbit,
			const std::vector<int>& clifford_range,
			int num_circuits,
			int shots,
			const std::vector<:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`>& interleaved_gates = {}
			);
	
		std::map<int, double> :target:`two_qubit_rb<doxid-class_q_panda_1_1_randomized_benchmarking_1a97284bf064ec28a0a73c5ba12025b819>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qbit0,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* qbit1,
			const std::vector<int>& clifford_range,
			int num_circuits,
			int shots,
			const std::vector<:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`>& interleaved_gates = {}
			);
	};
