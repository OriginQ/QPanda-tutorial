.. index:: pair: class; QPanda::QuantumCounting
.. _doxid-class_q_panda_1_1_quantum_counting:

class QPanda::QuantumCounting
=============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumCounting.h>
	
	class QuantumCounting: public :ref:`QPanda::AbstractQuantumCounting<doxid-class_q_panda_1_1_abstract_quantum_counting>`
	{
	public:
		// construction
	
		:target:`QuantumCounting<doxid-class_q_panda_1_1_quantum_counting_1a3da9273aa4b7a59a24f3c9775d2eb7a5>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` cir_oracle,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` cir_diffusion,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& data_index_qubits,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& ancilla_qubits
			);

		// methods
	
		virtual size_t :target:`qu_counting<doxid-class_q_panda_1_1_quantum_counting_1a582b976c88f8fdf72792abfeec0e4cfe>`();
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`build_qu_counting_prog<doxid-class_q_panda_1_1_quantum_counting_1a0c871659994c647c09ae1d220a08c7fe>`();
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`QFT<doxid-class_q_panda_1_1_quantum_counting_1a79e141ff73be299314b3de854eb42bc9>`(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> qvec);
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`QFTdagger<doxid-class_q_panda_1_1_quantum_counting_1adfa30c4a1f5c134c69a316f62e80c5a3>`(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> qvec);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual size_t :ref:`qu_counting<doxid-class_q_panda_1_1_abstract_quantum_counting_1a7a5627beca3eb4dd2d63633f34c5b139>`() = 0;

