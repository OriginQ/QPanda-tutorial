.. index:: pair: class; QPanda::QuantumVolume
.. _doxid-class_q_panda_1_1_quantum_volume:

class QPanda::QuantumVolume
===========================

.. toctree::
	:hidden:

	struct_QPanda_QuantumVolume_QvCircuit.rst

Calculate the quantum volume of the chip.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumVolume.h>
	
	class QuantumVolume
	{
	public:
		// structs
	
		struct :ref:`QvCircuit<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit>`;

		// construction
	
		:target:`QuantumVolume<doxid-class_q_panda_1_1_quantum_volume_1aa47e77f1ad0162cd527792cf569677f3>`(
			:ref:`MeasureQVMType<doxid-namespace_q_panda_1a8cf0cf019f194f7d9d0172bf3afd108a>` type,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);

		// methods
	
		size_t :target:`calcQuantumVolume<doxid-class_q_panda_1_1_quantum_volume_1ae3946ea164795fece320dcc6d8e265db>`(
			const std::vector<std::vector<int>>& qubit_lists,
			int ntrials,
			int shots
			);
	};
