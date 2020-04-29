.. index:: pair: class; QPanda::AbstractHandleNodes
.. _doxid-class_q_panda_1_1_abstract_handle_nodes:

template class QPanda::AbstractHandleNodes
==========================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

node handle :ref:`More...<details-class_q_panda_1_1_abstract_handle_nodes>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	template <typename... Args>
	class AbstractHandleNodes
	{
	public:
		// methods
	
		virtual void :ref:`handle_measure_node<doxid-class_q_panda_1_1_abstract_handle_nodes_1a80b30eaad05c74b9f33f504c826ac1e5>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_reset_node<doxid-class_q_panda_1_1_abstract_handle_nodes_1a294e7a69d1b81bcf5f2e037949d436c8>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_gate_node<doxid-class_q_panda_1_1_abstract_handle_nodes_1ac265826cf46fadc107a5137f5fec31a1>`(Args&&... func_args) = 0;
		virtual void :ref:`handle_work<doxid-class_q_panda_1_1_abstract_handle_nodes_1a66b6cbe7db19cf9248f89cbdae98a690>`(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` node_t, Args&&... func_args);
	};

	// direct descendants

	class :ref:`DrawByLayer<doxid-class_q_panda_1_1_draw_by_layer>`;
	class :ref:`FillLayerByNextLayerNodes<doxid-class_q_panda_1_1_fill_layer_by_next_layer_nodes>`;
	class :ref:`GetUsedQubits<doxid-class_q_panda_1_1_get_used_qubits>`;
	class :ref:`TryToMergeTimeSequence<doxid-class_q_panda_1_1_try_to_merge_time_sequence>`;
.. _details-class_q_panda_1_1_abstract_handle_nodes:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

node handle

Methods
-------

.. index:: pair: function; handle_measure_node
.. _doxid-class_q_panda_1_1_abstract_handle_nodes_1a80b30eaad05c74b9f33f504c826ac1e5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_measure_node(Args&&... func_args) = 0

handle measure node

.. index:: pair: function; handle_reset_node
.. _doxid-class_q_panda_1_1_abstract_handle_nodes_1a294e7a69d1b81bcf5f2e037949d436c8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_reset_node(Args&&... func_args) = 0

handle reset node

.. index:: pair: function; handle_gate_node
.. _doxid-class_q_panda_1_1_abstract_handle_nodes_1ac265826cf46fadc107a5137f5fec31a1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_gate_node(Args&&... func_args) = 0

handle gate node

.. index:: pair: function; handle_work
.. _doxid-class_q_panda_1_1_abstract_handle_nodes_1a66b6cbe7db19cf9248f89cbdae98a690:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void handle_work(const :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` node_t, Args&&... func_args)

handle work run

