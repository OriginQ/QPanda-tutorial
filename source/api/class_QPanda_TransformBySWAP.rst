.. index:: pair: class; QPanda::TransformBySWAP
.. _doxid-class_q_panda_1_1_transform_by_s_w_a_p:

class QPanda::TransformBySWAP
=============================

.. toctree::
	:hidden:

swap qubit location by SWAP quantum gate


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TransformBySWAP: public :ref:`QPanda::TransformSwapAlg<doxid-class_q_panda_1_1_transform_swap_alg>`
	{
	public:
		// methods
	
		virtual void :target:`transform<doxid-class_q_panda_1_1_transform_by_s_w_a_p_1a165f15488ff5ecd9595c93ee42ee9304>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual int :target:`getSwapCost<doxid-class_q_panda_1_1_transform_by_s_w_a_p_1a412a250076530bbf420b5bcf43542df6>`();
		virtual int :target:`getFlipCost<doxid-class_q_panda_1_1_transform_by_s_w_a_p_1a7659fa66d318e12e735271c77ee08e16>`();
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

