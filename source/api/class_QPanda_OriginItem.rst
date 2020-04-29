.. index:: pair: class; QPanda::OriginItem
.. _doxid-class_q_panda_1_1_origin_item:

class QPanda::OriginItem
========================

.. toctree::
	:hidden:

Origin item implementation class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QNode.h>
	
	class OriginItem: public :ref:`QPanda::Item<doxid-class_q_panda_1_1_item>`
	{
	public:
		// methods
	
		virtual :ref:`Item<doxid-class_q_panda_1_1_item>`* :target:`getNext<doxid-class_q_panda_1_1_origin_item_1a3fe1fffddfdeca8ae6e8dc4543b2adf1>`() const;
		virtual :ref:`Item<doxid-class_q_panda_1_1_item>`* :target:`getPre<doxid-class_q_panda_1_1_origin_item_1a3794a222ae36499a91534778fa80afc9>`() const;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :target:`getNode<doxid-class_q_panda_1_1_origin_item_1a1c25a87a1b943c49afa4534011c9cf7b>`() const;
		virtual void :target:`setNext<doxid-class_q_panda_1_1_origin_item_1aa635d792a5bef2b81f25332e7ff33d09>`(:ref:`Item<doxid-class_q_panda_1_1_item>`* pItem);
		virtual void :target:`setPre<doxid-class_q_panda_1_1_origin_item_1ae8f0e98222699b42f104466e0deb9c76>`(:ref:`Item<doxid-class_q_panda_1_1_item>`* pItem);
		virtual void :target:`setNode<doxid-class_q_panda_1_1_origin_item_1af90f7cf7ca96c2770efab85d737b239c>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> pNode);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`Item<doxid-class_q_panda_1_1_item>`* :ref:`getNext<doxid-class_q_panda_1_1_item_1a4ba41499f3d9b25e993430d60a87c9e4>`() const = 0;
		virtual :ref:`Item<doxid-class_q_panda_1_1_item>`* :ref:`getPre<doxid-class_q_panda_1_1_item_1a173d121be6ba7f748bbd182d80183e0e>`() const = 0;
		virtual std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`getNode<doxid-class_q_panda_1_1_item_1ad28ca697c2ce79c7c064cb24e6d2d6f5>`() const = 0;
		virtual void :ref:`setNext<doxid-class_q_panda_1_1_item_1a5acda15cef9a32e6a1d70a6dd7da9f2f>`(:ref:`Item<doxid-class_q_panda_1_1_item>`*) = 0;
		virtual void :ref:`setPre<doxid-class_q_panda_1_1_item_1ac75c3380e7a9e0353812b58236b27991>`(:ref:`Item<doxid-class_q_panda_1_1_item>`*) = 0;
		virtual void :ref:`setNode<doxid-class_q_panda_1_1_item_1ade5a8cd5c98bad9f2db7b052686249fe>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> pNode) = 0;

