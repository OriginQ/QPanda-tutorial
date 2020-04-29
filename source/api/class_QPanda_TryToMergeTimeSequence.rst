.. index:: pair: class; QPanda::TryToMergeTimeSequence
.. _doxid-class_q_panda_1_1_try_to_merge_time_sequence:

class QPanda::TryToMergeTimeSequence
====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Try to merge time sequence. :ref:`More...<details-class_q_panda_1_1_try_to_merge_time_sequence>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class TryToMergeTimeSequence: public :ref:`QPanda::AbstractHandleNodes<doxid-class_q_panda_1_1_abstract_handle_nodes>`
	{
	public:
		// construction
	
		:target:`TryToMergeTimeSequence<doxid-class_q_panda_1_1_try_to_merge_time_sequence_1a57547a4250ab2deebb288aa7053851ba>`(
			:ref:`DrawPicture<doxid-class_q_panda_1_1_draw_picture>`& parent,
			:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`& next_layer
			);

		// methods
	
		void :target:`handle_measure_node<doxid-class_q_panda_1_1_try_to_merge_time_sequence_1a1a1442fa566f1a0230f25894d623868c>`(
			DrawPicture::wireIter& cur_qu_wire,
			SequenceLayer::iterator& itr_on_next_layer,
			bool& b_found_node_on_cur_qu_wire
			);
	
		void :target:`handle_reset_node<doxid-class_q_panda_1_1_try_to_merge_time_sequence_1a3f75d15a0933c1eae0ad2456b615287c>`(
			DrawPicture::wireIter& cur_qu_wire,
			SequenceLayer::iterator& itr_on_next_layer,
			bool& b_found_node_on_cur_qu_wire
			);
	
		void :target:`handle_gate_node<doxid-class_q_panda_1_1_try_to_merge_time_sequence_1a28ba08f30622a6432a0bccc327f37355>`(
			DrawPicture::wireIter& cur_qu_wire,
			SequenceLayer::iterator& itr_on_next_layer,
			bool& b_found_node_on_cur_qu_wire
			);
	
		bool :ref:`could_continue_merge<doxid-class_q_panda_1_1_try_to_merge_time_sequence_1a420938c270391039c8921d60cd067bdc>`();
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

.. _details-class_q_panda_1_1_try_to_merge_time_sequence:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Try to merge time sequence.

Methods
-------

.. index:: pair: function; could_continue_merge
.. _doxid-class_q_panda_1_1_try_to_merge_time_sequence_1a420938c270391039c8921d60cd067bdc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool could_continue_merge()

judge whether to continue recurse



.. rubric:: Returns:

bool if could to continue recurse, return true, or else return false

