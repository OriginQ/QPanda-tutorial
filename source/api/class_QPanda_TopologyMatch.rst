.. index:: pair: class; QPanda::TopologyMatch
.. _doxid-class_q_panda_1_1_topology_match:

class QPanda::TopologyMatch
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QProg/QCircuit matches the topology of the physical qubits. :ref:`More...<details-class_q_panda_1_1_topology_match>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TopologyMatch: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`TopologyMatch<doxid-class_q_panda_1_1_topology_match_1a34f357540221de68db9433e2f9bf5d37>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
			:ref:`SwapQubitsMethod<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73>` method = :ref:`CNOT_GATE_METHOD<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73af0fd6c0d21b2b49d98160f724cff9cbe>`,
			:ref:`ArchType<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2a>` arch_type = :ref:`IBM_QX5_ARCH<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2aa1d998a495737ef4502e83b080f3dada0>`
			);

		// methods
	
		void :ref:`mappingQProg<doxid-class_q_panda_1_1_topology_match_1a7efaa5d48df471466f7d3a7a94c73d5e>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog);
	
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
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a1cb0c50abcd626b8c45b8aa389cb3541>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a6916170c055781c5ed5a615407390e1c>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1aa3389601eef27921246507d9bcd60e8f>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a2196c7ad5525e519cfedad3d0285d712>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a34a63b4019719d77711fcf6efbb6400c>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a310247426bda77a52b81c7654fa4b848>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traversal_interface_1a7d2fb53e43f56cc2f57cf0d025585146>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			Args&&... func_args
			) = 0;

.. _details-class_q_panda_1_1_topology_match:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QProg/QCircuit matches the topology of the physical qubits.

Methods
-------

.. index:: pair: function; mappingQProg
.. _doxid-class_q_panda_1_1_topology_match_1a7efaa5d48df471466f7d3a7a94c73d5e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void mappingQProg(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog)

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

