.. index:: pair: struct; QPanda::SU4TopologyMatch::gates_digraph
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph:

struct QPanda::SU4TopologyMatch::gates_digraph
==============================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Simple digraph, used to group all gates. :ref:`More...<details-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct gates_digraph
	{
		// fields
	
		std::map<size_t, std::pair<std::vector<gate>, std::vector<int>>> :target:`vertexs<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1a9ad88355ad4ff5e4e7afb608af802b9a>`;
		std::vector<std::pair<size_t, size_t>> :ref:`edges<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1acbcf7af9fc7680e731238d8eb6fae8de>`;
		size_t :target:`id<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1af3f0fa48cdd125604150f8da1762c560>` = 0;

		// methods
	
		size_t :target:`add_vertex<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1a72ada4e1c7a67fba55e4c72b88b0e9d5>`(std::pair<std::vector<gate>, std::vector<int>> info);
	
		bool :target:`add_edge<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1a31e0f045a4fcb202d728b65eab8b764a>`(
			size_t u,
			size_t v
			);
	
		bool :target:`remove_vertex<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1af7235e3610e48a8dd2e3ac75770cab41>`(size_t id);
		size_t :target:`in_degree<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1a5276cc959c05fbea7f577d14f7689fb4>`(size_t id);
	};
.. _details-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Simple digraph, used to group all gates.

Fields
------

.. index:: pair: variable; edges
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph_1acbcf7af9fc7680e731238d8eb6fae8de:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::pair<size_t, size_t>> edges

in --> out

