.. index:: pair: class; QPanda::NonKarusError
.. _doxid-class_q_panda_1_1_non_karus_error:

class QPanda::NonKarusError
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NoiseSimulator.h>
	
	class NonKarusError
	{
	public:
		// methods
	
		bool :target:`has_non_karus_error<doxid-class_q_panda_1_1_non_karus_error_1ad3e7d848f990d7afb300c9d956b0eead>`();
		void :target:`set_rotation_error<doxid-class_q_panda_1_1_non_karus_error_1a9498e968991f239fcb7a9862448bee44>`(double param);
		double :target:`get_rotation_error<doxid-class_q_panda_1_1_non_karus_error_1a7d1bc80ee68b808a266281944ac920e0>`();
	
		void :target:`set_reset_error<doxid-class_q_panda_1_1_non_karus_error_1a1279815dc249e7fcdfc7c95aa5cfac99>`(
			double p0_param,
			double p1_param
			);
	
		double :target:`get_reset_p0_error<doxid-class_q_panda_1_1_non_karus_error_1a32672551d8e98457dc0d75e35775329e>`();
		double :target:`get_reset_p1_error<doxid-class_q_panda_1_1_non_karus_error_1a08ce6727040017a00281c017eb412731>`();
		bool :target:`has_measure_qubit<doxid-class_q_panda_1_1_non_karus_error_1aa4f9cb9a6a711dd7213912c00943b827>`(size_t qubit);
		void :target:`set_measure_qubit<doxid-class_q_panda_1_1_non_karus_error_1a2bfcdc1b57ab957228f04c1306b8555d>`(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits);
		bool :target:`has_measure_error<doxid-class_q_panda_1_1_non_karus_error_1aa090da14421d88b96336afcc5e796dd8>`();
	
		void :target:`set_measure_error<doxid-class_q_panda_1_1_non_karus_error_1aed2aaaf5009eba356cd1dd52820199f3>`(
			int qubit,
			std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& karus_matrices
			);
	
		void :target:`get_measure_error<doxid-class_q_panda_1_1_non_karus_error_1acd76ece25058b985ed9c53f7d1de7776>`(
			int qubit,
			std::vector<:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`>& karus_matrices
			);
	
		bool :target:`has_readout_error<doxid-class_q_panda_1_1_non_karus_error_1a654f71b3c32112b0da900a539f3cae2c>`();
	
		bool :target:`get_readout_result<doxid-class_q_panda_1_1_non_karus_error_1a3bcbb2a6abfe9eeded9e55b36aa35f7c>`(
			bool result,
			size_t qubit
			);
	
		void :target:`set_readout_error<doxid-class_q_panda_1_1_non_karus_error_1a4b6e5ba3184087899221066bdf563e27>`(
			const std::vector<std::vector<double>>& readout_probabilities,
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qvec
			);
	};
