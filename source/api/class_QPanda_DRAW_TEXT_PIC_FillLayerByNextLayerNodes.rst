.. index:: pair: class; QPanda::DRAW_TEXT_PIC::FillLayerByNextLayerNodes
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes:

class QPanda::DRAW_TEXT_PIC::FillLayerByNextLayerNodes
======================================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Fill layer by next layer nodes. :ref:`More...<details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class FillLayerByNextLayerNodes: public :ref:`QPanda::DRAW_TEXT_PIC::AbstractHandleNodes<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes>`
	{
	public:
		// construction
	
		:target:`FillLayerByNextLayerNodes<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes_1a2bbdb2023c944e5b01476fe76145997d>`(
			:ref:`DrawPicture<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture>`& parent,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& unused_qubits_vec,
			:ref:`TopoSeqLayer<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1a1d8fafcae9df54dd8402be9279e5a577>`& target_layer,
			:ref:`TopoSeqLayer<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1a1d8fafcae9df54dd8402be9279e5a577>`& next_layer
			);

		// methods
	
		void :target:`handle_measure_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes_1a5ef769cbd8c9f21144f40d63dedbc9c0>`(:ref:`TopoSeqLayerIter<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1aef95ef7785dbd388c38f5ceab2087890>`& itr_on_next_layer);
		void :target:`handle_reset_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes_1a779e050ba909e48564243843d6991dfa>`(:ref:`TopoSeqLayerIter<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1aef95ef7785dbd388c38f5ceab2087890>`& itr_on_next_layer);
		void :target:`handle_gate_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes_1ae6b6ea30d44c5e8075ab34e87ce74858>`(:ref:`TopoSeqLayerIter<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1aef95ef7785dbd388c38f5ceab2087890>`& itr_on_next_layer);
		bool :ref:`have_got_available_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes_1a1778bfa7a0ea00a5a03ca6f4f8dd787d>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual void :ref:`handle_measure_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1ad039a9c5d1e99f73ce341480a6116074>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_reset_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1a54be32b87f0591523496103f4d8ee213>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_gate_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1a4c2cea51ac1610ae83c106a0a03781f1>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_work<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1ad69f9d8ce5231c4339eb98e4966904cc>`(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` node_t, Args&&... func_args);

.. _details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Fill layer by next layer nodes.

Methods
-------

.. index:: pair: function; have_got_available_node
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes_1a1778bfa7a0ea00a5a03ca6f4f8dd787d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool have_got_available_node()

judge whether get available node



.. rubric:: Returns:

bool if got available node, return true, or else return false

