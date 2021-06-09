.. index:: pair: class; QPanda::QCodarMatch
.. _doxid-class_q_panda_1_1_q_codar_match:

class QPanda::QCodarMatch
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

A Contextual Duration-Aware :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` Mapping (CODAR) :ref:`More...<details-class_q_panda_1_1_q_codar_match>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCodarMatch.h>
	
	class QCodarMatch: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`QCodarMatch<doxid-class_q_panda_1_1_q_codar_match_1aacdf002ef2cf6ef28b5c8e367b4694cc>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog,
			:ref:`QCodarGridDevice<doxid-namespace_q_panda_1a5afaac3cd1651ac2f627fa78bd2d4f6c>` arch_type,
			int m,
			int n,
			const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`
			);

		// methods
	
		void :target:`initScheduler<doxid-class_q_panda_1_1_q_codar_match_1a86a446047ab6cedc900240e6ea72026f>`(
			:ref:`QCodarGridDevice<doxid-namespace_q_panda_1a5afaac3cd1651ac2f627fa78bd2d4f6c>` arch_type,
			size_t qubits
			);
	
		void :target:`initGridDevice<doxid-class_q_panda_1_1_q_codar_match_1ae2e87a4495c9091a30a6b97d24b722e3>`(
			:ref:`QCodarGridDevice<doxid-namespace_q_panda_1a5afaac3cd1651ac2f627fa78bd2d4f6c>` arch_type,
			int& m,
			int& n
			);
	
		void :ref:`mappingQProg<doxid-class_q_panda_1_1_q_codar_match_1afdc0d179fc13a9199783c9344ce2c534>`(size_t run_times, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog);
	
		void :ref:`buildResultingQProg<doxid-class_q_panda_1_1_q_codar_match_1a38a438e7c3ab5c9e431f27d0f5ac36e1>`(
			const std::vector<:ref:`GateInfo<doxid-struct_q_panda_1_1_gate_info>`> resulting_gates,
			const std::vector<int> map_vec,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& q,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :ref:`traversalQProgParsingInfo<doxid-class_q_panda_1_1_q_codar_match_1a2c553a4f8fd12059fde31f5107b7c865>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`* prog);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_codar_match_1aacd70fe25937a4dac3f174aedf007595>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_codar_match_1a56eb8ca4948ca29d94794d766397d2df>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_codar_match_1a25ff5c21409f0426b5d5629a05595c04>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_codar_match_1a9fa4728e86e81102260c0e3ed9614927>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_codar_match_1acf0a0bfa97d1095fd658e0b2e62164fe>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_codar_match_1a69e81e82b207fabdbb61227b27539a15>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_codar_match_1a9295113f8a6b65bab66d9861ede1962b>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1adb53e4c20d48a0efd6e377680d7f0988>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aed584073b781c9a5c6441b08b14afc3d>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aadbf69a810033196de1790d3f362ef7a>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aab65fda71b8e1f719bc4b7bdd70a10e7>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1ab452f71d25eb3354d46346694ff82db7>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a4e97902dc8b42d5f5f50d790d11f1517>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aa311fe1c6abc46d84d90d6f412be063a>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			);

.. _details-class_q_panda_1_1_q_codar_match:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A Contextual Duration-Aware :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` Mapping (CODAR)

Methods
-------

.. index:: pair: function; mappingQProg
.. _doxid-class_q_panda_1_1_q_codar_match_1afdc0d179fc13a9199783c9344ce2c534:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void mappingQProg(size_t run_times, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog)

Mapping qubits in a quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- run_times : the number of times run the remapping

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- qubits vector

	*
		- Qprog&

		- the mapped quantum program



.. rubric:: Returns:

void

.. index:: pair: function; buildResultingQProg
.. _doxid-class_q_panda_1_1_q_codar_match_1a38a438e7c3ab5c9e431f27d0f5ac36e1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void buildResultingQProg(
		const std::vector<:ref:`GateInfo<doxid-struct_q_panda_1_1_gate_info>`> resulting_gates,
		const std::vector<int> map_vec,
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& q,
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
		)

build :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` by the mapping results



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<GateInfo>

		- gates info vector

	*
		- std::vector<int>

		- map vector

	*
		- Qprog&

		- the mapped quantum program



.. rubric:: Returns:

void

.. index:: pair: function; traversalQProgParsingInfo
.. _doxid-class_q_panda_1_1_q_codar_match_1a2c553a4f8fd12059fde31f5107b7c865:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void traversalQProgParsingInfo(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`* prog)

traversal quantum program and Parsing quantum program information



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg\*

		- quantum program pointer



.. rubric:: Returns:

void

