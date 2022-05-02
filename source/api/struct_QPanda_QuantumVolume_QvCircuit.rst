.. index:: pair: struct; QPanda::QuantumVolume::QvCircuit
.. _doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit:

struct QPanda::QuantumVolume::QvCircuit
=======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct QvCircuit
	{
		// fields
	
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`cir<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a5edefbbb0d8fde923b15652293a03fc0>`;
		int :target:`depth<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a25462914eac6027cb12d8ab9347c0cfb>`;
		int :target:`trial<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a45f6029c6c0125c37935a4df944664bb>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`qv<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a29361da6becb1e4da155b8f0f3882236>`;
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :target:`cv<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a0d7ab8f07d48794d25d0479ce103cb3a>`;
		:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`result<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a1bc8d89b7d7296276887439a4d0dcaad>`;
		float :target:`heavy_output<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a5e497e7b1f8f101d4d503995e23cd64f>`;
		int :target:`shots<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a41c0b2bbb8c9452b104ead1e7505eed1>`;
		int :target:`qvm_type<doxid-struct_q_panda_1_1_quantum_volume_1_1_qv_circuit_1a41ce5f517452d21696d49f2d3c771f66>`;
	};
