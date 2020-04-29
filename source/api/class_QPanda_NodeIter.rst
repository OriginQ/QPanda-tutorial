.. index:: pair: class; QPanda::NodeIter
.. _doxid-class_q_panda_1_1_node_iter:

class QPanda::NodeIter
======================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QNode.h>
	
	class NodeIter
	{
	public:
		// construction
	
		:target:`NodeIter<doxid-class_q_panda_1_1_node_iter_1af1607faeef3e912f70f88c184a4e7a35>`(:ref:`Item<doxid-class_q_panda_1_1_item>`* pItem);
		:target:`NodeIter<doxid-class_q_panda_1_1_node_iter_1a4614e19e6f87fc0234bc82fe88b6855b>`(const NodeIter& oldIter);
		:target:`NodeIter<doxid-class_q_panda_1_1_node_iter_1aba6cca3896c40266f66fc3122192f1ac>`();

		// methods
	
		:ref:`Item<doxid-class_q_panda_1_1_item>`* :target:`getPCur<doxid-class_q_panda_1_1_node_iter_1a2b926914956838f76364453fe2a6d360>`() const;
		void :target:`setPCur<doxid-class_q_panda_1_1_node_iter_1aa8cc1670b74a76b52295e5cef5a7d165>`(:ref:`Item<doxid-class_q_panda_1_1_item>`* pItem);
		NodeIter& :target:`operator ++<doxid-class_q_panda_1_1_node_iter_1ae82f21890c0800f801a6c296474d1d36>` ();
		NodeIter :target:`operator ++<doxid-class_q_panda_1_1_node_iter_1ae09b6138cb4f12bae9064b319be2681b>` (int);
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :target:`operator *<doxid-class_q_panda_1_1_node_iter_1ac2082f367107f05d7be05fbb3ba802d7>` () const;
		NodeIter& :target:`operator --<doxid-class_q_panda_1_1_node_iter_1af432868fc480f9c137908074e79287da>` ();
		NodeIter :target:`operator --<doxid-class_q_panda_1_1_node_iter_1a7616fb29bde9543aed0fb7d0088f56ef>` (int);
		NodeIter :target:`getNextIter<doxid-class_q_panda_1_1_node_iter_1ac97473927bc7fbc465662104552000d5>`();
		bool :target:`operator !=<doxid-class_q_panda_1_1_node_iter_1aedf78992bfc8d21f4e95a390cbaede80>` (NodeIter) const;
		bool :target:`operator ==<doxid-class_q_panda_1_1_node_iter_1ac8d909291187f5626056fc22d86d443d>` (NodeIter) const;
	};
