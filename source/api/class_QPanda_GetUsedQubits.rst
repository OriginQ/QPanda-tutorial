.. index:: pair: class; QPanda::GetUsedQubits
.. _doxid-class_q_panda_1_1_get_used_qubits:

class QPanda::GetUsedQubits
===========================

.. toctree::
	:hidden:

get all used qubits


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class GetUsedQubits: public :ref:`QPanda::AbstractHandleNodes<doxid-class_q_panda_1_1_abstract_handle_nodes>`
	{
	public:
		// construction
	
		:target:`GetUsedQubits<doxid-class_q_panda_1_1_get_used_qubits_1a760353ddb2556b899810b9b7726add38>`(
			:ref:`DrawPicture<doxid-class_q_panda_1_1_draw_picture>`& parent,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec
			);

		// methods
	
		void :target:`handle_measure_node<doxid-class_q_panda_1_1_get_used_qubits_1a03da86571b4d7210ef3f9fda21286f52>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
		void :target:`handle_reset_node<doxid-class_q_panda_1_1_get_used_qubits_1a02d4f33c32046f8bb9d1d806730f578f>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
		void :target:`handle_gate_node<doxid-class_q_panda_1_1_get_used_qubits_1a1ec697713e4af31261f7e073d6f4d653>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>& p_node);
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

