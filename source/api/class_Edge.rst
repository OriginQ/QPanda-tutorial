.. index:: pair: class; Edge
.. _doxid-class_edge:

class Edge
==========

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorNode.h>
	
	class Edge
	{
	public:
		// construction
	
		:target:`Edge<doxid-class_edge_1a8b074e6457229c6cff14470afe2e7740>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit_count,
			:ref:`ComplexTensor<doxid-class_complex_tensor>`& tensor,
			vector<pair<:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`>>& contect_vertice
			);
	
		:target:`Edge<doxid-class_edge_1ad7fae93aa7a54ed1236d7145c92c8d16>`(const Edge& old);

		// methods
	
		void :target:`earseContectVertice<doxid-class_edge_1a7a0c448063e3da971515c4836e22e483>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
			size_t num
			);
	
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getQubitCount<doxid-class_edge_1a8923b03ded966a25ed978b23bda3eda8>`() const;
		void :target:`premultiplication<doxid-class_edge_1a00c120825801f7fd188d3994a80c0300>`(Edge&);
		bool :target:`mergeEdge<doxid-class_edge_1a43ae69f59fbd09b34ddfbf2084738b46>`(Edge&);
	
		void :target:`dimDecrementbyValue<doxid-class_edge_1aa02d71f3b2dfc988fcce6c92e1ad2f4a>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			int value
			);
	
		void :target:`dimDecrement<doxid-class_edge_1a6c0eb035e38fb9797d6bbaf82d7846d5>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` num
			);
	
		void :target:`dimIncrementByEdge<doxid-class_edge_1a7152ab83003af77324fa69da1fd1144a>`(Edge&);
	
		void :target:`getEdgeMap<doxid-class_edge_1aa1a989e1c3c6b9f5f6afd3cffe385287>`(
			Edge&,
			size_t*
			);
	
		void :target:`mul<doxid-class_edge_1a2c55e21e4a42191ccd319d968c24294f>`(
			Edge&,
			size_t*
			);
	
		void :target:`swapByEdge<doxid-class_edge_1a0e8a076e0d964eb49a48b39357ce1507>`(Edge&);
		int :target:`getRank<doxid-class_edge_1acd311f2212b3467ef60210edadc4664b>`() const;
		:ref:`ComplexTensor<doxid-class_complex_tensor>` :target:`getComplexTensor<doxid-class_edge_1a5ee7e6b47fd6e1e95e9c7a87d7b4006d>`() const;
		:ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>` :target:`getElem<doxid-class_edge_1a30211f42fd630eb53442f111e9aa0aa2>`(:ref:`VerticeMatrix<doxid-class_vertice_matrix>`& vertice);
		void :target:`setComplexTensor<doxid-class_edge_1aa059907e44a66a7d990a53f750554ccd>`(:ref:`ComplexTensor<doxid-class_complex_tensor>`&);
		vector<pair<:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`>> :target:`getContectVertice<doxid-class_edge_1aa57bb423654f87f434532fdfb2d64f6f>`() const;
		void :target:`setContectVerticeVector<doxid-class_edge_1ac6302a6e87451ca58c77b8f00dccd3ae>`(const :ref:`qubit_vector_t<doxid-_tensor_node_8h_1aac19cd0cea4e3958f3c9339902f4addc>`&);
	
		void :target:`setContectVertice<doxid-class_edge_1af67cc0d2fdccad25ecc2a864181b2cda>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` src_num,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` des_num
			);
	};
