.. index:: pair: class; QPanda::TransformByISWAP
.. _doxid-class_q_panda_1_1_transform_by_i_s_w_a_p:

class QPanda::TransformByISWAP
==============================

.. toctree::
	:hidden:

swap qubit location by ISWAP quantum gate


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TransformByISWAP: public :ref:`QPanda::TransformSwapAlg<doxid-class_q_panda_1_1_transform_swap_alg>`
	{
	public:
		// methods
	
		virtual void :target:`transform<doxid-class_q_panda_1_1_transform_by_i_s_w_a_p_1a6cfe75145b999a6ff9fbff7abd710605>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual int :target:`getSwapCost<doxid-class_q_panda_1_1_transform_by_i_s_w_a_p_1a9665a66cd2f962c9dc91613bcfdcb899>`();
		virtual int :target:`getFlipCost<doxid-class_q_panda_1_1_transform_by_i_s_w_a_p_1a039facb1a373820c88c22b83ad9c146d>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual void :ref:`transform<doxid-class_q_panda_1_1_transform_swap_alg_1ae17305f8578833ffc0baf31f209a7e7d>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog) = 0;
		virtual int :ref:`getSwapCost<doxid-class_q_panda_1_1_transform_swap_alg_1a653cfea033151cc84e23b759cea8cd82>`() = 0;
		virtual int :ref:`getFlipCost<doxid-class_q_panda_1_1_transform_swap_alg_1ad86f1adead101e377f3474352fe7dbf7>`() = 0;

