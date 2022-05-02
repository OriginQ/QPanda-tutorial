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

Get information about adjacent nodes.


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
	
		:target:`AdjacentQGates<doxid-class_q_panda_1_1_adjacent_q_gates_1af6c3f4e0c5eb7a3a049350b0e8d7c79c>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog,
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
	
		virtual void :target:`traverse_qprog<doxid-class_q_panda_1_1_adjacent_q_gates_1aeba938c0af3f147a2a2455d785e85332>`();
	
		void :target:`update_front_iter<doxid-class_q_panda_1_1_adjacent_q_gates_1acdd3bf0470904cbb444ccafc2c498558>`(
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& itr,
			const :ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		void :target:`update_back_iter<doxid-class_q_panda_1_1_adjacent_q_gates_1a1a19538260f28ac7d77916967e423c4c>`(
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& itr,
			const :ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param
			);
	
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :target:`get_node_ype<doxid-class_q_panda_1_1_adjacent_q_gates_1af6e816d652206a633d7b36b909355518>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& ter);
		std::string :target:`get_node_type_str<doxid-class_q_panda_1_1_adjacent_q_gates_1ac37bb57694dfe97ee8fba03041d0b8c2>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& ter);
		std::string :target:`get_back_node_type_str<doxid-class_q_panda_1_1_adjacent_q_gates_1ae03a23cb69ed0006a47f8c8cac811573>`();
		std::string :target:`get_front_node_type_str<doxid-class_q_panda_1_1_adjacent_q_gates_1af1e8533806bd44a09dc389682727462d>`();
		bool :target:`is_valid_node_type<doxid-class_q_panda_1_1_adjacent_q_gates_1ae635ee08f9263bc6c9e8a49cafe9ca24>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& itr);
		bool :target:`is_valid_node_type<doxid-class_q_panda_1_1_adjacent_q_gates_1aaae6667b744b2ae58ed6d445b926c199>`(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` t);
		const :ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`& :target:`get_front_node<doxid-class_q_panda_1_1_adjacent_q_gates_1a858a2f9136224015a1ecedbd7eb76a64>`();
		const :ref:`NodeInfo<doxid-class_q_panda_1_1_node_info>`& :target:`get_back_node<doxid-class_q_panda_1_1_adjacent_q_gates_1a13c3be64245e2616b7fdbd9628a9eaed>`();
		void :target:`change_traversal_statue<doxid-class_q_panda_1_1_adjacent_q_gates_1ae96da1f378babd42506e7ed3ffb3c866>`(AbstractTraversalStatueInterface* s);
		static bool :target:`is_sub_prog_node<doxid-class_q_panda_1_1_adjacent_q_gates_1a39c02de1d08da426ba8cf0a5247ab3fe>`(const std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& node);
		static bool :target:`is_flow_ctrl_node<doxid-class_q_panda_1_1_adjacent_q_gates_1aedb92a399c4e8841f117e0028bf126d2>`(const std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& node);
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
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab298ca4e8835cb14518f8b83c87d6287>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);

