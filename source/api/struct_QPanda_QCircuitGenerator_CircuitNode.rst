.. index:: pair: struct; QPanda::QCircuitGenerator::CircuitNode
.. _doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node:

struct QPanda::QCircuitGenerator::CircuitNode
=============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct CircuitNode
	{
		// fields
	
		std::string :target:`m_op<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node_1ac8276c2f9a9c844615a5ddfb4d3ee446>`;
		std::vector<uint32_t> :target:`m_target_q<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node_1a1673833bb7c325799427b1d882fa4165>`;
		std::vector<uint32_t> :target:`m_control_q<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node_1a746bf688400229a23ffc64ebcc8fd697>`;
		bool :target:`m_is_dagger<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node_1a644578dbc61d611528e9d0d7906f3c5e>`;
		std::vector<std::string> :target:`m_angle<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node_1a43b38a66100f9a4cb2a938e0f2161675>`;

		// construction
	
		:target:`CircuitNode<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node_1a8976354edbd61373d1a39f14a70b8be9>`();
	
		:target:`CircuitNode<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node_1a21c19f3a5343b249481900d73ba02658>`(
			std::string op,
			const std::vector<uint32_t>& target_q,
			const std::vector<std::string>& angle,
			const std::vector<uint32_t>& control_q,
			bool is_dagger
			);
	};
