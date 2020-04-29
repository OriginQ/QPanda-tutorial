.. index:: pair: class; QPanda::FillLayerByNextLayerNodes
.. _doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes:

class QPanda::FillLayerByNextLayerNodes
=======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Fill layer by next layer nodes. :ref:`More...<details-class_q_panda_1_1_fill_layer_by_next_layer_nodes>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class FillLayerByNextLayerNodes: public :ref:`QPanda::AbstractHandleNodes<doxid-class_q_panda_1_1_abstract_handle_nodes>`
	{
	public:
		// construction
	
		:target:`FillLayerByNextLayerNodes<doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes_1a3f255b1fa6b245be5de541a109fe0dd2>`(
			:ref:`DrawPicture<doxid-class_q_panda_1_1_draw_picture>`& parent,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& unused_qubits_vec,
			:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`& target_layer,
			:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`& next_layer
			);

		// methods
	
		void :target:`handle_measure_node<doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes_1a9ec854074942485dc049ed0d84b6eefe>`(SequenceLayer::iterator& itr_on_next_layer);
		void :target:`handle_reset_node<doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes_1a0c218a1ad856ef45043067b78b16e7b6>`(SequenceLayer::iterator& itr_on_next_layer);
		void :target:`handle_gate_node<doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes_1afc97b277ee53f96fee34bf91277869e1>`(SequenceLayer::iterator& itr_on_next_layer);
		bool :ref:`have_got_available_node<doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes_1a304c02c8183dc9998eabb0b8035210d2>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual void :ref:`handle_measure_node<doxid-class_q_panda_1_1_abstract_handle_nodes_1a80b30eaad05c74b9f33f504c826ac1e5>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_reset_node<doxid-class_q_panda_1_1_abstract_handle_nodes_1a294e7a69d1b81bcf5f2e037949d436c8>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_gate_node<doxid-class_q_panda_1_1_abstract_handle_nodes_1ac265826cf46fadc107a5137f5fec31a1>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_work<doxid-class_q_panda_1_1_abstract_handle_nodes_1a66b6cbe7db19cf9248f89cbdae98a690>`(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` node_t, Args&&... func_args);

.. _details-class_q_panda_1_1_fill_layer_by_next_layer_nodes:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Fill layer by next layer nodes.

Methods
-------

.. index:: pair: function; have_got_available_node
.. _doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes_1a304c02c8183dc9998eabb0b8035210d2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool have_got_available_node()

judge whether get available node



.. rubric:: Returns:

bool if got available node, return true, or else return false

