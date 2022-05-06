.. index:: pair: class; QuickBB::Graph
.. _doxid-class_quick_b_b_1_1_graph:

class QuickBB::Graph
====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuickBB.h>
	
	class Graph
	{
	public:
		// methods
	
		const :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`& :target:`get_neighborhood<doxid-class_quick_b_b_1_1_graph_1ace12a885b0e60b875b8efcc993914644>`(:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` nodeIndex) const;
		auto :target:`begin<doxid-class_quick_b_b_1_1_graph_1a7261cab68fdd8702bdb6e95352e4b969>`() const;
		auto :target:`end<doxid-class_quick_b_b_1_1_graph_1ae6c27173a7715e591386e566818abc51>`() const;
		void :target:`remove_vertex<doxid-class_quick_b_b_1_1_graph_1acf8a064fd7b29f1b0512a31b9b510778>`(:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` vertexIndex);
	
		bool :target:`has_edge<doxid-class_quick_b_b_1_1_graph_1a357e4a7b2e8c11d127f744c7266bc18a>`(
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` u,
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` v
			) const;
	
		bool :target:`add_edge<doxid-class_quick_b_b_1_1_graph_1aad26e977aa772ea2081c81493657d9d0>`(
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` u,
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` v
			);
	
		bool :target:`remove_edge<doxid-class_quick_b_b_1_1_graph_1af4b638bc74dca26f175d4cb0fef0ad47>`(
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` u,
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` v
			);
	
		void :target:`contract_edge<doxid-class_quick_b_b_1_1_graph_1a78c2e7e4d40f21eaca599154d25b24a6>`(
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` u,
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` v
			);
	
		:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` :target:`degree<doxid-class_quick_b_b_1_1_graph_1a18df92a1d9c50c625b688f8098c18372>`(:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` nodeIndex) const;
		:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` :target:`order<doxid-class_quick_b_b_1_1_graph_1a2acb3e66b60729945bab3ad66afcd7e9>`() const;
	};
