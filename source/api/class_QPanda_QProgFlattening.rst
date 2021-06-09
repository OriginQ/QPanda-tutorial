.. index:: pair: class; QPanda::QProgFlattening
.. _doxid-class_q_panda_1_1_q_prog_flattening:

class QPanda::QProgFlattening
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

flatten quantum program and quantum circuit :ref:`More...<details-class_q_panda_1_1_q_prog_flattening>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgFlattening.h>
	
	class QProgFlattening: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`QProgFlattening<doxid-class_q_panda_1_1_q_prog_flattening_1a7ba7100ecf8d6ec952722b8be7832899>`(bool is_full_faltten = true);

		// methods
	
		void :target:`flatten_circuit<doxid-class_q_panda_1_1_q_prog_flattening_1a170139360689abf173dcf33399292aff>`(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& src_cir);
		void :target:`flatten_prog<doxid-class_q_panda_1_1_q_prog_flattening_1a1cfb85559dea4ad3316d63e2a35b23a0>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& src_prog);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1af4d57cc4e45317ef0e8ba854bf6a564b>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a3d4b99cd94470b232040a443afee6cd0>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1af2ceeb51f43296e7b3844f6793e7320c>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a8b83a0526d81b2514426c76c5a165522>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a5ab3df8d36f661beee00d5d3fb000e67>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a2d4565d77de79e169dce8960ef9868b7>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_flattening_1a263b3d44b8741a421686d0878aa11eec>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		static :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`prog_flatten_to_cir<doxid-group___utilities_1gabf5a4452e825f39dd89cef74b375d8dc>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
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

.. _details-class_q_panda_1_1_q_prog_flattening:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

flatten quantum program and quantum circuit

Methods
-------

.. index:: pair: function; prog_flatten_to_cir
.. _doxid-group___utilities_1gabf5a4452e825f39dd89cef74b375d8dc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` prog_flatten_to_cir(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

Flatten :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to :ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- the target :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`



.. rubric:: Returns:

Converted circuit @Note: The input :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` must be no-nesting, and only :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` type is supported.

