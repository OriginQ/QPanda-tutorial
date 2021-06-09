.. index:: pair: class; QPanda::DRAW_TEXT_PIC::DrawByLayer
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_by_layer:

class QPanda::DRAW_TEXT_PIC::DrawByLayer
========================================

.. toctree::
	:hidden:

draw layer nodes


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class DrawByLayer: public :ref:`QPanda::DRAW_TEXT_PIC::AbstractHandleNodes<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes>`
	{
	public:
		// construction
	
		:target:`DrawByLayer<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_by_layer_1a6e1a98d00b51033c9d9b56b8ea8f13e6>`(:ref:`DrawPicture<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture>`& parent);

		// methods
	
		void :target:`handle_measure_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_by_layer_1ad58426d9c81c42d6e25831144ba7b26f>`(
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node,
			:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`& p_node_info
			);
	
		void :target:`handle_reset_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_by_layer_1a7499921dba685df7ffdc018383cfe911>`(
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node,
			:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`& p_node_info
			);
	
		void :target:`handle_gate_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_by_layer_1a3800f045b055e8c916aa0e1f066709f0>`(
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node,
			:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`& p_node_info
			);
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

