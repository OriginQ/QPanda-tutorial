.. index:: pair: group; QuantumMachine
.. _doxid-group___quantum_machine:

QuantumMachine
==============

.. toctree::
	:hidden:

	class_QPanda_CBit.rst
	class_QPanda_CBitFactory.rst
	class_QPanda_CBitFactoryHelper.rst
	class_QPanda_CMem.rst
	class_QPanda_CMemFactory.rst
	class_QPanda_CMemFactoryHelper.rst
	class_QPanda_OriginCBit.rst
	class_QPanda_OriginCMem.rst
	class_QPanda_OriginPhysicalQubit.rst
	class_QPanda_OriginQMachineStatus.rst
	class_QPanda_OriginQResult.rst
	class_QPanda_OriginQubit.rst
	class_QPanda_OriginQubitPool.rst
	class_QPanda_OriginQubitPoolv2.rst
	class_QPanda_PartialAmplitudeQVM.rst
	class_QPanda_PhysicalQubit.rst
	class_QPanda_PhysicalQubitFactory.rst
	class_QPanda_PhysicalQubitFactoryHelper.rst
	class_QPanda_QMachineStatusFactory.rst
	class_QPanda_QMachineTypeTarnfrom.rst
	class_QPanda_QProgExecution.rst
	class_QPanda_QResult.rst
	class_QPanda_QResultFactory.rst
	class_QPanda_QResultFactoryHelper.rst
	class_QPanda_QVec.rst
	class_QPanda_QuantumMachine.rst
	class_QPanda_QuantumMachineFactory.rst
	class_QPanda_QuantumMachineFactoryHelper.rst
	class_QPanda_Qubit.rst
	class_QPanda_QubitFactory.rst
	class_QPanda_QubitFactoryHelper.rst
	class_QPanda_QubitPool.rst
	class_QPanda_QubitPoolFactory.rst
	class_QPanda_QubitPoolFactoryHelper.rst
	class_QPanda_QubitReference.rst
	class_QPanda_QubitReferenceInterface.rst
	class_QPanda_SingleAmplitudeQVM.rst

Overview
~~~~~~~~

