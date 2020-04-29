.. index:: pair: class; QPanda::IdealMachineInterface
.. _doxid-class_q_panda_1_1_ideal_machine_interface:

class QPanda::IdealMachineInterface
===================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMachineInterface.h>
	
	class IdealMachineInterface
	{
	public:
		// methods
	
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`PMeasure_no_index<doxid-class_q_panda_1_1_ideal_machine_interface_1aa1908bd072b61280a985f26369d574e5>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector) = 0;
	
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`getProbTupleList<doxid-class_q_panda_1_1_ideal_machine_interface_1a0d5e3fdae0eebcf046081eb1557f418c>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			) = 0;
	
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`getProbList<doxid-class_q_panda_1_1_ideal_machine_interface_1a4d3b351174020e7d36fdc6b3af805052>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			) = 0;
	
		virtual :ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :target:`getProbDict<doxid-class_q_panda_1_1_ideal_machine_interface_1a10941c69eb843f04949bff4ac272751f>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			) = 0;
	
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`probRunTupleList<doxid-class_q_panda_1_1_ideal_machine_interface_1ad54eae1ebb20721628bdfebfd0cd732e>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			) = 0;
	
		virtual :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>` :target:`probRunList<doxid-class_q_panda_1_1_ideal_machine_interface_1a9cc21ede35f892116f87e6697f2f4034>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			) = 0;
	
		virtual :ref:`prob_dict<doxid-_q_panda_namespace_8h_1a0b8487bf3711ffe87477dd745ab418dd>` :target:`probRunDict<doxid-class_q_panda_1_1_ideal_machine_interface_1a26484905dcc5faafa905c30246c7231f>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			int
			) = 0;
	
		virtual std::map<std::string, size_t> :target:`quickMeasure<doxid-class_q_panda_1_1_ideal_machine_interface_1adb5cf9a4ee37f1d74dc38ceee26a5033>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`,
			size_t
			) = 0;
	
		virtual :ref:`prob_tuple<doxid-_q_panda_namespace_8h_1ab92b79b1b1a44ee773053c13c7fb5344>` :target:`PMeasure<doxid-class_q_panda_1_1_ideal_machine_interface_1ad0519fea1275272071948226776df69b>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qubit_vector,
			int select_max
			) = 0;
	
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`getQStat<doxid-class_q_panda_1_1_ideal_machine_interface_1ac83e01310fc24e27ce7b1c6fac41138b>`() = 0;
	};

	// direct descendants

	class :ref:`IdealQVM<doxid-class_q_panda_1_1_ideal_q_v_m>`;
