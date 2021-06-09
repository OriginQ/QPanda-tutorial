.. index:: pair: class; QPanda::DRAW_TEXT_PIC::GetUsedQubits
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_get_used_qubits:

class QPanda::DRAW_TEXT_PIC::GetUsedQubits
==========================================

.. toctree::
	:hidden:

get all used qubits


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class GetUsedQubits: public :ref:`QPanda::DRAW_TEXT_PIC::AbstractHandleNodes<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes>`
	{
	public:
		// construction
	
		:target:`GetUsedQubits<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_get_used_qubits_1a045427765ff8e9e3532d7e61e2b237a4>`(
			:ref:`DrawPicture<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture>`& parent,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec
			);

		// methods
	
		void :target:`handle_measure_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_get_used_qubits_1a1fec8239c25c10949afc43edfce9d560>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
		void :target:`handle_reset_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_get_used_qubits_1a88d728b5f4fe372f2e2307286dcf7b4e>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
		void :target:`handle_gate_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_get_used_qubits_1a108a4e02870b8fdfe5c636fa6e4df44d>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
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

