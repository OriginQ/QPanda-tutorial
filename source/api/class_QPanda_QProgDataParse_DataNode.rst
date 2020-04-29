.. index:: pair: class; QPanda::QProgDataParse::DataNode
.. _doxid-union_q_panda_1_1_q_prog_data_parse_1_1_data_node:

class QPanda::QProgDataParse::DataNode
======================================

.. toctree::
	:hidden:

Quantum program node data.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class DataNode
	{
	public:
		// fields
	
		uint32_t :target:`qubit_data<doxid-union_q_panda_1_1_q_prog_data_parse_1_1_data_node_1a0b5bf973f837a828f5e1cf2e5f74f328>`;
		float :target:`angle_data<doxid-union_q_panda_1_1_q_prog_data_parse_1_1_data_node_1a9c48d2050fc2976f3925649cf4b23162>`;

		// construction
	
		:target:`DataNode<doxid-union_q_panda_1_1_q_prog_data_parse_1_1_data_node_1a27ddbaf87dc4ede022664d87a717b2fd>`();
		:target:`DataNode<doxid-union_q_panda_1_1_q_prog_data_parse_1_1_data_node_1ad434623d5b1874dd01a5b51524ae5744>`(uint32_t data);
		:target:`DataNode<doxid-union_q_panda_1_1_q_prog_data_parse_1_1_data_node_1a964cb14d901c803a4314174671cb0b32>`(float data);
	};