QPanda2 quantum virtual machine. :ref:`More...<details-group___quantum_machine>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// classes

	class :ref:`QPanda::CBit<doxid-class_q_panda_1_1_c_bit>`;
	class :ref:`QPanda::CBitFactory<doxid-class_q_panda_1_1_c_bit_factory>`;
	class :ref:`QPanda::CBitFactoryHelper<doxid-class_q_panda_1_1_c_bit_factory_helper>`;
	class :ref:`QPanda::CMem<doxid-class_q_panda_1_1_c_mem>`;
	class :ref:`QPanda::CMemFactory<doxid-class_q_panda_1_1_c_mem_factory>`;
	class :ref:`QPanda::CMemFactoryHelper<doxid-class_q_panda_1_1_c_mem_factory_helper>`;
	class :ref:`QPanda::OriginCBit<doxid-class_q_panda_1_1_origin_c_bit>`;
	class :ref:`QPanda::OriginCMem<doxid-class_q_panda_1_1_origin_c_mem>`;
	class :ref:`QPanda::OriginPhysicalQubit<doxid-class_q_panda_1_1_origin_physical_qubit>`;
	class :ref:`QPanda::OriginQMachineStatus<doxid-class_q_panda_1_1_origin_q_machine_status>`;
	class :ref:`QPanda::OriginQResult<doxid-class_q_panda_1_1_origin_q_result>`;
	class :ref:`QPanda::OriginQubit<doxid-class_q_panda_1_1_origin_qubit>`;
	class :ref:`QPanda::OriginQubitPool<doxid-class_q_panda_1_1_origin_qubit_pool>`;
	class :ref:`QPanda::OriginQubitPoolv2<doxid-class_q_panda_1_1_origin_qubit_poolv2>`;
	class :ref:`QPanda::PartialAmplitudeQVM<doxid-class_q_panda_1_1_partial_amplitude_q_v_m>`;
	class :ref:`QPanda::PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`;
	class :ref:`QPanda::PhysicalQubitFactory<doxid-class_q_panda_1_1_physical_qubit_factory>`;
	class :ref:`QPanda::PhysicalQubitFactoryHelper<doxid-class_q_panda_1_1_physical_qubit_factory_helper>`;
	class :ref:`QPanda::QMachineStatusFactory<doxid-class_q_panda_1_1_q_machine_status_factory>`;
	class :ref:`QPanda::QMachineTypeTarnfrom<doxid-class_q_panda_1_1_q_machine_type_tarnfrom>`;
	class :ref:`QPanda::QProgExecution<doxid-class_q_panda_1_1_q_prog_execution>`;
	class :ref:`QPanda::QResult<doxid-class_q_panda_1_1_q_result>`;
	class :ref:`QPanda::QResultFactory<doxid-class_q_panda_1_1_q_result_factory>`;
	class :ref:`QPanda::QResultFactoryHelper<doxid-class_q_panda_1_1_q_result_factory_helper>`;
	class :ref:`QPanda::QVec<doxid-class_q_panda_1_1_q_vec>`;
	class :ref:`QPanda::QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`;
	class :ref:`QPanda::QuantumMachineFactory<doxid-class_q_panda_1_1_quantum_machine_factory>`;
	class :ref:`QPanda::QuantumMachineFactoryHelper<doxid-class_q_panda_1_1_quantum_machine_factory_helper>`;
	class :ref:`QPanda::Qubit<doxid-class_q_panda_1_1_qubit>`;
	class :ref:`QPanda::QubitFactory<doxid-class_q_panda_1_1_qubit_factory>`;
	class :ref:`QPanda::QubitFactoryHelper<doxid-class_q_panda_1_1_qubit_factory_helper>`;
	class :ref:`QPanda::QubitPool<doxid-class_q_panda_1_1_qubit_pool>`;
	class :ref:`QPanda::QubitPoolFactory<doxid-class_q_panda_1_1_qubit_pool_factory>`;
	class :ref:`QPanda::QubitPoolFactoryHelper<doxid-class_q_panda_1_1_qubit_pool_factory_helper>`;
	class :ref:`QPanda::QubitReference<doxid-class_q_panda_1_1_qubit_reference>`;
	class :ref:`QPanda::QubitReferenceInterface<doxid-class_q_panda_1_1_qubit_reference_interface>`;
	class :ref:`QPanda::SingleAmplitudeQVM<doxid-class_q_panda_1_1_single_amplitude_q_v_m>`;

	// global functions

	std::string :ref:`QPanda::qProgToBinary<doxid-group___quantum_machine_1gab866832e6095f21fe98f8ec7cae1bfab>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*);
	void :ref:`QPanda::execute_qprog<doxid-group___quantum_machine_1ga3c31a727dcc23d3c9a918a4ec8441522>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu, :ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param);

.. _details-group___quantum_machine:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPanda2 quantum virtual machine.

Global Functions
----------------

.. index:: pair: function; qProgToBinary
.. _doxid-group___quantum_machine_1gab866832e6095f21fe98f8ec7cae1bfab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string QPanda::qProgToBinary(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`, :ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*)

Quamtum program tramsform to binary data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit num

	*
		- size_t

		- cbit num

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- the reference to a quantum program



.. rubric:: Returns:

std::string binary data

.. index:: pair: function; execute_qprog
.. _doxid-group___quantum_machine_1ga3c31a727dcc23d3c9a918a4ec8441522:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void QPanda::execute_qprog(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QPUImpl<doxid-class_q_p_u_impl>`* qpu, :ref:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config>`& param)

execute qprog



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

		- quantum program

	*
		- QPUImpl\*

		- 

	*
		- TraversalConfig&

		- traversal configuration



.. rubric:: Returns:

