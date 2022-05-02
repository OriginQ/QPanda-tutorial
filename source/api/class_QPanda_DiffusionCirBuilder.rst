.. index:: pair: class; QPanda::DiffusionCirBuilder
.. _doxid-class_q_panda_1_1_diffusion_cir_builder:

class QPanda::DiffusionCirBuilder
=================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <DiffusionCircuit.h>
	
	class DiffusionCirBuilder: public :ref:`QPanda::AbstractDiffusionOperator<doxid-class_q_panda_1_1_abstract_diffusion_operator>`
	{
	public:
		// methods
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_diffusion_circuit<doxid-class_q_panda_1_1_diffusion_cir_builder_1a209a02d0883c3cdda5af1588c0ec0c87>`(const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qvec);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`build_diffusion_circuit<doxid-class_q_panda_1_1_abstract_diffusion_operator_1a4cd81b226bcffcb5bc92ab3b0955d329>`(const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qvec) = 0;

