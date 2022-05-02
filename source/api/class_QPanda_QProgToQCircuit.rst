.. index:: pair: class; QPanda::QProgToQCircuit
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit:

class QPanda::QProgToQCircuit
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

cast :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to :ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>` :ref:`More...<details-class_q_panda_1_1_q_prog_to_q_circuit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgToQCircuit.h>
	
	class QProgToQCircuit: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_circuit_1ae7bcedcab6519d38c99c5bbe9898bfd4>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a8b2e4bd8eae0388d1d83a44eaa299e24>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_circuit_1aad5bfa0416c7c6d7a82db5f70f6aaeb9>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a1c8741d88c4cbc4b3e1eb88a8b98f6ab>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_circuit_1ad75af973b9c5849e5aac1db879c4f65d>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a0287980b4c4b2714ec09e553d5e62f7c>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a14b0eb9b85e2496cb5b94629de52e5a1>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
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

.. _details-class_q_panda_1_1_q_prog_to_q_circuit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

cast :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to :ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`

Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit_1ae7bcedcab6519d38c99c5bbe9898bfd4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a8b2e4bd8eae0388d1d83a44eaa299e24:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit_1aad5bfa0416c7c6d7a82db5f70f6aaeb9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a1c8741d88c4cbc4b3e1eb88a8b98f6ab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit_1ad75af973b9c5849e5aac1db879c4f65d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a0287980b4c4b2714ec09e553d5e62f7c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_circuit_1a14b0eb9b85e2496cb5b94629de52e5a1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& circuit
		)

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

