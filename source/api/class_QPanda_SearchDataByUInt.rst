.. index:: pair: class; QPanda::SearchDataByUInt
.. _doxid-class_q_panda_1_1_search_data_by_u_int:

class QPanda::SearchDataByUInt
==============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <SearchDataType.h>
	
	class SearchDataByUInt: public :ref:`QPanda::AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`
	{
	public:
		// construction
	
		:target:`SearchDataByUInt<doxid-class_q_panda_1_1_search_data_by_u_int_1a94019f076ed9b536b1e234cf21859b41>`(unsigned int val = 0);

		// methods
	
		virtual bool :target:`operator <<doxid-class_q_panda_1_1_search_data_by_u_int_1a957a3117bd0a14bf1615185961611cc4>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const;
		virtual bool :target:`operator <=<doxid-class_q_panda_1_1_search_data_by_u_int_1a169b5cacdd8e10c76498b4211311f6b9>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const;
		virtual bool :target:`operator ><doxid-class_q_panda_1_1_search_data_by_u_int_1a73095a75e03ecd1d594715139793ee55>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const;
		virtual bool :target:`operator >=<doxid-class_q_panda_1_1_search_data_by_u_int_1a3e7fb74fb6e2d16712db0b8b8a6deb0e>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const;
		virtual bool :target:`operator ==<doxid-class_q_panda_1_1_search_data_by_u_int_1a295252f3689f471d05584710d3f97272>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`&& other) const;
		virtual :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& :target:`operator -<doxid-class_q_panda_1_1_search_data_by_u_int_1a0182dc594441151969442484a8c7a4e6>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other);
		SearchDataByUInt& :target:`operator =<doxid-class_q_panda_1_1_search_data_by_u_int_1ad5a19a1af163f80a232c6e9ee5bdc248>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other);
		virtual size_t :target:`check_max_need_qubits<doxid-class_q_panda_1_1_search_data_by_u_int_1aa0856e8a83c468900a2b001548d5e9c2>`();
		virtual :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& :target:`set_val<doxid-class_q_panda_1_1_search_data_by_u_int_1a4fc5e5ed4764eec0afa36f42d917e065>`(const char* p_val);
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_to_circuit<doxid-class_q_panda_1_1_search_data_by_u_int_1ae027381b0dbdd0a3904b51e0e2423ee3>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& oracle_qubits,
			size_t use_qubit_cnt,
			const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& mini_data
			) const;
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`build_to_condition_circuit<doxid-class_q_panda_1_1_search_data_by_u_int_1a6dd76f33f47a87cd59f389ac7d678fa6>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& oracle_qubits,
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` cir_mark,
			const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& mini_data
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual bool :ref:`operator <<doxid-class_q_panda_1_1_abstract_search_data_1ac8be608f843f97befcafb8703e108e2e>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const = 0;
		virtual bool :ref:`operator <=<doxid-class_q_panda_1_1_abstract_search_data_1a7810978c9562e0b3d432fcef7603dd73>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const = 0;
		virtual bool :ref:`operator ><doxid-class_q_panda_1_1_abstract_search_data_1a3a64b342f0a64cb4010dfeadb0330250>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const = 0;
		virtual bool :ref:`operator >=<doxid-class_q_panda_1_1_abstract_search_data_1abf75efa070629e9e3af09006c2610b07>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) const = 0;
		virtual bool :ref:`operator ==<doxid-class_q_panda_1_1_abstract_search_data_1aeeb1bd1f0c8816827ac629ba4018de96>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`&& other) const = 0;
		virtual :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& :ref:`operator -<doxid-class_q_panda_1_1_abstract_search_data_1a23d2332f7b25112ab26c44e4da2959d1>` (const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& other) = 0;
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`build_to_circuit<doxid-class_q_panda_1_1_abstract_search_data_1a3c6c99e74388fa49fe4c74be1e24ad90>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& used_qubits, size_t use_qubit_cnt, const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& mini_data) const = 0;
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`build_to_condition_circuit<doxid-class_q_panda_1_1_abstract_search_data_1a5bd409c893b41e165312cc65b9951ffd>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& used_qubits, :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` cir_mark, const :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& mini_data) = 0;
		virtual size_t :ref:`check_max_need_qubits<doxid-class_q_panda_1_1_abstract_search_data_1ace19ca4185587c60bd0da34f47ade3f2>`() = 0;
		virtual :ref:`AbstractSearchData<doxid-class_q_panda_1_1_abstract_search_data>`& :ref:`set_val<doxid-class_q_panda_1_1_abstract_search_data_1a37c2c5a1eee89450a731862cda15049d>`(const char* p_val) = 0;

