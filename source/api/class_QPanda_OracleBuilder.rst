.. index:: pair: class; QPanda::OracleBuilder
.. _doxid-class_q_panda_1_1_oracle_builder:

template class QPanda::OracleBuilder
====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Oracle.h>
	
	template <class T>
	class OracleBuilder
	{
	public:
		// construction
	
		:target:`OracleBuilder<doxid-class_q_panda_1_1_oracle_builder_1a9db3909b4f5fcba7b7b4cc6cc800473c>`(
			const std::vector<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>& data_vec,
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` condition,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);

		// methods
	
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_oracle_circuit<doxid-class_q_panda_1_1_oracle_builder_1a1477d4b078a1945421a1bfedc791b54b>`(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` cir_mark);
		const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& :target:`get_index_qubits<doxid-class_q_panda_1_1_oracle_builder_1a0b08effbb8a2f3e56e6d30e1c72c1502>`();
		const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& :target:`get_oracle_qubits<doxid-class_q_panda_1_1_oracle_builder_1af687b5b52190660e7da6faa1b47ce52e>`();
		const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& :target:`get_ancilla_qubits<doxid-class_q_panda_1_1_oracle_builder_1a5e837605daaa1fa5ba6e2209f978163f>`();
	};
