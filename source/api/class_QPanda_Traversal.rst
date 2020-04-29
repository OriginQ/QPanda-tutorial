.. index:: pair: class; QPanda::Traversal
.. _doxid-class_q_panda_1_1_traversal:

class QPanda::Traversal
=======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Traversing all the nodes of the linked qprog/qcircuit/control_flow_node. :ref:`More...<details-class_q_panda_1_1_traversal>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Traversal.h>
	
	class Traversal
	{
	public:
		// methods
	
		template <typename T, typename... Args>
		static void :ref:`traversal<doxid-class_q_panda_1_1_traversal_1a264fb3bbb9ae66571d47247572dc843a>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> control_flow_node,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
			Args&&... func_args
			);
	
		template <typename T, typename... Args>
		static void :ref:`traversal<doxid-class_q_panda_1_1_traversal_1aa2daec4b699425bfe553d96cc0e040b8>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> qcircuit_node,
			bool identify_dagger,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
			Args&&... func_args
			);
	
		template <typename T, typename... Args>
		static void :ref:`traversal<doxid-class_q_panda_1_1_traversal_1a6413204e195915ff3b418f4f5da1b429>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> qprog_node,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
			Args&&... func_args
			);
	
		template <typename T, typename... Args>
		static void :ref:`traversalByType<doxid-class_q_panda_1_1_traversal_1a28ad283edfd3ef5256adb9e3169d49a2>`(
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
			Args&&... func_args
			);
	};
.. _details-class_q_panda_1_1_traversal:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Traversing all the nodes of the linked qprog/qcircuit/control_flow_node.

Methods
-------

.. index:: pair: function; traversal
.. _doxid-class_q_panda_1_1_traversal_1a264fb3bbb9ae66571d47247572dc843a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename... Args>
	static void traversal(
		std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> control_flow_node,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
		Args&&... func_args
		)

Traversing qprog control flow circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractControlFlowNode\*

		- Control flow nodes that need to be traversed

	*
		- TraversalInterface\*

		- The method object needed for traversal



.. rubric:: Returns:

void

.. index:: pair: function; traversal
.. _doxid-class_q_panda_1_1_traversal_1aa2daec4b699425bfe553d96cc0e040b8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename... Args>
	static void traversal(
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> qcircuit_node,
		bool identify_dagger,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
		Args&&... func_args
		)

Traversing qcircuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumCircuit\*

		- :ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>` nodes that need to be traversed

	*
		- TraversalInterface\*

		- The method object needed for traversal

	*
		- bool

		- Whether the quantum circuit needs to be transposed



.. rubric:: Returns:

void

.. index:: pair: function; traversal
.. _doxid-class_q_panda_1_1_traversal_1a6413204e195915ff3b418f4f5da1b429:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename... Args>
	static void traversal(
		std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> qprog_node,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
		Args&&... func_args
		)

Traversing qprog.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- AbstractQuantumProgram\*

		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` nodes that need to be traversed

	*
		- TraversalInterface\*

		- The method object needed for traversal



.. rubric:: Returns:

void

.. index:: pair: function; traversalByType
.. _doxid-class_q_panda_1_1_traversal_1a28ad283edfd3ef5256adb9e3169d49a2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T, typename... Args>
	static void traversalByType(
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node,
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& func_class,
		Args&&... func_args
		)

traversalByType



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QNode\*

		- nodes that need to be traversed

	*
		- parent_node\*

		- nodes that need to be traversed

	*
		- TraversalInterface\*

		- The method object needed for traversal



.. rubric:: Returns:

void

