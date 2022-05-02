.. index:: pair: class; QPanda::QProgToDAG::QCirParamForDAG
.. _doxid-class_q_panda_1_1_q_prog_to_d_a_g_1_1_q_cir_param_for_d_a_g:

class QPanda::QProgToDAG::QCirParamForDAG
=========================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class QCirParamForDAG: public :ref:`QPanda::QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`
	{
	public:
		// fields
	
		:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& :target:`m_dag<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1_1_q_cir_param_for_d_a_g_1a0a37b226584e242ba659a4ce7a83848d>`;

		// construction
	
		:target:`QCirParamForDAG<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1_1_q_cir_param_for_d_a_g_1ad5f055184972553d2b13c328f88ab0cb>`(:ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& dag);

		// methods
	
		std::shared_ptr<:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`> :target:`clone<doxid-class_q_panda_1_1_q_prog_to_d_a_g_1_1_q_cir_param_for_d_a_g_1a8d9fc2196afccb2d04ae344a3ebc897c>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// fields
	
		bool :ref:`m_is_dagger<doxid-class_q_panda_1_1_q_circuit_param_1a5b815041da10bbf9cd84dd9888aa486c>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`m_control_qubits<doxid-class_q_panda_1_1_q_circuit_param_1a20df1b07df27232f0b4f3bfd904de0a7>`;

		// methods
	
		virtual std::shared_ptr<:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param>`> :ref:`clone<doxid-class_q_panda_1_1_q_circuit_param_1a225d03c234a07cd157e0bec0017dea64>`();
		void :ref:`append_control_qubits<doxid-class_q_panda_1_1_q_circuit_param_1ae6c97a2064895b2602ad64ed05436b1d>`(const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& ctrl_qubits);
		static :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`get_real_append_qubits<doxid-class_q_panda_1_1_q_circuit_param_1a71fe32cc5e7f1342dee18f887bda4dcd>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` append_qubits, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` target_qubits);

