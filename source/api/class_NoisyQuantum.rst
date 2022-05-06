.. index:: pair: class; NoisyQuantum
.. _doxid-class_noisy_quantum:

class NoisyQuantum
==================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NoiseModel.h>
	
	class NoisyQuantum
	{
	public:
		// typedefs
	
		typedef std::map<std::string, size_t> :target:`qubit_quantum_error_map_t<doxid-class_noisy_quantum_1a3891bb9abfc083aecb16493ff172db69>`;
		typedef std::map<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`, :ref:`qubit_quantum_error_map_t<doxid-class_noisy_quantum_1a3891bb9abfc083aecb16493ff172db69>`> :target:`gate_noisy_map_t<doxid-class_noisy_quantum_1a7e38b6e36e7a2f552b2ffc03d63b45c7>`;

		// methods
	
		bool :target:`sample_noisy_op<doxid-class_noisy_quantum_1a0c5b2a9d4ea8fb3d9fb2b11362795ee1>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` type,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qns,
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& ops,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& effect_qubits,
			:ref:`RandomEngine19937<doxid-class_random_engine19937>`& rng
			);
	
		bool :target:`sample_noisy_op<doxid-class_noisy_quantum_1ad8bb500c7e0cd51d7c869bf04a2493a0>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` type,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qns,
			:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& ops,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& effect_qubits,
			:ref:`RandomEngine19937<doxid-class_random_engine19937>`& rng
			);
	
		bool :target:`sample_noisy_op<doxid-class_noisy_quantum_1a4e79a34a102201fe403929cfd2cf87d3>`(
			size_t qn,
			std::vector<std::vector<double>>& readout,
			:ref:`RandomEngine19937<doxid-class_random_engine19937>`& rng
			);
	
		void :target:`add_quamtum_error<doxid-class_noisy_quantum_1ae0731bf5a6ed1df4e9328ab6bfdf32b0>`(
			:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` type,
			const :ref:`QuantumError<doxid-class_quantum_error>`& quantum_error,
			const :ref:`QuantumError::noise_qubits_t<doxid-class_quantum_error_1a6d07618457b15c65b2b60aa356ac6426>`& noise_qubits = {}
			);
	};
