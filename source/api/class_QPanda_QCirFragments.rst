.. index:: pair: class; QPanda::QCirFragments
.. _doxid-class_q_panda_1_1_q_cir_fragments:

class QPanda::QCirFragments
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CutQC.h>
	
	class QCirFragments
	{
	public:
		// fields
	
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`m_cir<doxid-class_q_panda_1_1_q_cir_fragments_1aada3890e52b947d4a851f0bfc44ff887>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`m_prep_qubits<doxid-class_q_panda_1_1_q_cir_fragments_1a1fab8c1b7d9be8876d0f37ad72b2f767>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`m_meas_qubits<doxid-class_q_panda_1_1_q_cir_fragments_1a5d80eec90ea39cd8065aad6383d321b5>`;
		std::vector<:ref:`FragmentResult<doxid-class_q_panda_1_1_fragment_result>`> :target:`m_fragment_results<doxid-class_q_panda_1_1_q_cir_fragments_1a5efe06c215a8559af418c050ab7d9ea6>`;

		// construction
	
		:target:`QCirFragments<doxid-class_q_panda_1_1_q_cir_fragments_1a95bdd8a868ef17887357309565a69664>`(const :ref:`SubCircuit<doxid-struct_q_panda_1_1_sub_circuit>`& frag);
	};
