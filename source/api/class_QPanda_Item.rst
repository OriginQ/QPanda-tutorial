.. index:: pair: class; QPanda::Item
.. _doxid-class_q_panda_1_1_item:

class QPanda::Item
==================

.. toctree::
	:hidden:

:ref:`Item <doxid-class_q_panda_1_1_item>` basic abstract class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QNode.h>
	
	class Item
	{
	public:
		// methods
	
		virtual Item* :target:`getNext<doxid-class_q_panda_1_1_item_1a4ba41499f3d9b25e993430d60a87c9e4>`() const = 0;
		virtual Item* :target:`getPre<doxid-class_q_panda_1_1_item_1a173d121be6ba7f748bbd182d80183e0e>`() const = 0;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :target:`getNode<doxid-class_q_panda_1_1_item_1ad28ca697c2ce79c7c064cb24e6d2d6f5>`() const = 0;
		virtual void :target:`setNext<doxid-class_q_panda_1_1_item_1a5acda15cef9a32e6a1d70a6dd7da9f2f>`(Item*) = 0;
		virtual void :target:`setPre<doxid-class_q_panda_1_1_item_1ac75c3380e7a9e0353812b58236b27991>`(Item*) = 0;
		virtual void :target:`setNode<doxid-class_q_panda_1_1_item_1ade5a8cd5c98bad9f2db7b052686249fe>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> pNode) = 0;
	};

	// direct descendants

	class :ref:`OriginItem<doxid-class_q_panda_1_1_origin_item>`;
