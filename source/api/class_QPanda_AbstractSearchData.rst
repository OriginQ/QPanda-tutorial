.. index:: pair: class; QPanda::AbstractSearchData
.. _doxid-class_q_panda_1_1_abstract_search_data:

class QPanda::AbstractSearchData
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <SearchDataType.h>
	
	class AbstractSearchData
	{
	public:
		// methods
	
		virtual bool :target:`operator <<doxid-class_q_panda_1_1_abstract_search_data_1ac8be608f843f97befcafb8703e108e2e>` (const AbstractSearchData& other) const = 0;
		virtual bool :target:`operator <=<doxid-class_q_panda_1_1_abstract_search_data_1a7810978c9562e0b3d432fcef7603dd73>` (const AbstractSearchData& other) const = 0;
		virtual bool :target:`operator ><doxid-class_q_panda_1_1_abstract_search_data_1a3a64b342f0a64cb4010dfeadb0330250>` (const AbstractSearchData& other) const = 0;
		virtual bool :target:`operator >=<doxid-class_q_panda_1_1_abstract_search_data_1abf75efa070629e9e3af09006c2610b07>` (const AbstractSearchData& other) const = 0;
		virtual bool :target:`operator ==<doxid-class_q_panda_1_1_abstract_search_data_1aeeb1bd1f0c8816827ac629ba4018de96>` (const AbstractSearchData&& other) const = 0;
		virtual AbstractSearchData& :target:`operator -<doxid-class_q_panda_1_1_abstract_search_data_1a23d2332f7b25112ab26c44e4da2959d1>` (const AbstractSearchData& other) = 0;
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_to_circuit<doxid-class_q_panda_1_1_abstract_search_data_1a3c6c99e74388fa49fe4c74be1e24ad90>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& used_qubits,
			size_t use_qubit_cnt,
			const AbstractSearchData& mini_data
			) const = 0;
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_to_condition_circuit<doxid-class_q_panda_1_1_abstract_search_data_1a5bd409c893b41e165312cc65b9951ffd>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& used_qubits,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` cir_mark,
			const AbstractSearchData& mini_data
			) = 0;
	
		virtual size_t :target:`check_max_need_qubits<doxid-class_q_panda_1_1_abstract_search_data_1ace19ca4185587c60bd0da34f47ade3f2>`() = 0;
		virtual AbstractSearchData& :target:`set_val<doxid-class_q_panda_1_1_abstract_search_data_1a37c2c5a1eee89450a731862cda15049d>`(const char* p_val) = 0;
	};

	// direct descendants

	class :ref:`SearchDataByUInt<doxid-class_q_panda_1_1_search_data_by_u_int>`;
