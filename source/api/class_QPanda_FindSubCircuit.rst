.. index:: pair: class; QPanda::FindSubCircuit
.. _doxid-class_q_panda_1_1_find_sub_circuit:

class QPanda::FindSubCircuit
============================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitOptimize.h>
	
	class FindSubCircuit
	{
	public:
		// typedefs
	
		typedef :ref:`SeqNode<doxid-namespace_q_panda_1a428cfe37e5f8fe10b03e17bd47e56808>`<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> :target:`MatchNode<doxid-class_q_panda_1_1_find_sub_circuit_1a6f6a5c26934d15ed0907eaa3b1ab482c>`;
		typedef std::vector<:ref:`MatchNode<doxid-class_q_panda_1_1_find_sub_circuit_1a6f6a5c26934d15ed0907eaa3b1ab482c>`<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>> :target:`MatchNodeVec<doxid-class_q_panda_1_1_find_sub_circuit_1a44847444eae8c2f16619856d934152c1>`;
		typedef std::vector<std::pair<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`, :ref:`MatchNodeVec<doxid-class_q_panda_1_1_find_sub_circuit_1a44847444eae8c2f16619856d934152c1>`<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>>> :target:`MatchNodeTable<doxid-class_q_panda_1_1_find_sub_circuit_1a7027be4854ece3b80ceb84ffe36e8307>`;

		// construction
	
		:target:`FindSubCircuit<doxid-class_q_panda_1_1_find_sub_circuit_1aa0afa01488d8eeb9297033533325a9d3>`(:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& topolog_sequence);

		// methods
	
		void :ref:`sub_cir_query<doxid-group___utilities_1ga98f8e27f8d14cb10ccfe86eadb2b72f6>`(:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& sub_sequence);
	
		bool :target:`node_match<doxid-class_q_panda_1_1_find_sub_circuit_1ac37a22adb6c41a5901893ee685953657>`(
			const :ref:`SeqNode<doxid-namespace_q_panda_1a428cfe37e5f8fe10b03e17bd47e56808>`<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>& target_seq_node,
			const :ref:`SeqNode<doxid-namespace_q_panda_1a428cfe37e5f8fe10b03e17bd47e56808>`<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>& graph_node
			);
	
		bool :target:`check_angle<doxid-class_q_panda_1_1_find_sub_circuit_1a43364cf3d13b9b668019c6d8ddc5b220>`(
			const :ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>` node_1,
			const :ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>` node_2
			);
	
		void :ref:`match_layer<doxid-group___utilities_1ga2f1d4adcbb4069815651f15127ca164f>`(:ref:`SeqLayer<doxid-namespace_q_panda_1a6ed9ed67bc56f43d141fc68fec4c6231>`<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>& sub_seq_layer, const size_t match_layer, std::vector<:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`>& sub_graph_vec);
	
		void :ref:`merge_sub_graph_vec<doxid-group___utilities_1ga11e904035981925506cb8459bcd8116b>`(
			std::vector<:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`>& sub_graph_vec,
			const size_t match_layer,
			:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& target_sub_sequence
			);
	
		void :ref:`clean_sub_graph_vec<doxid-group___utilities_1ga75b7ecc1316df12b781e7e0d7e8b2a1f>`(std::vector<:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`>& sub_graph_vec, :ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& target_sub_sequence);
		void :ref:`merge_topolog_sequence<doxid-group___utilities_1ga2fa18e5bc2684b0eef3a7ec427f0eca7>`(:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& src_seq, :ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& dst_seq);
		const std::vector<:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`>& :target:`get_sub_graph_vec<doxid-class_q_panda_1_1_find_sub_circuit_1ab11d942c7f83b3ade55ca4969058ca15>`();
		void :target:`clear<doxid-class_q_panda_1_1_find_sub_circuit_1ad8ff4d47162bfed1e4964661f094f68f>`();
	};
.. _details-class_q_panda_1_1_find_sub_circuit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; sub_cir_query
.. _doxid-group___utilities_1ga98f8e27f8d14cb10ccfe86eadb2b72f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void sub_cir_query(:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& sub_sequence)

Query the subgraph and store the query results in query_Result.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- LayeredTopoSeq&

		- store the query results



.. rubric:: Returns:

.. index:: pair: function; match_layer
.. _doxid-group___utilities_1ga2f1d4adcbb4069815651f15127ca164f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void match_layer(
		:ref:`SeqLayer<doxid-namespace_q_panda_1a6ed9ed67bc56f43d141fc68fec4c6231>`<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>& sub_seq_layer,
		const size_t match_layer,
		std::vector<:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`>& sub_graph_vec
		)

Layer matching: matching and combining the nodes of each layer of the sub graph.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- SeqLayer<pOptimizerNodeInfo>&

		- the target matching sub-seq-layer

	*
		- const

		- size_t the current matching layer

	*
		- std::vector<LayeredTopoSeq>&

		- sub-graph vector



.. rubric:: Returns:

.. index:: pair: function; merge_sub_graph_vec
.. _doxid-group___utilities_1ga11e904035981925506cb8459bcd8116b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void merge_sub_graph_vec(
		std::vector<:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`>& sub_graph_vec,
		const size_t match_layer,
		:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& target_sub_sequence
		)

Merge incomplete subgraphs Implementation method: get the node set of the next layer of each subgraph of the matching subgraph set. If the node set of the next layer of the two subgraphs has duplicate elements, merge the two subgraphs.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<LayeredTopoSeq>&

		- the sub graph vector

	*
		- const

		- size_t the target layer

	*
		- LayeredTopoSeq&

		- the target sub-sequence



.. rubric:: Returns:

.. index:: pair: function; clean_sub_graph_vec
.. _doxid-group___utilities_1ga75b7ecc1316df12b781e7e0d7e8b2a1f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void clean_sub_graph_vec(std::vector<:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`>& sub_graph_vec, :ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& target_sub_sequence)

Clean up the result set of matching subgraphs and delete the wrong matches.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<LayeredTopoSeq>&

		- the result set of matching subgraphs

	*
		- LayeredTopoSeq&

		- the target sub-sequence



.. rubric:: Returns:

.. index:: pair: function; merge_topolog_sequence
.. _doxid-group___utilities_1ga2fa18e5bc2684b0eef3a7ec427f0eca7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void merge_topolog_sequence(:ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& src_seq, :ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& dst_seq)

merge sub-graph: merging src_seq into dst_seq by layer



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- LayeredTopoSeq&

		- the src_seq

	*
		- LayeredTopoSeq&

		- dst_seq



.. rubric:: Returns:

