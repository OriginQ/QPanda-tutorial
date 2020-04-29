.. index:: pair: class; QPanda::QProgFlattening
.. _doxid-class_q_panda_1_1_q_prog_flattening:

class QPanda::QProgFlattening
=============================

.. toctree::
	:hidden:

flatten quantum program and quantum circuit


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgFlattening.h>
	
	class QProgFlattening: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`QProgFlattening<doxid-class_q_panda_1_1_q_prog_flattening_1abcc78022558016b87a5114d04956a27b>`(bool is_full_faltten = false);

		// methods
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a3fac22a5cb006cd2d4aa8f420892e9ad>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1af0a2d0abf83b362f6b0246667ff653db>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a70b7df440b769b60ebfc43c59bad0f2b>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a6a47382976195995753a0773abe9d2a2>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a52b4310ebea577f3c4061f70f933cc83>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1aad2dda6669bed9e60f78368e7b4d82f2>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a4a8678b6f35a6047f8219836ee17f4f8>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		void :target:`flatten_by_type<doxid-class_q_panda_1_1_q_prog_flattening_1aa43a171ffb2ec696448fe82ed9b5d268>`(
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& out_prog,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& out_circuit
			);
	
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`get_two_qvec_union<doxid-class_q_panda_1_1_q_prog_flattening_1ab02df36b9032673f4add378981b5dcc9>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qv_1,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qv_2
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

