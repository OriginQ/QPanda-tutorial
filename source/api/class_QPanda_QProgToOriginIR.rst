.. index:: pair: class; QPanda::QProgToOriginIR
.. _doxid-class_q_panda_1_1_q_prog_to_origin_i_r:

class QPanda::QProgToOriginIR
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QuantumProg Transform To OriginIR instruction sets. :ref:`More...<details-class_q_panda_1_1_q_prog_to_origin_i_r>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgToOriginIR.h>
	
	class QProgToOriginIR: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`QProgToOriginIR<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a179380d0a9dcc0ad99a31296e0cf59a8>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine);

		// methods
	
		virtual void :ref:`transform<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a1b6a00a4680bc5f92cd6010492a1ac93>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
	
		template <typename _Ty>
		void :target:`traversal<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a16a1fd80adb0ad7d13b995db48e473e1>`(_Ty& node);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a1d20587bb883eef3312d70d9164527e3>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a4fc1fe77333c9591e8d54279dfdbb8e4>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a8576775ecc24535b968216cf5111faf0>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1ac74fd6dfe359665895516eef0f64acc0>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a545a7505fd5d6f77919a9ec73fe08d71>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a83ebc082a45052b69213fce3cbddf58e>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a9cbdb81cced450539ee920eaf0f6d551>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node
			);
	
		virtual std::string :ref:`getInsturctions<doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a7d1499b5b5388303b5ac7744f2c03f49>`();
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

.. _details-class_q_panda_1_1_q_prog_to_origin_i_r:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QuantumProg Transform To OriginIR instruction sets.

Methods
-------

.. index:: pair: function; transform
.. _doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a1b6a00a4680bc5f92cd6010492a1ac93:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void transform(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

Transform quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

void

.. index:: pair: function; getInsturctions
.. _doxid-class_q_panda_1_1_q_prog_to_origin_i_r_1a7d1499b5b5388303b5ac7744f2c03f49:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getInsturctions()

get OriginIR insturction set



.. rubric:: Returns:

std::string

