.. index:: pair: class; QPanda::AbstractDiffusionOperator
.. _doxid-class_q_panda_1_1_abstract_diffusion_operator:

class QPanda::AbstractDiffusionOperator
=======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <DiffusionCircuit.h>
	
	class AbstractDiffusionOperator
	{
	public:
		// methods
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_diffusion_circuit<doxid-class_q_panda_1_1_abstract_diffusion_operator_1a4cd81b226bcffcb5bc92ab3b0955d329>`(const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qvec) = 0;
	};

	// direct descendants

	class :ref:`DiffusionCirBuilder<doxid-class_q_panda_1_1_diffusion_cir_builder>`;
