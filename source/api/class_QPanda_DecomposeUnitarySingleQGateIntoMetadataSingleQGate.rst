.. index:: pair: class; QPanda::DecomposeUnitarySingleQGateIntoMetadataSingleQGate
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate:

class QPanda::DecomposeUnitarySingleQGateIntoMetadataSingleQGate
================================================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Decomposing unitary single qgate into metadata single qgate in qprog. :ref:`More...<details-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TransformDecomposition.h>
	
	class DecomposeUnitarySingleQGateIntoMetadataSingleQGate: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`DecomposeUnitarySingleQGateIntoMetadataSingleQGate<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1adbd504cb21cb4a80257a4576e4b94b17>`(
			std::vector<std::vector<std::string>> qgate_matrix,
			std::vector<std::vector<std::string>>& valid_qgate_matrix
			);

		// methods
	
		void :ref:`execute<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a371e3be60860f57d31cd02b1ea833cef>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a183a4a4f437ab6bf14f9a7ee73dbd896>`(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a5228530197be13937585f607974f3ed4>`(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1aef78bee4ab10eed77a8737eafb11bd6d>`(std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1aec4eb51f673dfcbe5d34c23aaa606e05>`(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1ae048a00ae87be4fca71d66e9a5c37d6f>`(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
		virtual void :ref:`execute<doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a61e617886203e7f5ded7c3c6acd1eb18>`(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node);
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

.. _details-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Decomposing unitary single qgate into metadata single qgate in qprog.

Methods
-------

.. index:: pair: function; execute
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a371e3be60860f57d31cd02b1ea833cef:

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
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a183a4a4f437ab6bf14f9a7ee73dbd896:

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
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a5228530197be13937585f607974f3ed4:

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
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1aef78bee4ab10eed77a8737eafb11bd6d:

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
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1aec4eb51f673dfcbe5d34c23aaa606e05:

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
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1ae048a00ae87be4fca71d66e9a5c37d6f:

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
.. _doxid-class_q_panda_1_1_decompose_unitary_single_q_gate_into_metadata_single_q_gate_1a61e617886203e7f5ded7c3c6acd1eb18:

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

