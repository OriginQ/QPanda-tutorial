.. index:: pair: class; QPanda::QPEAlg
.. _doxid-class_q_panda_1_1_q_p_e_alg:

class QPanda::QPEAlg
====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPE.h>
	
	class QPEAlg
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`)> :target:`generate_cir_U<doxid-class_q_panda_1_1_q_p_e_alg_1a15ab376162796c62b23f8874a15088e1>`;

		// construction
	
		:target:`QPEAlg<doxid-class_q_panda_1_1_q_p_e_alg_1a4de6acd251810cb4fd4489ddcb8ff357>`(
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& control_qubits,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& target_qubits,
			const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix
			);
	
		:target:`QPEAlg<doxid-class_q_panda_1_1_q_p_e_alg_1a47d6fc975b4947a11a256b7c999da00c>`(
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& control_qubits,
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& target_qubits,
			:ref:`generate_cir_U<doxid-class_q_panda_1_1_q_p_e_alg_1a15ab376162796c62b23f8874a15088e1>` cir_fun
			);

		// methods
	
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`QPE<doxid-class_q_panda_1_1_q_p_e_alg_1a5edf7ae1095002c4da7c8cb6f1a4f4a1>`();
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`quantum_eigenvalue_estimation<doxid-class_q_panda_1_1_q_p_e_alg_1ae1e846b3bb6f515eded88a8b1f2f2ad5>`();
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`get_qpe_circuit<doxid-class_q_panda_1_1_q_p_e_alg_1acddeb9cadaef5b56a57ff39f184e919e>`();
	};
