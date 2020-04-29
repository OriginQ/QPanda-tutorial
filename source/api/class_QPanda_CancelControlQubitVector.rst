.. index:: pair: class; QPanda::CancelControlQubitVector
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector:

class QPanda::CancelControlQubitVector
======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Cancel control qubit vector in qprog. :ref:`More...<details-class_q_panda_1_1_cancel_control_qubit_vector>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TransformDecomposition.h>
	
	class CancelControlQubitVector: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		void :ref:`execute<doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a8596c56b70815266956e49d3c84e74a1>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		void :ref:`execute<doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a8762d444afca1a72456ef3a4cbfbaffc>`(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a7b265896b9f295c49bab7c64dbacf08b>`(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a982e82d1453ffbb8bd203d0f3e053d47>`(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_cancel_control_qubit_vector_1ae97de0465d0b4ef5fac0765769a4428d>`(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a2e5e0b8de3f4b2a6e1b63facde82cb44>`(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a23a68678b108ac45a132502d61f97a87>`(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
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

.. _details-class_q_panda_1_1_cancel_control_qubit_vector:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Cancel control qubit vector in qprog.

Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a8596c56b70815266956e49d3c84e74a1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void execute(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qgatenode.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQGateNode\*

		- quantum gate

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a8762d444afca1a72456ef3a4cbfbaffc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void execute(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qcircuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumCircuit\*

		- quantum circuit

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a7b265896b9f295c49bab7c64dbacf08b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal measure node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumMeasure\*

		- measure node

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a982e82d1453ffbb8bd203d0f3e053d47:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal reset node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumReset\*

		- reset node

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector_1ae97de0465d0b4ef5fac0765769a4428d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal control flow node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractControlFlowNode\*

		- control flow node

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a2e5e0b8de3f4b2a6e1b63facde82cb44:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qprog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumProgram\*

		- quantum prog

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_cancel_control_qubit_vector_1a23a68678b108ac45a132502d61f97a87:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

Execution traversal qprog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractClassicalProg\*

		- quantum prog

	*
		- AbstractQGateNode\*

		- quantum gate



.. rubric:: Returns:

void

