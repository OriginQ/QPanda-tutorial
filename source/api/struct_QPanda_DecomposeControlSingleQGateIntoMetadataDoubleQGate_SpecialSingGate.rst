.. index:: pair: struct; QPanda::DecomposeControlSingleQGateIntoMetadataDoubleQGate::SpecialSingGate
.. _doxid-struct_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate_1_1_special_sing_gate:

struct QPanda::DecomposeControlSingleQGateIntoMetadataDoubleQGate::SpecialSingGate
==================================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct SpecialSingGate
	{
		// fields
	
		double :target:`m_alpha<doxid-struct_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate_1_1_special_sing_gate_1a07bb42c1f612cf46242c9c9320c5c1d3>`;
		double :target:`m_beta<doxid-struct_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate_1_1_special_sing_gate_1adfb364ede4a8c89d3ed9d803306bb921>`;
		double :target:`m_delta<doxid-struct_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate_1_1_special_sing_gate_1a49a1df311d20854c6465bec19bc6b7e9>`;
		double :target:`m_gamma<doxid-struct_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate_1_1_special_sing_gate_1a16f4a0f4c86d65ffea13e4e4fea4a9ad>`;

		// methods
	
		std::vector<double> :target:`parse_angle<doxid-struct_q_panda_1_1_decompose_control_single_q_gate_into_metadata_double_q_gate_1_1_special_sing_gate_1aaec6757dcfb30bbb3a8db588c9912302>`(
			double alpha,
			double beta,
			double delta,
			double gamma
			) const;
	};
