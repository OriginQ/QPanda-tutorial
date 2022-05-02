.. index:: pair: class; QPanda::SearchSpace
.. _doxid-class_q_panda_1_1_search_space:

template class QPanda::SearchSpace
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <SearchSpace.h>
	
	template <class T>
	class SearchSpace
	{
	public:
		// construction
	
		:target:`SearchSpace<doxid-class_q_panda_1_1_search_space_1a480cd439ae790f75e4b1895924577325>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm,
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>` condition
			);

		// methods
	
		const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& :target:`get_index_qubits<doxid-class_q_panda_1_1_search_space_1a0e35fd158c8efdbe03c1cb886acdb19e>`();
		const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& :target:`get_data_qubits<doxid-class_q_panda_1_1_search_space_1aee0e9d1d084ff00cb49075bf365cffa0>`();
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_to_circuit<doxid-class_q_panda_1_1_search_space_1aa409c7a757f697dea86bac2c4753d8ea>`(const std::vector<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>& data_vec);
		const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& :target:`get_mini_data<doxid-class_q_panda_1_1_search_space_1ab3d79392847f6e60a29a5d564e20adfb>`();
	};
