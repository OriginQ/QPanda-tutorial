.. index:: pair: class; QuantumError
.. _doxid-class_quantum_error:

class QuantumError
==================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NoiseModel.h>
	
	class QuantumError
	{
	public:
		// typedefs
	
		typedef std::vector<std::vector<size_t>> :target:`noise_qubits_t<doxid-class_quantum_error_1a6d07618457b15c65b2b60aa356ac6426>`;

		// construction
	
		:target:`QuantumError<doxid-class_quantum_error_1af926d059f13e50fc0e7bcb051eea674f>`();
	
		:target:`QuantumError<doxid-class_quantum_error_1ae8347cece72fdff85edc2c4c9a0f055a>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			double prob,
			size_t qubit_num
			);

		// methods
	
		void :target:`set_noise<doxid-class_quantum_error_1a8d695519ea5d5ec8e4b66bfb5e94e934>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			double prob,
			size_t qubit_num
			);
	
		void :target:`set_noise<doxid-class_quantum_error_1a497dbe6068c6887dad45c35d1f1694c8>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			double T1,
			double T2,
			double t_gate,
			size_t qubit_num
			);
	
		void :target:`set_noise<doxid-class_quantum_error_1a346541043c4cc93f8a42a0d8b40cb4a9>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices,
			const std::vector<double>& probs,
			size_t qubit_num
			);
	
		void :target:`set_noise<doxid-class_quantum_error_1a2c139b36b91be866dca5a6f7e99ea23b>`(
			const :ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices,
			size_t qubit_num
			);
	
		void :target:`set_reset_error<doxid-class_quantum_error_1afce88e4d3c9daa6e6898c78b0a1d7596>`(
			double p0,
			double p1
			);
	
		void :target:`set_readout_error<doxid-class_quantum_error_1a5b868a71f15ae70e68ab157f0a80ec71>`(
			const std::vector<std::vector<double>>& probs_list,
			size_t qubit_num
			);
	
		bool :target:`sample_noise<doxid-class_quantum_error_1a285b51e236cda6ad40ef0e9e082bc357>`(
			:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`& model,
			:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise_ops,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& noise_qubits,
			:ref:`RandomEngine19937<doxid-class_random_engine19937>`& rng
			);
	
		bool :target:`sample_noise<doxid-class_quantum_error_1ab66f942257317c3ce8bc148d69bfbd70>`(
			:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& noise_ops,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& noise_qubits,
			:ref:`RandomEngine19937<doxid-class_random_engine19937>`& rng
			);
	
		bool :target:`sample_readout<doxid-class_quantum_error_1a01d3e4e40ed486db60c9d09377c865d8>`(std::vector<std::vector<double>>& readout);
		void :target:`set_qubit_num<doxid-class_quantum_error_1ae7a787542b1c3d8a14ca82ea4e6fe1aa>`(int num);
		int :target:`get_qubit_num<doxid-class_quantum_error_1a2988ee68c481ce145fcb3ce53d12d323>`() const;
		bool :target:`_optimize_ops<doxid-class_quantum_error_1afcb8efe0ba9b8dc5cfe61b19bfdfde22>`(:ref:`NoiseOp<doxid-_noise_model_8h_1ab2a7591e4959d317081e50c00caad539>`& ops);
		:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>` :target:`get_noise_model<doxid-class_quantum_error_1a5d5d1f2d890d12e54d8ba3e92d4f6b65>`();
	};
