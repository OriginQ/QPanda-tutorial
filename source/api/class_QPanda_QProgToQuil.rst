.. index:: pair: class; QPanda::QProgToQuil
.. _doxid-class_q_panda_1_1_q_prog_to_quil:

class QPanda::QProgToQuil
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QuantumProg Transform To Quil instruction sets. :ref:`More...<details-class_q_panda_1_1_q_prog_to_quil>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgToQuil.h>
	
	class QProgToQuil: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`QProgToQuil<doxid-class_q_panda_1_1_q_prog_to_quil_1a410f26b6bb0355a12acbbdf1915af9ff>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine);

		// methods
	
		virtual void :ref:`transform<doxid-class_q_panda_1_1_q_prog_to_quil_1a99b1689d775e339edad54c477c432b75>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
		virtual std::string :ref:`getInsturctions<doxid-class_q_panda_1_1_q_prog_to_quil_1a69881bec169a2b73f1e1176cff5ceb08>`();
		void :ref:`transformQProgByTraversalAlg<doxid-class_q_panda_1_1_q_prog_to_quil_1ae9c39756138a1c6cfd8e0a8447c83b54>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`* prog);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_quil_1a7278e9cd940c44cee8fbc533b3b21cdf>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_quil_1abaed286165daa63507510704c95e7861>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_quil_1a4fbe9388d863a68e61e0178e7d22285b>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_quil_1a036cb2e3e5fd71bc7b4712a7d0a6035a>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_quil_1a1308f0e081a2975d2d973c2fbc870bbf>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_quil_1a786bf8401385e547e049ceb035926ebf>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_quil_1abf7a5ad15f6de29833cedee79f2f4f94>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
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

.. _details-class_q_panda_1_1_q_prog_to_quil:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QuantumProg Transform To Quil instruction sets.

Methods
-------

.. index:: pair: function; transform
.. _doxid-class_q_panda_1_1_q_prog_to_quil_1a99b1689d775e339edad54c477c432b75:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void transform(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

transform quantum program



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

void

.. index:: pair: function; getInsturctions
.. _doxid-class_q_panda_1_1_q_prog_to_quil_1a69881bec169a2b73f1e1176cff5ceb08:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getInsturctions()

get Quil insturction set



.. rubric:: Returns:

std::string

.. index:: pair: function; transformQProgByTraversalAlg
.. _doxid-class_q_panda_1_1_q_prog_to_quil_1ae9c39756138a1c6cfd8e0a8447c83b54:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void transformQProgByTraversalAlg(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`* prog)

Transform Quantum program by :ref:`Traversal <doxid-class_q_panda_1_1_traversal>` algorithm, refer to class :ref:`Traversal <doxid-class_q_panda_1_1_traversal>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

void

