.. index:: pair: class; QPanda::SearchCondition
.. _doxid-class_q_panda_1_1_search_condition:

template class QPanda::SearchCondition
======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <SearchCondition.h>
	
	template <class T>
	class SearchCondition
	{
	public:
		// construction
	
		:target:`SearchCondition<doxid-class_q_panda_1_1_search_condition_1a8453fb26e40b529923b75620dd2398ec>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm,
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` condition
			);

		// methods
	
		void :target:`load_search_condition<doxid-class_q_panda_1_1_search_condition_1ae5d3c1dbb4c81ff7ca8a426b2201813e>`();
	
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_to_circuit<doxid-class_q_panda_1_1_search_condition_1ae0b46b0842e70ede44ce117197ff0cb4>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` oracle_qubits,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` ancilla_qubits,
			const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& mini_data,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` cir_mark
			);
	};
