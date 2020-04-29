.. index:: pair: class; QPanda::JudgeTwoNodeIterIsSwappable
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable:

class QPanda::JudgeTwoNodeIterIsSwappable
=========================================

.. toctree::
	:hidden:

	class_QPanda_JudgeTwoNodeIterIsSwappable_AbstractJudgeStatueInterface.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_CanNotBeExchange.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_CoubleBeExchange.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_OnInitStatue.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_OnJudgeLayerInfo.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_OnPickUpNode.rst

Overview
~~~~~~~~

Judge two node is swappable. :ref:`More...<details-class_q_panda_1_1_judge_two_node_iter_is_swappable>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <JudgeTwoNodeIterIsSwappable.h>
	
	class JudgeTwoNodeIterIsSwappable: public :ref:`QPanda::TraverseByNodeIter<doxid-class_q_panda_1_1_traverse_by_node_iter>`
	{
	public:
		// classes
	
		class :ref:`AbstractJudgeStatueInterface<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface>`;
		class :ref:`CanNotBeExchange<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_can_not_be_exchange>`;
		class :ref:`CoubleBeExchange<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_couble_be_exchange>`;
		class :ref:`OnInitStatue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue>`;
		class :ref:`OnJudgeLayerInfo<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_judge_layer_info>`;
		class :ref:`OnPickUpNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node>`;

		// construction
	
		:ref:`JudgeTwoNodeIterIsSwappable<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a59c4523affea4adb4dec20c508bfcce7>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_1, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_2);

		// methods
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a5824b7748c95f61fa82c66675629d5a7>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1acf0694ae685f5bb49ce786be2d65a3a0>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1af71e5441f4dd16eb78cdb188b17e714d>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a269bbd839e44f75a913def139f9290f2>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a40fddf390915f71d4d89ffb53a01187e>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1acc472e761ffd92775000c8f6b66e7080>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a294f75ddd8e21827e2266ee700956a12>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		bool :ref:`getResult<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1abbb830fa02bdac8614dfee99c902e464>`();
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a8dabbdb29ac5c475dc6ded45fae27e4e>`();
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
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab322f1c7e3734cf25d22c57c1dfe6e98>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a73c8f60de984e2aa5705211b361d98e1>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1aeea9c768792ed69bccd8cd9418fa9180>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1af01742419980d7fc620f085fffcc319b>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1a95859495e9b97db265dc1a0932836366>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1adadb977d5747ba2f307f6f8d7bf49742>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`execute<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab5039119411bc0f91236fac876fc606f>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`& cir_param,
			:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& cur_node_iter
			);
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_traverse_by_node_iter_1a407bc9a3cc75874142fbfec69447e9e2>`();

.. _details-class_q_panda_1_1_judge_two_node_iter_is_swappable:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Judge two node is swappable.

Construction
------------

.. index:: pair: function; JudgeTwoNodeIterIsSwappable
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a59c4523affea4adb4dec20c508bfcce7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	JudgeTwoNodeIterIsSwappable(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_1, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_2)

Constructor of :ref:`JudgeTwoNodeIterIsSwappable <doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable>`.

Methods
-------

.. index:: pair: function; getResult
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1abbb830fa02bdac8614dfee99c902e464:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool getResult()

get final judge result



.. rubric:: Returns:

bool

.. index:: pair: function; traverse_qprog
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a8dabbdb29ac5c475dc6ded45fae27e4e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void traverse_qprog()

start traverse a quantum prog

