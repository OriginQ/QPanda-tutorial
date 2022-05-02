.. index:: pair: class; QPanda::DRAW_TEXT_PIC::AbstractHandleNodes
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes:

template class QPanda::DRAW_TEXT_PIC::AbstractHandleNodes
=========================================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

node handle :ref:`More...<details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	template <typename... Args>
	class AbstractHandleNodes
	{
	public:
		// methods
	
		virtual void :ref:`handle_measure_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1ad039a9c5d1e99f73ce341480a6116074>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_reset_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1a54be32b87f0591523496103f4d8ee213>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_gate_node<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1a4c2cea51ac1610ae83c106a0a03781f1>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_work<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1ad69f9d8ce5231c4339eb98e4966904cc>`(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` node_t, Args&&... func_args);
	};

	// direct descendants

	class :ref:`DrawByLayer<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_by_layer>`;
	class :ref:`FillLayerByNextLayerNodes<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_fill_layer_by_next_layer_nodes>`;
	class :ref:`GetUsedQubits<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_get_used_qubits>`;
.. _details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

node handle

Methods
-------

.. index:: pair: function; handle_measure_node
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1ad039a9c5d1e99f73ce341480a6116074:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_measure_node(Args&&... func_args) = 0

handle measure node

.. index:: pair: function; handle_reset_node
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1a54be32b87f0591523496103f4d8ee213:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_reset_node(Args&&... func_args) = 0

handle reset node

.. index:: pair: function; handle_gate_node
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1a4c2cea51ac1610ae83c106a0a03781f1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_gate_node(Args&&... func_args) = 0

handle gate node

.. index:: pair: function; handle_work
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_abstract_handle_nodes_1ad69f9d8ce5231c4339eb98e4966904cc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_work(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` node_t, Args&&... func_args)

handle work run

