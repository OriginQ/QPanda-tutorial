.. index:: pair: class; QPanda::QProgCheck
.. _doxid-class_q_panda_1_1_q_prog_check:

class QPanda::QProgCheck
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Qunatum :ref:`QProgCheck <doxid-class_q_panda_1_1_q_prog_check>`. :ref:`More...<details-class_q_panda_1_1_q_prog_check>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgCheck.h>
	
	class QProgCheck
	{
	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_check_1a1af9dc52be7e351eedf35c0912a74439>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_check_1a874fe9e75d25bc5b664d271e8b7e21b9>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_check_1acd5a4b4dd60c83dd3cec5644d1868bdf>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_check_1aff243d0817632f7bb8831a7cf1ce9549>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_check_1a5992f4eeb7092986cb8feea4d8358dcc>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_check_1a33273624a4ad8d714c80319d76030205>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& paramu
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_check_1ad16b8082507970443628911fba590340>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
			);
	};
.. _details-class_q_panda_1_1_q_prog_check:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Qunatum :ref:`QProgCheck <doxid-class_q_panda_1_1_q_prog_check>`.

Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_check_1a1af9dc52be7e351eedf35c0912a74439:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
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

	*
		- :ref:`TraversalConfig <doxid-class_q_panda_1_1_traversal_config>`

		- traversal config

	*
		- QPUImpl\*

		- virtual quantum processor



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_check_1a874fe9e75d25bc5b664d271e8b7e21b9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
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

	*
		- :ref:`TraversalConfig <doxid-class_q_panda_1_1_traversal_config>`

		- traversal config

	*
		- QPUImpl\*

		- virtual quantum processor



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_check_1acd5a4b4dd60c83dd3cec5644d1868bdf:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
		)

Execution traversal reset node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumReset\*

		- reset node

	*
		- QNode\*

		- parent node

	*
		- :ref:`TraversalConfig <doxid-class_q_panda_1_1_traversal_config>`

		- traversal config

	*
		- QPUImpl\*

		- virtual quantum processor



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_check_1aff243d0817632f7bb8831a7cf1ce9549:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
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

	*
		- :ref:`TraversalConfig <doxid-class_q_panda_1_1_traversal_config>`

		- traversal config

	*
		- QPUImpl\*

		- virtual quantum processor



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_check_1a5992f4eeb7092986cb8feea4d8358dcc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
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

	*
		- :ref:`TraversalConfig <doxid-class_q_panda_1_1_traversal_config>`

		- traversal config

	*
		- QPUImpl\*

		- virtual quantum processor



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_check_1a33273624a4ad8d714c80319d76030205:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& paramu
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

	*
		- :ref:`TraversalConfig <doxid-class_q_panda_1_1_traversal_config>`

		- traversal config

	*
		- QPUImpl\*

		- virtual quantum processor



.. rubric:: Returns:

void

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_check_1ad16b8082507970443628911fba590340:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param
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

	*
		- :ref:`TraversalConfig <doxid-class_q_panda_1_1_traversal_config>`

		- traversal config

	*
		- QPUImpl\*

		- virtual quantum processor



.. rubric:: Returns:

void

