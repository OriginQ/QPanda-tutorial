.. index:: pair: class; QPanda::TransformByCZ
.. _doxid-class_q_panda_1_1_transform_by_c_z:

class QPanda::TransformByCZ
===========================

.. toctree::
	:hidden:

swap qubit location by CZ quantum gate


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TransformByCZ: public :ref:`QPanda::TransformSwapAlg<doxid-class_q_panda_1_1_transform_swap_alg>`
	{
	public:
		// methods
	
		virtual void :target:`transform<doxid-class_q_panda_1_1_transform_by_c_z_1af40d24451c52a7cd27cc4200328a50eb>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual int :target:`getSwapCost<doxid-class_q_panda_1_1_transform_by_c_z_1a930e4ef217571780fe30a6c0507784fe>`();
		virtual int :target:`getFlipCost<doxid-class_q_panda_1_1_transform_by_c_z_1af3a6cc2b5c0aafad43d131a9baec6159>`();
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

