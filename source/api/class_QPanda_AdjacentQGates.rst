.. index:: pair: class; QPanda::AdjacentQGates
.. _doxid-class_q_panda_1_1_adjacent_q_gates:

class QPanda::AdjacentQGates
============================

.. toctree::
	:hidden:

	class_QPanda_AdjacentQGates_AbstractTraversalStatueInterface.rst
	class_QPanda_AdjacentQGates_FoundAllAdjacentNode.rst
	class_QPanda_AdjacentQGates_HaveNotFoundTargetNode.rst
	class_QPanda_AdjacentQGates_ToFindBackNode.rst

Overview
~~~~~~~~

Get information about adjacent nodes. :ref:`More...<details-class_q_panda_1_1_adjacent_q_gates>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <GetAdjacentNodes.h>
	
	class AdjacentQGates: public :ref:`QPanda::TraverseByNodeIter<doxid-class_q_panda_1_1_traverse_by_node_iter>`
	{
	public:
		// classes
	
		class :ref:`AbstractTraversalStatueInterface<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_abstract_traversal_statue_interface>`;
		class :ref:`FoundAllAdjacentNode<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_found_all_adjacent_node>`;
		class :ref:`HaveNotFoundTargetNode<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_have_not_found_target_node>`;
		class :ref:`ToFindBackNode<doxid-class_q_panda_1_1_adjacent_q_gates_1_1_to_find_back_node>`;

		// construction
	
		:target:`AdjacentQGates<doxid-class_q_panda_1_1_adjacent_q_gates_1a856c1aa25b558aa45c1c03977e898cec>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr
			);

		// methods
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_adjacent_q_gates_1a75f5e05279716129d526b460d1dfd9d6>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_adjacent_q_gates_1a60bae92a5ee4fddbb2c1441fb5c5a2cc>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_adjacent_q_gates_1ab29d733e88af79d50fdb62f0dcb18790>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_adjacent_q_gates_1aa08291576b8f6f4be536c63055f180ec>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_adjacent_q_gates_1a4d8ad97f452bb18196addccb09db9b69>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_adjacent_q_gates_1a31817f1d297385fbff9afb361745a990>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_adjacent_q_gates_1a6cf6becfd4542c03dfad2abade79fef6>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_adjacent_q_gates_1aaa74c3f6608c3d47306aa73e96e42fef>`();
	
		void :target:`updateFrontIter<doxid-class_q_panda_1_1_adjacent_q_gates_1a85a59c8774e508fd0e7408b0b9c0e1ea>`(
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& itr,
			const :ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`updateBackIter<doxid-class_q_panda_1_1_adjacent_q_gates_1a20010bff9444676d52932f878ebbc0de>`(
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& itr,
			const :ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :target:`getFrontIterNodeType<doxid-class_q_panda_1_1_adjacent_q_gates_1a4572dca852908ac90ceabc05c24e1321>`();
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :target:`getBackIterNodeType<doxid-class_q_panda_1_1_adjacent_q_gates_1ae2d9e06e198fe1596a2fd29aab245d4e>`();
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :target:`getItrNodeType<doxid-class_q_panda_1_1_adjacent_q_gates_1a4758eedc50d40eadee0c6b3398bcf351>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& ter);
		std::string :target:`getItrNodeTypeStr<doxid-class_q_panda_1_1_adjacent_q_gates_1a9e72e609dba92e8dd0902139a7df6141>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& ter);
		std::string :target:`getBackIterNodeTypeStr<doxid-class_q_panda_1_1_adjacent_q_gates_1ac3b2e054f93a1955a16e72d8c1f5aee4>`();
		std::string :target:`getFrontIterNodeTypeStr<doxid-class_q_panda_1_1_adjacent_q_gates_1a9420d579110095f1974e9c1febe9a03d>`();
		bool :target:`isValidNodeType<doxid-class_q_panda_1_1_adjacent_q_gates_1a0fdd9689320e65906171028b32fea37d>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& itr);
		bool :target:`isValidNodeType<doxid-class_q_panda_1_1_adjacent_q_gates_1ac95975acb0d17e56d71d6144a3035b5a>`(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` t);
		const :ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`& :target:`getFrontNode<doxid-class_q_panda_1_1_adjacent_q_gates_1a4fd1eba4c5c1d7ec3c4ec59e541c2297>`();
		const :ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`& :target:`getBackNode<doxid-class_q_panda_1_1_adjacent_q_gates_1ac0fef19215659c800f59990e4d536833>`();
		void :target:`changeTraversalStatue<doxid-class_q_panda_1_1_adjacent_q_gates_1a89a949e0e04e5904834fe005472ba8b4>`(AbstractTraversalStatueInterface* s);
		static bool :target:`isSubProgNode<doxid-class_q_panda_1_1_adjacent_q_gates_1a357648b447853847ac6b51dfa233d33f>`(const std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& node);
		static bool :target:`isFlowCtrlNode<doxid-class_q_panda_1_1_adjacent_q_gates_1ad55677f6167897601e37ddbd4340d5e5>`(const std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& node);
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
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab322f1c7e3734cf25d22c57c1dfe6e98>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a73c8f60de984e2aa5705211b361d98e1>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1aeea9c768792ed69bccd8cd9418fa9180>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1af01742419980d7fc620f085fffcc319b>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a95859495e9b97db265dc1a0932836366>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1adadb977d5747ba2f307f6f8d7bf49742>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab5039119411bc0f91236fac876fc606f>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_traverse_by_node_iter_1a407bc9a3cc75874142fbfec69447e9e2>`();

.. _details-class_q_panda_1_1_adjacent_q_gates:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Get information about adjacent nodes.

Methods
-------

.. index:: pair: function; traverse_qprog
.. _doxid-class_q_panda_1_1_adjacent_q_gates_1aaa74c3f6608c3d47306aa73e96e42fef:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void traverse_qprog()

start traverse a quantum prog

