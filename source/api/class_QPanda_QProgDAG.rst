.. index:: pair: class; QPanda::QProgDAG
.. _doxid-class_q_panda_1_1_q_prog_d_a_g:

class QPanda::QProgDAG
======================

.. toctree::
	:hidden:

	struct_QPanda_QProgDAG_NodeInfo.rst

Overview
~~~~~~~~

transform :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to DAG(directed acyclic graph) :ref:`More...<details-class_q_panda_1_1_q_prog_d_a_g>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	class QProgDAG
	{
	public:
		// typedefs
	
		typedef std::map<size_t, :ref:`NodeInfo<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info>`> :target:`vertices_map<doxid-class_q_panda_1_1_q_prog_d_a_g_1a579150f8d7695b6cb39bf8d4da0adc6f>`;

		// structs
	
		struct :ref:`NodeInfo<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info>`;

		// fields
	
		std::vector<size_t> :target:`m_qubit_vec<doxid-class_q_panda_1_1_q_prog_d_a_g_1ac985b30e204dc7ee95e05c200b138a57>`;

		// methods
	
		void :ref:`getTopologincalSequence<doxid-class_q_panda_1_1_q_prog_d_a_g_1acbec7ff5d8d514245a91c78d5a8fd4ef>`(:ref:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`&);
		size_t :ref:`add_vertex<doxid-class_q_panda_1_1_q_prog_d_a_g_1a45034b99564aef20cbb00ff5bdd97cb2>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node);
		size_t :ref:`add_vertex<doxid-class_q_panda_1_1_q_prog_d_a_g_1afa4c6c76f1ef865ecd2f3090f5885e9b>`(const :ref:`NodeInfo<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info>`& node_info);
		void :ref:`add_edge<doxid-class_q_panda_1_1_q_prog_d_a_g_1a41a42f215bc33eed2f948a7d19f76e66>`(size_t, size_t);
		void :ref:`get_adjacency_matrix<doxid-class_q_panda_1_1_q_prog_d_a_g_1a9a578c8553bb2d9d2f15efb6a4ce26a4>`(const :ref:`vertices_map<doxid-class_q_panda_1_1_q_prog_d_a_g_1a579150f8d7695b6cb39bf8d4da0adc6f>`&, :ref:`AdjacencyMatrix<doxid-namespace_q_panda_1a97e0cecb440ec41f5e549157287bc9c1>`&);
		:ref:`SequenceNode<doxid-struct_q_panda_1_1_sequence_node>` :ref:`construct_sequence_node<doxid-class_q_panda_1_1_q_prog_d_a_g_1a83d8e70402f4e46a5fe0f8b16868226d>`(size_t);
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :ref:`get_vertex<doxid-class_q_panda_1_1_q_prog_d_a_g_1a5bcd579ae8bd8d7e0a4971a6c7a18d36>`(size_t) const;
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`get_vertex_nodeIter<doxid-class_q_panda_1_1_q_prog_d_a_g_1aaf747b806c4f199e1486ae3e4483fe19>`(size_t) const;
		void :ref:`add_qubit_map<doxid-class_q_panda_1_1_q_prog_d_a_g_1ad364e511f4284b7e6256a48d8c8ba5f9>`(size_t, size_t);
		bool :target:`is_connected_graph<doxid-class_q_panda_1_1_q_prog_d_a_g_1a4baabd6245c36afcfc7c75cebfe31c40>`();
	};
.. _details-class_q_panda_1_1_q_prog_d_a_g:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

transform :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to DAG(directed acyclic graph)

transform :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to DAG

Methods
-------

.. index:: pair: function; getTopologincalSequence
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1acbec7ff5d8d514245a91c78d5a8fd4ef:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void getTopologincalSequence(:ref:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`&)

get TopologincalSequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- TopologicalSequence

		- 



.. rubric:: Returns:

void

.. index:: pair: function; add_vertex
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1a45034b99564aef20cbb00ff5bdd97cb2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t add_vertex(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node)

add vertex



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- quantum node



.. rubric:: Returns:

size_t vertex num

.. index:: pair: function; add_vertex
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1afa4c6c76f1ef865ecd2f3090f5885e9b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t add_vertex(const :ref:`NodeInfo<doxid-struct_q_panda_1_1_q_prog_d_a_g_1_1_node_info>`& node_info)

add vertex



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node_info

		- 



.. rubric:: Returns:

size_t vertex num

.. index:: pair: function; add_edge
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1a41a42f215bc33eed2f948a7d19f76e66:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_edge(size_t, size_t)

add edge



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- vertex num

	*
		- size_t

		- vertex num



.. rubric:: Returns:

void

.. index:: pair: function; get_adjacency_matrix
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1a9a578c8553bb2d9d2f15efb6a4ce26a4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void get_adjacency_matrix(const :ref:`vertices_map<doxid-class_q_panda_1_1_q_prog_d_a_g_1a579150f8d7695b6cb39bf8d4da0adc6f>`&, :ref:`AdjacencyMatrix<doxid-namespace_q_panda_1a97e0cecb440ec41f5e549157287bc9c1>`&)

get adjacency_matrix



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- vertices_map&

		- 

	*
		- AdjacencyMatrix&

		- 



.. rubric:: Returns:

void

.. index:: pair: function; construct_sequence_node
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1a83d8e70402f4e46a5fe0f8b16868226d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`SequenceNode<doxid-struct_q_panda_1_1_sequence_node>` construct_sequence_node(size_t)

construct sequence node



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- vertex num



.. rubric:: Returns:

:ref:`QPanda::SequenceNode <doxid-struct_q_panda_1_1_sequence_node>`

.. index:: pair: function; get_vertex
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1a5bcd579ae8bd8d7e0a4971a6c7a18d36:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> get_vertex(size_t) const

get vertex by vertex num



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- vertex num



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> qnode

.. index:: pair: function; get_vertex_nodeIter
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1aaf747b806c4f199e1486ae3e4483fe19:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` get_vertex_nodeIter(size_t) const

get vertex nodeIter by vertex num



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- vertex num



.. rubric:: Returns:

:ref:`QPanda::NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; add_qubit_map
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1ad364e511f4284b7e6256a48d8c8ba5f9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_qubit_map(size_t, size_t)

add qubit map



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit

	*
		- size_t

		- vertex num



.. rubric:: Returns:

void

