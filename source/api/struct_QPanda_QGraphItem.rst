.. index:: pair: struct; QPanda::QGraphItem
.. _doxid-struct_q_panda_1_1_q_graph_item:

struct QPanda::QGraphItem
=========================

.. toctree::
	:hidden:

Graph element structure.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <DataStruct.h>
	
	struct QGraphItem
	{
		// fields
	
		size_t :target:`first<doxid-struct_q_panda_1_1_q_graph_item_1a93ed5da7a2190055cb423e21a7562617>`;
		size_t :target:`second<doxid-struct_q_panda_1_1_q_graph_item_1a69f565d69ced1941c966fd472d98d55b>`;
		double :target:`weight<doxid-struct_q_panda_1_1_q_graph_item_1acb448dd2a76c687bd5aca389ab9bc081>`;

		// construction
	
		:target:`QGraphItem<doxid-struct_q_panda_1_1_q_graph_item_1a3e15394e7fdae378f58da2a17e77a90c>`();
	
		:target:`QGraphItem<doxid-struct_q_panda_1_1_q_graph_item_1a1a281b9502a306846272999fefe58963>`(
			size_t first,
			size_t second,
			double weight
			);
	};
