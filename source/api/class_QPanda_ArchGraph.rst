.. index:: pair: class; QPanda::ArchGraph
.. _doxid-class_q_panda_1_1_arch_graph:

class QPanda::ArchGraph
=======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

This is the base class for the architectures that this project will be supporting. :ref:`More...<details-class_q_panda_1_1_arch_graph>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ArchGraph.h>
	
	class ArchGraph: public :ref:`QPanda::WeightedGraph<doxid-class_q_panda_1_1_weighted_graph>`
	{
	public:
		// typedefs
	
		typedef ArchGraph* :target:`Ref<doxid-class_q_panda_1_1_arch_graph_1a99f40f087af629451e44d64e7a91bdec>`;
		typedef std::unique_ptr<ArchGraph> :target:`uRef<doxid-class_q_panda_1_1_arch_graph_1a52dde251002cab5358cc23640821e239>`;
		typedef std::shared_ptr<ArchGraph> :target:`sRef<doxid-class_q_panda_1_1_arch_graph_1a9c281b804cf8363fc16ce47e61b53de9>`;
		typedef std::vector<std::pair<std::string, uint32_t>> :target:`RegsVector<doxid-class_q_panda_1_1_arch_graph_1a6695e57d326fd47599c0551fe4c0c2af>`;
		typedef RegsVector::iterator :target:`RegsIterator<doxid-class_q_panda_1_1_arch_graph_1a9af1055c6de8dad694f85b0ff562d945>`;

		// methods
	
		uint32_t :target:`putVertex<doxid-class_q_panda_1_1_arch_graph_1a92560ecf8ddcaba04d9e4d04506cd1d4>`(std::string s);
	
		void :target:`putReg<doxid-class_q_panda_1_1_arch_graph_1a704aa1aaf05933ca6c9de7e694088efb>`(
			std::string id,
			std::string size
			);
	
		uint32_t :target:`get_vertex_count<doxid-class_q_panda_1_1_arch_graph_1a71db3d6218085e764a73bcedc9cd726a>`();
		std::vector<std::vector<int>> :target:`get_adjacent_matrix<doxid-class_q_panda_1_1_arch_graph_1a12e2f54f53bd280e9c79e8fe33349c75>`();
		std::vector<std::vector<double>> :target:`get_adj_weight_matrix<doxid-class_q_panda_1_1_arch_graph_1abc09d59fc8afe6ea51a2320ff205661a>`();
		bool :ref:`isGeneric<doxid-class_q_panda_1_1_arch_graph_1a172cd0ae8b09851c48582f2862d596f6>`();
		:ref:`RegsIterator<doxid-class_q_panda_1_1_arch_graph_1a9af1055c6de8dad694f85b0ff562d945>` :target:`reg_begin<doxid-class_q_panda_1_1_arch_graph_1a225a2527171c3c976cb07231a85667d4>`();
		:ref:`RegsIterator<doxid-class_q_panda_1_1_arch_graph_1a9af1055c6de8dad694f85b0ff562d945>` :target:`reg_end<doxid-class_q_panda_1_1_arch_graph_1ab13424029c821e57129dd2faacd5251e>`();
		std::vector<std::pair<uint32_t, uint32_t>> :target:`get_all_edges<doxid-class_q_panda_1_1_arch_graph_1a55f81959c28c5de3df0b5a9288097fc7>`();
		static bool :target:`ClassOf<doxid-class_q_panda_1_1_arch_graph_1a11dd74c9f84cca8f658dc2571c8b7515>`(const :ref:`Graph<doxid-class_q_panda_1_1_graph>`* g);
		static :ref:`uRef<doxid-class_q_panda_1_1_arch_graph_1a52dde251002cab5358cc23640821e239>` :target:`Create<doxid-class_q_panda_1_1_arch_graph_1afe264d04a535b9a9117003ea193110a1>`(uint32_t n);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`Graph<doxid-class_q_panda_1_1_graph>`* :ref:`Ref<doxid-class_q_panda_1_1_graph_1ac91477f35144fe2bbf3e5ec898bd96e3>`;
		typedef std::unique_ptr<:ref:`Graph<doxid-class_q_panda_1_1_graph>`> :ref:`uRef<doxid-class_q_panda_1_1_graph_1a16445397ef7a07bf9a66089eba05c301>`;
		typedef std::shared_ptr<:ref:`Graph<doxid-class_q_panda_1_1_graph>`> :ref:`sRef<doxid-class_q_panda_1_1_graph_1ac94f722e5b4c4365172440c335968abf>`;
		typedef :ref:`WeightedGraph<doxid-class_q_panda_1_1_weighted_graph>`<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>* :ref:`Ref<doxid-class_q_panda_1_1_weighted_graph_1a0d341785fb24384be65f2df4d341bf40>`;
		typedef std::unique_ptr<:ref:`WeightedGraph<doxid-class_q_panda_1_1_weighted_graph>`<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>> :ref:`uRef<doxid-class_q_panda_1_1_weighted_graph_1a004f1f47805aed33e1154be4cf7d8a9b>`;
		typedef std::shared_ptr<:ref:`WeightedGraph<doxid-class_q_panda_1_1_weighted_graph>`<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>> :ref:`sRef<doxid-class_q_panda_1_1_weighted_graph_1ab4e139d37e3bf1834283398c05b5d2a6>`;

		// enums
	
		enum :ref:`Kind<doxid-class_q_panda_1_1_graph_1a44942fc753a97e4cc34ad9aca5be826b>`;
		enum :ref:`Type<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0>`;

		// methods
	
		uint32_t :ref:`inDegree<doxid-class_q_panda_1_1_graph_1acec6c51b4eaf05fc0a5fe548746edfd6>`(uint32_t i) const;
		uint32_t :ref:`outDegree<doxid-class_q_panda_1_1_graph_1ac16ef642f9bf40dc7b220f7ab06f751a>`(uint32_t i) const;
		uint32_t :ref:`size<doxid-class_q_panda_1_1_graph_1a40bbfdf0743a39d554fcc87975775ab5>`() const;
		std::set<uint32_t>& :ref:`succ<doxid-class_q_panda_1_1_graph_1a153d772f1535f357cbe7c0c50cd2b6e3>`(uint32_t i);
		const std::set<uint32_t>& :ref:`c_succ<doxid-class_q_panda_1_1_graph_1a874e6da07ecb665376db4ce8b48cfb94>`(uint32_t i) const;
		std::set<uint32_t>& :ref:`pred<doxid-class_q_panda_1_1_graph_1ae989a39d199841714e4677187cd2822a>`(uint32_t i);
		std::set<uint32_t> :ref:`adj<doxid-class_q_panda_1_1_graph_1aface3f2abf761590940df4f061dc791e>`(uint32_t i) const;
		void :ref:`putEdge<doxid-class_q_panda_1_1_graph_1aa01d66d3ec49a4b43b19718783b80e47>`(uint32_t i, uint32_t j);
		bool :ref:`hasEdge<doxid-class_q_panda_1_1_graph_1abde4fa4ebb1c201686f55c327eeb1525>`(uint32_t i, uint32_t j) const;
		bool :ref:`isWeighted<doxid-class_q_panda_1_1_graph_1aef2276cd3d4f619d5c450807ba4b233b>`() const;
		bool :ref:`isArch<doxid-class_q_panda_1_1_graph_1a91b257ec542e482fe87c61c1dd5a0b0b>`() const;
		bool :ref:`isDirectedGraph<doxid-class_q_panda_1_1_graph_1a22cdbb3cc434c7317d772c979683c879>`() const;
		std::string :ref:`dotify<doxid-class_q_panda_1_1_graph_1ad7059152b00e0c81c5bd52bdaeeb0650>`(std::string name = "Dump") const;
		static bool :ref:`ClassOf<doxid-class_q_panda_1_1_graph_1adf4beee9b41213052d1e0bd8989eeb1e>`(const :ref:`Graph<doxid-class_q_panda_1_1_graph>`* g);
		static :ref:`uRef<doxid-class_q_panda_1_1_graph_1a16445397ef7a07bf9a66089eba05c301>` :ref:`Create<doxid-class_q_panda_1_1_graph_1ae66095c750d4d17cd9080f176659fd67>`(uint32_t n, :ref:`Type<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0>` ty = :ref:`Undirected<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0a539bbb9d44da151ac636b174cc7f1013>`);
		void :ref:`putEdge<doxid-class_q_panda_1_1_weighted_graph_1ac08cef2b4c6d6357bc7b81b53825a441>`(uint32_t i, uint32_t j, :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` w);
		void :ref:`setW<doxid-class_q_panda_1_1_weighted_graph_1a096f4eefc037efd05068e202dcc76f77>`(uint32_t i, uint32_t j, :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` w);
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` :ref:`getW<doxid-class_q_panda_1_1_weighted_graph_1ae9f6e0920c15fc4b02f0e4b8c278665d>`(uint32_t i, uint32_t j) const;
		static bool :ref:`ClassOf<doxid-class_q_panda_1_1_weighted_graph_1ab0222ef823f09c9f8ffe620d83aa96fc>`(const :ref:`Graph<doxid-class_q_panda_1_1_graph>`* g);
		static :ref:`uRef<doxid-class_q_panda_1_1_graph_1a16445397ef7a07bf9a66089eba05c301>` :ref:`Create<doxid-class_q_panda_1_1_weighted_graph_1a18d55c231ad72b19664c4e666b2a9661>`(uint32_t n, :ref:`Type<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0>` ty = :ref:`Undirected<doxid-class_q_panda_1_1_graph_1a9a507519fc3dd114005091be263b8cb0a539bbb9d44da151ac636b174cc7f1013>`);

.. _details-class_q_panda_1_1_arch_graph:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This is the base class for the architectures that this project will be supporting.

Methods
-------

.. index:: pair: function; isGeneric
.. _doxid-class_q_panda_1_1_arch_graph_1a172cd0ae8b09851c48582f2862d596f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isGeneric()

Returns true if this is a generic architechture graph, i.e.: it was not created by any of the architechtures compiled within the program.

