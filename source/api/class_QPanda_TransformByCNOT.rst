.. index:: pair: class; QPanda::TransformByCNOT
.. _doxid-class_q_panda_1_1_transform_by_c_n_o_t:

class QPanda::TransformByCNOT
=============================

.. toctree::
	:hidden:

swap qubit location by CNOT quantum gate


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TransformByCNOT: public :ref:`QPanda::TransformSwapAlg<doxid-class_q_panda_1_1_transform_swap_alg>`
	{
	public:
		// methods
	
		virtual void :target:`transform<doxid-class_q_panda_1_1_transform_by_c_n_o_t_1a73316547664a45b6d858a87327b1180d>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* control_qubit,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* target_qubit,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		virtual int :target:`getSwapCost<doxid-class_q_panda_1_1_transform_by_c_n_o_t_1a084586175eaf166b13e7f125f1e0ddb1>`();
		virtual int :target:`getFlipCost<doxid-class_q_panda_1_1_transform_by_c_n_o_t_1a5d730cb2de7c5ea3e6fee8aa0b152024>`();
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

