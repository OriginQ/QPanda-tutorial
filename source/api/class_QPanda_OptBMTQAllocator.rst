.. index:: pair: class; QPanda::OptBMTQAllocator
.. _doxid-class_q_panda_1_1_opt_b_m_t_q_allocator:

class QPanda::OptBMTQAllocator
==============================

.. toctree::
	:hidden:

Subgraph Isomorphism based :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` Allocator. This QAllocator is split into 3 phases: 1.Partitions the program into a number of smaller programs, and find all\* subgraph isomorphisms from the graph of that program to the coupling graph (architecture); 2.Dynamic programming that tests all combinations of subgraph isomorphisms, while estimating the cost of glueing themtogether; 3.Reconstructs the selected sequence of subgraph isomorphismsinto a program.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OBMTQMapping.h>
	
	class OptBMTQAllocator: public :ref:`QPanda::AbstractQubitMapping<doxid-class_q_panda_1_1_abstract_qubit_mapping>`
	{
	public:
		// typedefs
	
		typedef OptBMTQAllocator* :target:`Ref<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1adb571a082d0fd53e6bc120aaf4798550>`;
		typedef std::unique_ptr<OptBMTQAllocator> :target:`uRef<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a6d202e96a601bff6dcd0856eb70eae89>`;

		// fields
	
		std::vector<std::vector<double>> :target:`mCnotReliability<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1ae0e2e11961b88c7a63790de42089d52a>`;
		std::vector<std::vector<double>> :target:`mSwapDist<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a238893c3ab952c8b1f0bde9266b0a0d3>`;
		std::vector<double> :target:`mMeaReliability<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a2601abe05aeb7769356adc5cb76fdf74>`;
		double :target:`mCirReliability<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a58e5ce92a83e570b52230ee414e4c709>` = 1.0;

		// methods
	
		static :ref:`uRef<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a6d202e96a601bff6dcd0856eb70eae89>` :target:`Create<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a5daccd30426f551a9c8867bcb34aa6a3>`(
			:ref:`QPanda::ArchGraph::sRef<doxid-class_q_panda_1_1_arch_graph_1a9c281b804cf8363fc16ce47e61b53de9>` ag,
			bool optimization = false,
			uint32_t max_partial = (std::numeric_limits<uint32_t>::max)(),
			uint32_t max_children = (std::numeric_limits<uint32_t>::max)()
			);
	
		static :ref:`QPanda::ArchGraph::sRef<doxid-class_q_panda_1_1_arch_graph_1a9c281b804cf8363fc16ce47e61b53de9>` :target:`build_arch_graph<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a7b2d04b59813b040cdf49894c34b6118>`(const std::string& config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`);
		void :target:`setChildrenSelector<doxid-class_q_panda_1_1_opt_b_m_t_q_allocator_1a36170aac7cd7500cac011c04f87879ca>`(:ref:`CandidateSelector::uRef<doxid-struct_q_panda_1_1_candidate_selector_1af31ad9af8ccee7de624d1482d3b69ef7>` sel);
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

