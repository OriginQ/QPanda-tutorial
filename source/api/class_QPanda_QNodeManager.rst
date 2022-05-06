.. index:: pair: class; QPanda::QNodeManager
.. _doxid-class_q_panda_1_1_q_node_manager:

class QPanda::QNodeManager
==========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QNodeManager.h>
	
	class QNodeManager
	{
	public:
		// construction
	
		:target:`QNodeManager<doxid-class_q_panda_1_1_q_node_manager_1a7ee937efe949717ce1e1af25d55b4d1f>`(const :ref:`QNode<doxid-class_q_panda_1_1_q_node>`* parent);
		:target:`QNodeManager<doxid-class_q_panda_1_1_q_node_manager_1af8ac57e92a995ac30271b9c383f84c52>`();

		// methods
	
		void :target:`push_back_node<doxid-class_q_panda_1_1_q_node_manager_1acba42fbb5976fb8135ee3913cb09432d>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node);
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`get_first_node_iter<doxid-class_q_panda_1_1_q_node_manager_1ab5d3d8f935a091f7d48943af686d35c9>`();
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`get_last_node_iter<doxid-class_q_panda_1_1_q_node_manager_1a3d7082a3d57f8299669ef275d0e5eef1>`();
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`get_end_node_iter<doxid-class_q_panda_1_1_q_node_manager_1a927417de2e7b629e1fcc7899fcc44fe7>`();
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`get_head_node_iter<doxid-class_q_panda_1_1_q_node_manager_1a156875d1097e017ce97b55102316063e>`();
	
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`insert_QNode<doxid-class_q_panda_1_1_q_node_manager_1a816f3e39562dfb68318c881c28d7cff5>`(
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& perIter,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node
			);
	
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :target:`delete_QNode<doxid-class_q_panda_1_1_q_node_manager_1ae0e2dee6a349f0cd60eae4bdf1f6185b>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`& target_iter);
		void :target:`clear<doxid-class_q_panda_1_1_q_node_manager_1ada08cf640e6a9514eb8c259d47f6ce4f>`();
	};
