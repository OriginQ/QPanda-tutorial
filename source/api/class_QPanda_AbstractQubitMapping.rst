.. index:: pair: class; QPanda::AbstractQubitMapping
.. _doxid-class_q_panda_1_1_abstract_qubit_mapping:

class QPanda::AbstractQubitMapping
==================================

.. toctree::
	:hidden:

Base abstract class that allocates the qbits used in the program to the qbits that are in the physical architecture.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitMapping.h>
	
	class AbstractQubitMapping
	{
	public:
		// typedefs
	
		typedef AbstractQubitMapping* :target:`Ref<doxid-class_q_panda_1_1_abstract_qubit_mapping_1a4e1a3cc6a1d1c7ace5fa2e3a2d46dd09>`;
		typedef std::unique_ptr<AbstractQubitMapping> :target:`uRef<doxid-class_q_panda_1_1_abstract_qubit_mapping_1aec10d5d3e1e72d771e3e1839b23ddb56>`;

		// methods
	
		bool :target:`run<doxid-class_q_panda_1_1_abstract_qubit_mapping_1a395d5db7f7eb197e73500dd070a0d073>`(
			:ref:`QPanda::QProg<doxid-class_q_panda_1_1_q_prog>` prog,
			:ref:`QPanda::QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);
	
		void :target:`setGateWeightMap<doxid-class_q_panda_1_1_abstract_qubit_mapping_1ad6346d2f3960468cd2a1ad825918ce89>`(const :ref:`GateWeightMap<doxid-namespace_q_panda_1a812633bf3046648fea1dc3d7814a54d6>`& weightMap);
		const :ref:`Mapping<doxid-namespace_q_panda_1a7b5fe6d8f00345359e7ae23d05af5e24>`& :target:`get_final_mapping<doxid-class_q_panda_1_1_abstract_qubit_mapping_1a4e7d42081a6dbfb38106cc69349bdba1>`() const;
		const :ref:`Mapping<doxid-namespace_q_panda_1a7b5fe6d8f00345359e7ae23d05af5e24>`& :target:`get_init_mapping<doxid-class_q_panda_1_1_abstract_qubit_mapping_1acbfbb14deed6a04ee3255ca3f9e5d363>`() const;
		:ref:`QPanda::QProg<doxid-class_q_panda_1_1_q_prog>` :target:`get_mapped_prog<doxid-class_q_panda_1_1_abstract_qubit_mapping_1abb4be5792d7f7d28312b5e46855cddee>`() const;
	};

	// direct descendants

	class :ref:`OptBMTQAllocator<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator>`;
	class :ref:`SabreQAllocator<doxid-class_q_panda_1_1_sabre_q_allocator>`;
