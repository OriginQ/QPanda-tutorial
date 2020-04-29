.. index:: pair: class; QPanda::QProgToQMeasure
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure:

class QPanda::QProgToQMeasure
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

cast :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to :ref:`QMeasure <doxid-class_q_panda_1_1_q_measure>` :ref:`More...<details-class_q_panda_1_1_q_prog_to_q_measure>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgToQMeasure.h>
	
	class QProgToQMeasure: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_measure_1ade1511a4386f3d4c1ba751ebd58e7e60>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_measure_1a0599ba0c09c21ec3fc9961b4dd082986>`(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_measure_1afc6c85de2407fc79df67b29b06868fa9>`(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_measure_1a7d784bd90abbb09b5bfdc24daf178dcd>`(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_measure_1a57ba999a287f4ffa6630f0064437e1af>`(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_measure_1a8f49328d5d5ea5eaa649941542f54071>`(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_to_q_measure_1a49cb520462ea94d609c88ec118697a62>`(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> :target:`get_qmeasure<doxid-class_q_panda_1_1_q_prog_to_q_measure_1ab0ec0474a3c620eb68797732484eac30>`();
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

.. _details-class_q_panda_1_1_q_prog_to_q_measure:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

cast :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to :ref:`QMeasure <doxid-class_q_panda_1_1_q_measure>`

Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure_1ade1511a4386f3d4c1ba751ebd58e7e60:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure_1a0599ba0c09c21ec3fc9961b4dd082986:

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure_1afc6c85de2407fc79df67b29b06868fa9:

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure_1a7d784bd90abbb09b5bfdc24daf178dcd:

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure_1a57ba999a287f4ffa6630f0064437e1af:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node)

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure_1a8f49328d5d5ea5eaa649941542f54071:

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
.. _doxid-class_q_panda_1_1_q_prog_to_q_measure_1a49cb520462ea94d609c88ec118697a62:

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

