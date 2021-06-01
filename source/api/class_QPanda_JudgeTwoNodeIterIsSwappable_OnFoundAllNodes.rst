.. index:: pair: class; QPanda::JudgeTwoNodeIterIsSwappable::OnFoundAllNodes
.. _doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_found_all_nodes:

class QPanda::JudgeTwoNodeIterIsSwappable::OnFoundAllNodes
==========================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class OnFoundAllNodes: public QPanda::JudgeTwoNodeIterIsSwappable::AbstractJudgeStatueInterface
	{
	public:
		// construction
	
		:target:`OnFoundAllNodes<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_found_all_nodes_1a1c385cab93bafeebd1d679c955718921>`(
			:ref:`JudgeTwoNodeIterIsSwappable<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable>`& parent,
			ResultStatue s
			);

		// methods
	
		void :target:`on_traversal_end<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_found_all_nodes_1aef4a60919c973ab9a39034d1f4c0b499>`();
		ResultStatue :target:`get_statue<doxid-class_q_panda_1_1_judge_two_node_iter_is_swappable_1_1_on_found_all_nodes_1ae86fdb2632461eb729efa6ddb719e65b>`() const;
	};
