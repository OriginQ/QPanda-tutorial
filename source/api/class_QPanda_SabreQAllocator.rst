.. index:: pair: class; QPanda::SabreQAllocator
.. _doxid-class_q_panda_1_1_sabre_q_allocator:

class QPanda::SabreQAllocator
=============================

.. toctree::
	:hidden:

SABRE qubit mapping Implemented from Gushu et. al.: Tackling the :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` Mapping Problem for NISQ-Era Quantum Devices.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <SabreQMapping.h>
	
	class SabreQAllocator: public :ref:`QPanda::AbstractQubitMapping<doxid-class_q_panda_1_1_abstract_qubit_mapping>`
	{
	public:
		// typedefs
	
		typedef SabreQAllocator* :target:`Ref<doxid-class_q_panda_1_1_sabre_q_allocator_1a9cd1ae73c6256c0d6bfc1a65da4e5996>`;
		typedef std::unique_ptr<SabreQAllocator> :target:`uRef<doxid-class_q_panda_1_1_sabre_q_allocator_1a2c52244c7753395c9e72a42c0f078605>`;

		// methods
	
		static :ref:`uRef<doxid-class_q_panda_1_1_abstract_qubit_mapping_1aec10d5d3e1e72d771e3e1839b23ddb56>` :target:`Create<doxid-class_q_panda_1_1_sabre_q_allocator_1a99c123d0bc37e306fa48f7df60909fad>`(
			:ref:`QPanda::ArchGraph::sRef<doxid-class_q_panda_1_1_arch_graph_1a9c281b804cf8363fc16ce47e61b53de9>` ag,
			uint32_t max_look_ahead = 20,
			uint32_t max_iterations = 10
			);
	
		uint32_t :target:`get_swap_cnt<doxid-class_q_panda_1_1_sabre_q_allocator_1a8517cdeedb429f47bfbec89da99f9d3c>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`AbstractQubitMapping<doxid-class_q_panda_1_1_abstract_qubit_mapping>`* :ref:`Ref<doxid-class_q_panda_1_1_abstract_qubit_mapping_1a4e1a3cc6a1d1c7ace5fa2e3a2d46dd09>`;
		typedef std::unique_ptr<:ref:`AbstractQubitMapping<doxid-class_q_panda_1_1_abstract_qubit_mapping>`> :ref:`uRef<doxid-class_q_panda_1_1_abstract_qubit_mapping_1aec10d5d3e1e72d771e3e1839b23ddb56>`;

		// methods
	
		bool :ref:`run<doxid-class_q_panda_1_1_abstract_qubit_mapping_1a395d5db7f7eb197e73500dd070a0d073>`(:ref:`QPanda::QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QPanda::QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm);
		void :ref:`setGateWeightMap<doxid-class_q_panda_1_1_abstract_qubit_mapping_1ad6346d2f3960468cd2a1ad825918ce89>`(const :ref:`GateWeightMap<doxid-namespace_q_panda_1a812633bf3046648fea1dc3d7814a54d6>`& weightMap);
		const :ref:`Mapping<doxid-namespace_q_panda_1a7b5fe6d8f00345359e7ae23d05af5e24>`& :ref:`get_final_mapping<doxid-class_q_panda_1_1_abstract_qubit_mapping_1a4e7d42081a6dbfb38106cc69349bdba1>`() const;
		const :ref:`Mapping<doxid-namespace_q_panda_1a7b5fe6d8f00345359e7ae23d05af5e24>`& :ref:`get_init_mapping<doxid-class_q_panda_1_1_abstract_qubit_mapping_1acbfbb14deed6a04ee3255ca3f9e5d363>`() const;
		:ref:`QPanda::QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`get_mapped_prog<doxid-class_q_panda_1_1_abstract_qubit_mapping_1abb4be5792d7f7d28312b5e46855cddee>`() const;

