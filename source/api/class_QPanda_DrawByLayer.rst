.. index:: pair: class; QPanda::DrawByLayer
.. _doxid-class_q_panda_1_1_draw_by_layer:

class QPanda::DrawByLayer
=========================

.. toctree::
	:hidden:

draw layer nodes


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class DrawByLayer: public :ref:`QPanda::AbstractHandleNodes<doxid-class_q_panda_1_1_abstract_handle_nodes>`
	{
	public:
		// construction
	
		:target:`DrawByLayer<doxid-class_q_panda_1_1_draw_by_layer_1a67d351a4a352f750e9d8c7ca56ae4fac>`(:ref:`DrawPicture<doxid-class_q_panda_1_1_draw_picture>`& parent);

		// methods
	
		void :target:`handle_measure_node<doxid-class_q_panda_1_1_draw_by_layer_1a93bf4ee1983dc7806db738e0357bd73b>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
		void :target:`handle_reset_node<doxid-class_q_panda_1_1_draw_by_layer_1a554c46d91547f8cc7cbad8b8d3ab48d7>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
		void :target:`handle_gate_node<doxid-class_q_panda_1_1_draw_by_layer_1ae0c3945ef804901fa6557bd46c71ecf8>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
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

