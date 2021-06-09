.. index:: pair: class; QPanda::JudgeTwoNodeIterIsSwappable
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable:

class QPanda::JudgeTwoNodeIterIsSwappable
=========================================

.. toctree::
	:hidden:

	struct_QPanda_JudgeTwoNodeIterIsSwappable_NodeInCircuitInfo.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_AbstractJudgeStatueInterface.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_CanNotBeExchange.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_CoubleBeExchange.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_OnFoundAllNodes.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_OnInitStatue.rst
	class_QPanda_JudgeTwoNodeIterIsSwappable_OnJudgeMatrix.rst
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
		// structs
	
		struct :ref:`NodeInCircuitInfo<doxid-struct_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_node_in_circuit_info>`;

		// classes
	
		class :ref:`AbstractJudgeStatueInterface<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_abstract_judge_statue_interface>`;
		class :ref:`CanNotBeExchange<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_can_not_be_exchange>`;
		class :ref:`CoubleBeExchange<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_couble_be_exchange>`;
		class :ref:`OnFoundAllNodes<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_found_all_nodes>`;
		class :ref:`OnInitStatue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_init_statue>`;
		class :ref:`OnJudgeMatrix<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_judge_matrix>`;
		class :ref:`OnPickUpNode<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_pick_up_node>`;

		// construction
	
		:ref:`JudgeTwoNodeIterIsSwappable<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a541e11f5ad59758919fdd8ff285983d3>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_1, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_2);

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
	
		bool :ref:`get_result<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a1893f3ac9aafcd0365bc53f295436f3c>`();
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1aa4a16728faeea9bffc647a55209e4bd1>`();
		bool :ref:`judge_node_type<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a54d42c0436d969f2e19d86ad773fd91b>`();
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
	
		virtual void :ref:`traverse_qprog<doxid-class_q_panda_1_1_traverse_by_node_iter_1ab298ca4e8835cb14518f8b83c87d6287>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);

.. _details-class_q_panda_1_1_judge_two_node_iter_is_swappable:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Judge two node is swappable.

Construction
------------

.. index:: pair: function; JudgeTwoNodeIterIsSwappable
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a541e11f5ad59758919fdd8ff285983d3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	JudgeTwoNodeIterIsSwappable(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_1, :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& nodeItr_2)

Constructor of :ref:`JudgeTwoNodeIterIsSwappable <doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable>`.

Methods
-------

.. index:: pair: function; get_result
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a1893f3ac9aafcd0365bc53f295436f3c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool get_result()

get final judge result



.. rubric:: Returns:

bool

.. index:: pair: function; traverse_qprog
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1aa4a16728faeea9bffc647a55209e4bd1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void traverse_qprog()

start traverse a quantum prog

.. index:: pair: function; judge_node_type
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1a54d42c0436d969f2e19d86ad773fd91b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool judge_node_type()

judge the input two node type



.. rubric:: Returns:

if any input node is unswappable type, return false, else return true.

