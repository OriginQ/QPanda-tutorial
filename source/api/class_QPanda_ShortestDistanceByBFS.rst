.. index:: pair: class; QPanda::ShortestDistanceByBFS
.. _doxid-class_q_panda_1_1_shortest_distance_by_b_f_s:

class QPanda::ShortestDistanceByBFS
===================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Calculates the distance between two vertices by applying BFS. :ref:`More...<details-class_q_panda_1_1_shortest_distance_by_b_f_s>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ShortestDistanceByBFS.h>
	
	class ShortestDistanceByBFS
	{
	public:
		// typedefs
	
		typedef ShortestDistanceByBFS* :target:`Ref<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1ae546ef3cc762746f81743e9895a53c01>`;
		typedef std::shared_ptr<ShortestDistanceByBFS> :target:`sRef<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1ad6f76b890260c9db741f923afd7ae03a>`;
		typedef std::unique_ptr<ShortestDistanceByBFS> :target:`uRef<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1a9e5bb3d14b051739bb8ffba65c12693f>`;
		typedef std::vector<uint32_t> :target:`VecUInt32<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1ae4e7bd2b5e88741904ac8e411221d540>`;
		typedef std::vector<:ref:`VecUInt32<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1ae4e7bd2b5e88741904ac8e411221d540>`> :target:`MatrixUInt32<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1a36654c2a04085502652b0fa36fbd4266>`;

		// methods
	
		void :target:`init<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1af90b91474df0b13c6ac6b9f34d2daec3>`(:ref:`Graph::Ref<doxid-class_q_panda_1_1_graph_1ac91477f35144fe2bbf3e5ec898bd96e3>` graph);
	
		uint32_t :target:`get<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1abbc8c5a8f2b01f466b1e95a31fefa31f>`(
			uint32_t u,
			uint32_t v
			);
	
		static :ref:`uRef<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1a9e5bb3d14b051739bb8ffba65c12693f>` :ref:`create<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1a9a0ee7f393c0ad5c02ec9c71f77fb507>`();
	};
.. _details-class_q_panda_1_1_shortest_distance_by_b_f_s:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Calculates the distance between two vertices by applying BFS.

Methods
-------

.. index:: pair: function; create
.. _doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1a9a0ee7f393c0ad5c02ec9c71f77fb507:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`uRef<doxid-class_q_panda_1_1_shortest_distance_by_b_f_s_1a9e5bb3d14b051739bb8ffba65c12693f>` create()

Instantiate one object of this type.

