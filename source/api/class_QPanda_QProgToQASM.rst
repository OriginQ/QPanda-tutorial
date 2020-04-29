.. index:: pair: class; QPanda::QProgToQASM
.. _doxid-class_q_panda_1_1_q_prog_to_q_a_s_m:

class QPanda::QProgToQASM
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum Prog Transform To QASM instruction sets. :ref:`More...<details-class_q_panda_1_1_q_prog_to_q_a_s_m>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgToQASM.h>
	
	class QProgToQASM: public :ref:`QPanda::TraversalInterface<doxid-class_q_panda_1_1_traversal_interface>`
	{
	public:
		// construction
	
		:target:`QProgToQASM<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1a77d72b71c1d25b7117490f9d2f424e00>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* quantum_machine,
			:ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` ibmBackend = :ref:`IBMQ_QASM_SIMULATOR<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8ca09728e1eb958bbe0ec92174a7ce111cd>`
			);

		// methods
	
		virtual std::string :ref:`getInsturctions<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1aa111eace9acba3aed04690aafcf217f4>`();
		virtual void :ref:`transform<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1ad71a1b6bcb8e4d2c9f63a850a9a7f5cb>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1a937fc740d01e4fc10e2559a57f1c3dbf>`(
			std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1a8d076073f726b087faa25672bdd606da>`(
			std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1ae0c672ed40329e1aac8653625c9d84a6>`(
			std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1a0e20bd9cc8438ca00dc781109af2f8f5>`(
			std::shared_ptr<:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1afa9f7a6f0fa1cdd117c2261e68d5db18>`(
			std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1a2e9560de47e679755fc8e43f92e5e95d>`(
			std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		virtual void :target:`execute<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1a2e5f5ffb53105c91d88ac4c6ebfea7b5>`(
			std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> cur_node,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			bool&
			);
	
		static std::string :target:`getIBMQBackendName<doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1a59cdc01f5dd5ec938916f230eef5f64f>`(:ref:`IBMQBackends<doxid-namespace_q_panda_1a13af700f152a6c7260fee48f68442b8c>` typeNum);
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

.. _details-class_q_panda_1_1_q_prog_to_q_a_s_m:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum Prog Transform To QASM instruction sets.

Methods
-------

.. index:: pair: function; getInsturctions
.. _doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1aa111eace9acba3aed04690aafcf217f4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getInsturctions()

get QASM insturction set



.. rubric:: Returns:

std::string

.. index:: pair: function; transform
.. _doxid-class_q_panda_1_1_q_prog_to_q_a_s_m_1ad71a1b6bcb8e4d2c9f63a850a9a7f5cb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void transform(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&)

Transform Quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- quantum program



.. rubric:: Returns:

void

