.. index:: pair: struct; QPanda::CutQCircuit::CutFragment
.. _doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment:

struct QPanda::CutQCircuit::CutFragment
=======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct CutFragment
	{
		// fields
	
		std::set<uint32_t> :target:`m_vertice<doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1a6a862b2563915da1d85f8ce4864b0baa>`;
		std::set<uint32_t> :target:`m_qubit<doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1a3ed91c0d70d9063192aa617c2365e303>`;
		std::set<uint32_t> :ref:`m_prep_qubit<doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1a907ae4e8414b5860fda6f31cab4a4e1c>`;
		std::set<uint32_t> :ref:`m_meas_qubit<doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1af786218dc3b68a81a903789d351a57ad>`;
		std::map<uint32_t, uint32_t> :target:`m_auxi_qubit_map<doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1acbfc1dd487de16c166fa2ff91c8e0842>`;
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`m_cir<doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1a39e6a4099bf9c57819d339e4c54c16ea>`;
	};
.. _details-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Fields
------

.. index:: pair: variable; m_prep_qubit
.. _doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1a907ae4e8414b5860fda6f31cab4a4e1c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::set<uint32_t> m_prep_qubit

preparation-qubit fragment

.. index:: pair: variable; m_meas_qubit
.. _doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment_1af786218dc3b68a81a903789d351a57ad:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::set<uint32_t> m_meas_qubit

measure-qubit

