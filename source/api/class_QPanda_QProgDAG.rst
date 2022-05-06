.. index:: pair: class; QPanda::QProgDAG
.. _doxid-class_q_panda_1_1_q_prog_d_a_g:

class QPanda::QProgDAG
======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

transform :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to DAG(directed acyclic graph) :ref:`More...<details-class_q_panda_1_1_q_prog_d_a_g>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDAG.h>
	
	class QProgDAG
	{
	public:
		// fields
	
		std::map<uint32_t, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> :target:`m_qubits<doxid-class_q_panda_1_1_q_prog_d_a_g_1abe2f04e013026c79a77c44264cfa5b9f>`;

		// methods
	
		void :ref:`add_vertex<doxid-class_q_panda_1_1_q_prog_d_a_g_1a3dae8d6e1582cec3b3aefdbbe65583de>`(std::shared_ptr<:ref:`QProgDAGNode<doxid-struct_q_panda_1_1_q_prog_d_a_g_node>`> n, :ref:`DAGNodeType<doxid-namespace_q_panda_1ab003414a5253d4a751cb89f052573337>` type);
		void :ref:`get_adjacency_matrix<doxid-class_q_panda_1_1_q_prog_d_a_g_1acc3078ef02bcb756a459fc1f1f17f0ca>`(:ref:`AdjacencyMatrix<doxid-namespace_q_panda_1a97e0cecb440ec41f5e549157287bc9c1>`& matrix);
		const :ref:`QProgDAGVertex<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex>`& :ref:`get_vertex<doxid-class_q_panda_1_1_q_prog_d_a_g_1a2617344d69a4c577f9663363f8ab9db1>`(const size_t vertice_num) const;
		bool :target:`is_connected_graph<doxid-class_q_panda_1_1_q_prog_d_a_g_1a4baabd6245c36afcfc7c75cebfe31c40>`();
		:ref:`TopologSequence<doxid-class_q_panda_1_1_topolog_sequence>`<:ref:`DAGSeqNode<doxid-struct_q_panda_1_1_d_a_g_seq_node>`> :target:`build_topo_sequence<doxid-class_q_panda_1_1_q_prog_d_a_g_1a6cdbaad50fb8c2f5433a8ed194792053>`();
		std::set<:ref:`QProgDAGEdge<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge>`> :target:`get_edges<doxid-class_q_panda_1_1_q_prog_d_a_g_1aeb5ec4051aea4265917239ddd999aa0b>`() const;
		void :target:`remove_edge<doxid-class_q_panda_1_1_q_prog_d_a_g_1a323c8ae43adf27a7afed8c1662c9592b>`(const :ref:`QProgDAGEdge<doxid-struct_q_panda_1_1_q_prog_d_a_g_edge>`& e);
		const std::vector<:ref:`QProgDAGVertex<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex>`>& :target:`get_vertex_c<doxid-class_q_panda_1_1_q_prog_d_a_g_1aa012b0e6c510577c4a45a6ce396d9e1f>`() const;
		std::vector<:ref:`QProgDAGVertex<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex>`>& :target:`get_vertex<doxid-class_q_panda_1_1_q_prog_d_a_g_1a90ad43dfdeba2218981522c8de14ead6>`();
		const auto& :target:`get_qubit_vertices_map<doxid-class_q_panda_1_1_q_prog_d_a_g_1ae794e61ce6cca5d12488e16240a018f2>`() const;
		std::shared_ptr<:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`> :target:`dag_to_qprog<doxid-class_q_panda_1_1_q_prog_d_a_g_1a4e0ab9fa492d7434279f72c3dd034790>`();
	};
.. _details-class_q_panda_1_1_q_prog_d_a_g:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

transform :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to DAG(directed acyclic graph)

transform :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` to DAG

Methods
-------

.. index:: pair: function; add_vertex
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1a3dae8d6e1582cec3b3aefdbbe65583de:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void add_vertex(std::shared_ptr<:ref:`QProgDAGNode<doxid-struct_q_panda_1_1_q_prog_d_a_g_node>`> n, :ref:`DAGNodeType<doxid-namespace_q_panda_1ab003414a5253d4a751cb89f052573337>` type)

add vertex



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node_info

		- 



.. rubric:: Returns:

size_t vertex num

.. index:: pair: function; get_adjacency_matrix
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1acc3078ef02bcb756a459fc1f1f17f0ca:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void get_adjacency_matrix(:ref:`AdjacencyMatrix<doxid-namespace_q_panda_1a97e0cecb440ec41f5e549157287bc9c1>`& matrix)

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

.. index:: pair: function; get_vertex
.. _doxid-class_q_panda_1_1_q_prog_d_a_g_1a2617344d69a4c577f9663363f8ab9db1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`QProgDAGVertex<doxid-class_q_panda_1_1_q_prog_d_a_g_vertex>`& get_vertex(const size_t vertice_num) const

get vertex by vertex num



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- vertex num



.. rubric:: Returns:

std::shared_ptr<QPanda::QNode> qnode

