.. index:: pair: class; QPanda::TopologyMatch
.. _doxid-class_q_panda_1_1_topology_match:

class QPanda::TopologyMatch
===========================

.. toctree::
	:hidden:

	struct_QPanda_TopologyMatch_edge.rst
	struct_QPanda_TopologyMatch_gate.rst
	struct_QPanda_TopologyMatch_node.rst
	struct_QPanda_TopologyMatch_node_cmp.rst

Overview
~~~~~~~~

QProg/QCircuit matches the topology of the physical qubits. :ref:`More...<details-class_q_panda_1_1_topology_match>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TopologyMatch: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// structs
	
		struct :ref:`edge<doxid-struct_q_panda_1_1_topology_match_1_1edge>`;
		struct :ref:`gate<doxid-struct_q_panda_1_1_topology_match_1_1gate>`;
		struct :ref:`node<doxid-struct_q_panda_1_1_topology_match_1_1node>`;
		struct :ref:`node_cmp<doxid-struct_q_panda_1_1_topology_match_1_1node__cmp>`;

		// construction
	
		:target:`TopologyMatch<doxid-class_q_panda_1_1_topology_match_1afe4c974b8e2444336fc7fed8ccae1869>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog,
			:ref:`SwapQubitsMethod<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73>` method = :ref:`CNOT_GATE_METHOD<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73af0fd6c0d21b2b49d98160f724cff9cbe>`,
			:ref:`ArchType<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2a>` arch_type = :ref:`IBM_QX5_ARCH<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2aa1d998a495737ef4502e83b080f3dada0>`,
			const std::string conf = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`
			);

		// methods
	
		void :ref:`mappingQProg<doxid-class_q_panda_1_1_topology_match_1a6b5bf04991ba44cfc9165d9322e602bb>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_topology_match_1a83fb3a65558ed1b9b529e596cf43c7fc>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_topology_match_1aa71f6c95041a59229d35dd71fd2f3a32>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_topology_match_1ad0c48f556dc4aa0bb524574a8e32f82b>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_topology_match_1a52ef7a35da10864a323a0bff57c78e05>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_topology_match_1af95f9b874ad73b74c9a96e74afa92e00>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_topology_match_1ae4eb4ba04dcce79349e7d028cbf3b0fc>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_topology_match_1a726b1fe66d0c9fcdcc8f92c7186f3c0d>`(
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

.. _details-class_q_panda_1_1_topology_match:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QProg/QCircuit matches the topology of the physical qubits.

Methods
-------

.. index:: pair: function; mappingQProg
.. _doxid-class_q_panda_1_1_topology_match_1a6b5bf04991ba44cfc9165d9322e602bb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void mappingQProg(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog)

Mapping qubits in a quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qprog

		- quantum program

	*
		- Qprog&

		- the mapped quantum program



.. rubric:: Returns:

void

