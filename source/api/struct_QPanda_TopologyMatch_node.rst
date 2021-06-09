.. index:: pair: struct; QPanda::TopologyMatch::node
.. _doxid-struct_q_panda_1_1_topology_match_1_1node:

struct QPanda::TopologyMatch::node
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct node
	{
		// fields
	
		int :target:`cost_fixed<doxid-struct_q_panda_1_1_topology_match_1_1node_1ab9ccd7c27b4eaa78ccdd261df4f93a50>`;
		int :target:`cost_heur<doxid-struct_q_panda_1_1_topology_match_1_1node_1af5f2fcb499d8a015ad6b3725270588ea>`;
		int :target:`cost_heur2<doxid-struct_q_panda_1_1_topology_match_1_1node_1ad35e3a2cebaf7528e0f871f23133b5a4>`;
		int :target:`depth<doxid-struct_q_panda_1_1_topology_match_1_1node_1a0bde176fed9e4530635fbeb7958ccbba>`;
		std::vector<int> :target:`qubits<doxid-struct_q_panda_1_1_topology_match_1_1node_1ab466b0728e20f0bd4118bb8e4631ed8b>`;
		std::vector<int> :target:`locations<doxid-struct_q_panda_1_1_topology_match_1_1node_1a0d36e10ba0898a26dba7afd4d63199a6>`;
		int :target:`nswaps<doxid-struct_q_panda_1_1_topology_match_1_1node_1aa58c62b55d303793105cd243099df78c>`;
		int :target:`done<doxid-struct_q_panda_1_1_topology_match_1_1node_1aef46784a95243abfc06c5a6b3d982db3>`;
		std::vector<std::vector<edge>> :target:`swaps<doxid-struct_q_panda_1_1_topology_match_1_1node_1a50c97875edea8b0abdd239b0fceb1db8>`;
	};
