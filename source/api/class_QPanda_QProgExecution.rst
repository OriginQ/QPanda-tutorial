.. index:: pair: class; QPanda::QProgExecution
.. _doxid-class_q_panda_1_1_q_prog_execution:

class QPanda::QProgExecution
============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Qunatum Execution. :ref:`More...<details-class_q_panda_1_1_q_prog_execution>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgExecution.h>
	
	class QProgExecution
	{
	public:
		// methods
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_execution_1a966f9d5c43b67d5119c48daeb3f3cd1e>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_execution_1a563963e4aaedd262182cb6104ce1a904>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_execution_1af07ecb2c67cff5e9271ef30f440f525d>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_execution_1aeae5e229609cedd06b9dde140b5b86ec>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_execution_1a999d22f945b16297062cdbff50134884>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_execution_1ada5ddf5df30b2dee029d0cc37bd290ca>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_q_prog_execution_1ae5201ee2cc2d58a7973c5e2daeaac167>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
			);
	
		void :ref:`get_return_value<doxid-class_q_panda_1_1_q_prog_execution_1ae77b5a3ebdbda8ad84e02d7bdc80024b>`(std::map<std::string, bool>& result);
	};
.. _details-class_q_panda_1_1_q_prog_execution:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Qunatum Execution.

Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_q_prog_execution_1a966f9d5c43b67d5119c48daeb3f3cd1e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
		:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
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
.. _doxid-class_q_panda_1_1_q_prog_execution_1a563963e4aaedd262182cb6104ce1a904:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
		:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
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
.. _doxid-class_q_panda_1_1_q_prog_execution_1af07ecb2c67cff5e9271ef30f440f525d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
		:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
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
.. _doxid-class_q_panda_1_1_q_prog_execution_1aeae5e229609cedd06b9dde140b5b86ec:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
		:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
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
.. _doxid-class_q_panda_1_1_q_prog_execution_1a999d22f945b16297062cdbff50134884:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
		:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
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
.. _doxid-class_q_panda_1_1_q_prog_execution_1ada5ddf5df30b2dee029d0cc37bd290ca:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
		:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
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
.. _doxid-class_q_panda_1_1_q_prog_execution_1ae5201ee2cc2d58a7973c5e2daeaac167:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void execute(
		std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param,
		:ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu
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

.. index:: pair: function; get_return_value
.. _doxid-class_q_panda_1_1_q_prog_execution_1ae77b5a3ebdbda8ad84e02d7bdc80024b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void get_return_value(std::map<std::string, bool>& result)

get result value



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::map<std::string

		- 

	*
		- bool>

		- & result map

