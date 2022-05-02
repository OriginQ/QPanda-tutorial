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

