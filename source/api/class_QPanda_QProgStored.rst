.. index:: pair: class; QPanda::QProgStored
.. _doxid-class_q_panda_1_1_q_prog_stored:

class QPanda::QProgStored
=========================

.. toctree::
	:hidden:

	union_QPanda_QProgStored_DataNode.rst

Overview
~~~~~~~~

Utilities class for quantum program stored to binary data. :ref:`More...<details-class_q_panda_1_1_q_prog_stored>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgStored.h>
	
	class QProgStored: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// unions
	
		union :ref:`DataNode<doxid-union_q_panda_1_1_q_prog_stored_1_1_data_node>`;

		// construction
	
		:target:`QProgStored<doxid-class_q_panda_1_1_q_prog_stored_1a67c42b7f98fa59dbb968efa37b52fe77>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);

		// methods
	
		void :ref:`transform<doxid-class_q_panda_1_1_q_prog_stored_1a01fd4518f247f3e21d2f5e67027d1f01>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
		void :ref:`store<doxid-class_q_panda_1_1_q_prog_stored_1a2e843583ccc083b2d11e0f6bab494371>`(const std::string&);
		std::vector<uint8_t> :ref:`getInsturctions<doxid-class_q_panda_1_1_q_prog_stored_1a3c14c7592acbaa2f75a2b1bb2341281b>`();
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_stored_1a2e766476fb51855200c951dbc57488a5>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_stored_1aba2e8b266578fae20e492b1b9858c9fc>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_stored_1ad25b6cba45d6ae6a1f6e3bc8b87f4348>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_stored_1a415c4d125b2ce9550a95b97423ab0568>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_stored_1a3f029d8506de3ecd1a6bf66c2a4ff894>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_stored_1a582496bc937f3326b74a6350a6eccda4>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_stored_1a6e7b6907230b926671c9e8b4659cf713>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
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

.. _details-class_q_panda_1_1_q_prog_stored:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Utilities class for quantum program stored to binary data.

Methods
-------

.. index:: pair: function; transform
.. _doxid-class_q_panda_1_1_q_prog_stored_1a01fd4518f247f3e21d2f5e67027d1f01:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void transform(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

transform quantum program



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

void

.. index:: pair: function; store
.. _doxid-class_q_panda_1_1_q_prog_stored_1a2e843583ccc083b2d11e0f6bab494371:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void store(const std::string&)

Store quantum program data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- std::string& filename



.. rubric:: Returns:

void

.. index:: pair: function; getInsturctions
.. _doxid-class_q_panda_1_1_q_prog_stored_1a3c14c7592acbaa2f75a2b1bb2341281b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<uint8_t> getInsturctions()

get quantum program binary data



.. rubric:: Returns:

std::vector<uint8_t> quantum program binary data vector

