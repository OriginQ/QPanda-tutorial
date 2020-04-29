.. index:: pair: class; QPanda::TransformSwapAlg
.. _doxid-class_q_panda_1_1_transform_swap_alg:

class QPanda::TransformSwapAlg
==============================

.. toctree::
	:hidden:

swap qubit location algorithm abstract class


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TransformSwapAlg
	{
	public:
		// methods
	
		virtual void :target:`transform<doxid-class_q_panda_1_1_transform_swap_alg_1ae17305f8578833ffc0baf31f209a7e7d>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			) = 0;
	
		virtual int :target:`getSwapCost<doxid-class_q_panda_1_1_transform_swap_alg_1a653cfea033151cc84e23b759cea8cd82>`() = 0;
		virtual int :target:`getFlipCost<doxid-class_q_panda_1_1_transform_swap_alg_1ad86f1adead101e377f3474352fe7dbf7>`() = 0;
	};

	// direct descendants

	class :ref:`TransformByCNOT<doxid-class_q_panda_1_1_transform_by_c_n_o_t>`;
	class :ref:`TransformByCZ<doxid-class_q_panda_1_1_transform_by_c_z>`;
	class :ref:`TransformByISWAP<doxid-class_q_panda_1_1_transform_by_i_s_w_a_p>`;
	class :ref:`TransformBySWAP<doxid-class_q_panda_1_1_transform_by_s_w_a_p>`;
