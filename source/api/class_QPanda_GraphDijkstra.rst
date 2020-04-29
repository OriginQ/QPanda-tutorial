.. index:: pair: class; QPanda::GraphDijkstra
.. _doxid-class_q_panda_1_1_graph_dijkstra:

class QPanda::GraphDijkstra
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Solutions for Dijkstra algorithm. :ref:`More...<details-class_q_panda_1_1_graph_dijkstra>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <GraphDijkstra.h>
	
	class GraphDijkstra
	{
	public:
		// construction
	
		:target:`GraphDijkstra<doxid-class_q_panda_1_1_graph_dijkstra_1af169543122193fcf0e3bd4a64e76d808>`();
		:target:`GraphDijkstra<doxid-class_q_panda_1_1_graph_dijkstra_1a4a357cca61b3f7c8488fc5c06d644437>`(const std::vector<std::vector<int>>& matrix);

		// methods
	
		int :ref:`getShortestPath<doxid-class_q_panda_1_1_graph_dijkstra_1a1a474cd7c7e4abd5b07daf0bb4dc83f2>`(int begin, int end, std::vector<int>& path_vec);
		bool :ref:`is_connective<doxid-class_q_panda_1_1_graph_dijkstra_1a194beca99d848dbae810a4f8a385f5f4>`();
	};
.. _details-class_q_panda_1_1_graph_dijkstra:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Solutions for Dijkstra algorithm.

Methods
-------

.. index:: pair: function; getShortestPath
.. _doxid-class_q_panda_1_1_graph_dijkstra_1a1a474cd7c7e4abd5b07daf0bb4dc83f2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int getShortestPath(int begin, int end, std::vector<int>& path_vec)

Get the shortest path of the graph between begin with end.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- Begin: starting point

	*
		- int

		- End: end point

	*
		- std::vector<int>&

		- path_vec: The points at which the shortes path passes



.. rubric:: Returns:

int The length of the shortes path

.. index:: pair: function; is_connective
.. _doxid-class_q_panda_1_1_graph_dijkstra_1a194beca99d848dbae810a4f8a385f5f4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_connective()

Determine if the graph is connected.



.. rubric:: Returns:

bool Result of the judgement



.. rubric:: See also:

