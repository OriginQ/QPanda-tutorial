.. index:: pair: class; QPanda::Graph
.. _doxid-class_q_panda_1_1_graph:

class QPanda::Graph
===================

.. toctree::
	:hidden:

	enum_QPanda_Graph_Kind.rst
	enum_QPanda_Graph_Type.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Graph.h>
	
	class Graph
	{
	public:
		// typedefs
	
		typedef Graph* :target:`Ref<doxid-class_q_panda_1_1_graph_1ac91477f35144fe2bbf3e5ec898bd96e3>`;
		typedef std::unique_ptr<Graph> :target:`uRef<doxid-class_q_panda_1_1_graph_1a16445397ef7a07bf9a66089eba05c301>`;
		typedef std::shared_ptr<Graph> :target:`sRef<doxid-class_q_panda_1_1_graph_1ac94f722e5b4c4365172440c335968abf>`;

		// enums
	
		enum :ref:`Kind<doxid-class_q_panda_1_1_graph_1a44942fc753a97e4cc34ad9aca5be826b>`;
		enum :ref:`Type<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0>`;

		// construction
	
		:target:`Graph<doxid-class_q_panda_1_1_graph_1a57eacec00461fba93f0672a7feed886e>`(
			uint32_t n,
			:ref:`Type<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0>` ty = :ref:`Undirected<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0a539bbb9d44da151ac636b174cc7f1013>`
			);

		// methods
	
		uint32_t :target:`inDegree<doxid-class_q_panda_1_1_graph_1acec6c51b4eaf05fc0a5fe548746edfd6>`(uint32_t i) const;
		uint32_t :target:`outDegree<doxid-class_q_panda_1_1_graph_1ac16ef642f9bf40dc7b220f7ab06f751a>`(uint32_t i) const;
		uint32_t :target:`size<doxid-class_q_panda_1_1_graph_1a40bbfdf0743a39d554fcc87975775ab5>`() const;
		std::set<uint32_t>& :target:`succ<doxid-class_q_panda_1_1_graph_1a153d772f1535f357cbe7c0c50cd2b6e3>`(uint32_t i);
		const std::set<uint32_t>& :target:`c_succ<doxid-class_q_panda_1_1_graph_1a874e6da07ecb665376db4ce8b48cfb94>`(uint32_t i) const;
		std::set<uint32_t>& :target:`pred<doxid-class_q_panda_1_1_graph_1ae989a39d199841714e4677187cd2822a>`(uint32_t i);
		std::set<uint32_t> :target:`adj<doxid-class_q_panda_1_1_graph_1aface3f2abf761590940df4f061dc791e>`(uint32_t i) const;
	
		void :target:`putEdge<doxid-class_q_panda_1_1_graph_1aa01d66d3ec49a4b43b19718783b80e47>`(
			uint32_t i,
			uint32_t j
			);
	
		bool :target:`hasEdge<doxid-class_q_panda_1_1_graph_1abde4fa4ebb1c201686f55c327eeb1525>`(
			uint32_t i,
			uint32_t j
			) const;
	
		bool :target:`isWeighted<doxid-class_q_panda_1_1_graph_1aef2276cd3d4f619d5c450807ba4b233b>`() const;
		bool :target:`isArch<doxid-class_q_panda_1_1_graph_1a91b257ec542e482fe87c61c1dd5a0b0b>`() const;
		bool :target:`isDirectedGraph<doxid-class_q_panda_1_1_graph_1a22cdbb3cc434c7317d772c979683c879>`() const;
		std::string :target:`dotify<doxid-class_q_panda_1_1_graph_1ad7059152b00e0c81c5bd52bdaeeb0650>`(std::string name = "Dump") const;
		static bool :target:`ClassOf<doxid-class_q_panda_1_1_graph_1adf4beee9b41213052d1e0bd8989eeb1e>`(const Graph* g);
	
		static :ref:`uRef<doxid-class_q_panda_1_1_graph_1a16445397ef7a07bf9a66089eba05c301>` :target:`Create<doxid-class_q_panda_1_1_graph_1ae66095c750d4d17cd9080f176659fd67>`(
			uint32_t n,
			:ref:`Type<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0>` ty = :ref:`Undirected<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0a539bbb9d44da151ac636b174cc7f1013>`
			);
	};

	// direct descendants

	template <typename T>
	class :ref:`WeightedGraph<doxid-class_q_panda_1_1_weighted_graph>`;
