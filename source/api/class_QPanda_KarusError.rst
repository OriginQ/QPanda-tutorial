.. index:: pair: class; QPanda::KarusError
.. _doxid-class_q_panda_1_1_karus_error:

class QPanda::KarusError
========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NoiseSimulator.h>
	
	class KarusError
	{
	public:
		// construction
	
		:target:`KarusError<doxid-class_q_panda_1_1_karus_error_1a13980fe3f6924d96de0a345c09897da1>`();
		:target:`KarusError<doxid-class_q_panda_1_1_karus_error_1ab73f214b67619e581cd5e9c6a29e51f2>`(const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>&);
	
		:target:`KarusError<doxid-class_q_panda_1_1_karus_error_1a41cb2f958800ba322c050535d9227885>`(
			const std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>&,
			const std::vector<double>&
			);

		// methods
	
		bool :target:`has_karus_error<doxid-class_q_panda_1_1_karus_error_1ae7b03e74028b000745486446898891a9>`();
		void :target:`set_unitary_probs<doxid-class_q_panda_1_1_karus_error_1a24758a2efac9856e760913fd7f357c95>`(std::vector<double>& probs_vec);
		void :target:`get_unitary_probs<doxid-class_q_panda_1_1_karus_error_1a5cb40cb905ea0f6893b0600cc2aeb03b>`(std::vector<double>& probs_vec) const;
		void :target:`set_unitary_matrices<doxid-class_q_panda_1_1_karus_error_1af545ccb87c2ed97aa54e1d9c21f62978>`(std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices);
		void :target:`get_unitary_matrices<doxid-class_q_panda_1_1_karus_error_1ab8103a9923302acb950220c3a5311b6f>`(std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& unitary_matrices) const;
		void :target:`set_karus_matrices<doxid-class_q_panda_1_1_karus_error_1a3eb6fd16a6f2edb94646b4923cfc4c6f>`(std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& karus_matrices);
		void :target:`get_karus_matrices<doxid-class_q_panda_1_1_karus_error_1a27c5a583014f5043b7292f8bbc8da44b>`(std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& karus_matrices) const;
		KarusError :target:`tensor<doxid-class_q_panda_1_1_karus_error_1aba3f227dbac94344d5cc6b90a533776c>`(const KarusError& karus_error);
		KarusError :target:`expand<doxid-class_q_panda_1_1_karus_error_1a457cb436e2a2040a45c4daec5e02f757>`(const KarusError& karus_error);
		KarusError :target:`compose<doxid-class_q_panda_1_1_karus_error_1ad9d12bcad9002b6ff0bd0d083337feda>`(const KarusError& karus_error);
		size_t :target:`get_qubit_num<doxid-class_q_panda_1_1_karus_error_1ac4a90ec0272f28769a4712efb5388f59>`() const;
		:ref:`KarusErrorType<doxid-namespace_q_panda_1a38ded6ef39c4ae9be23de6361ca5bff5>` :target:`get_karus_error_type<doxid-class_q_panda_1_1_karus_error_1a67e5917887188572092ead906e2094a0>`();
	};
