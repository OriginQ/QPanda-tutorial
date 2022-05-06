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
	
		:target:`Edge<doxid-class_edge_1a89417f404d801d00bb87046c1635c172>`(
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit_count,
			:ref:`ComplexTensor<doxid-class_complex_tensor>`& tensor,
			std::vector<std::pair<:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`>>& contect_vertice
			);

		// methods
	
		void :target:`earseContectVertice<doxid-class_edge_1a7a0c448063e3da971515c4836e22e483>`(
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
			size_t num
			);
	
		:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getQubitCount<doxid-class_edge_1a8923b03ded966a25ed978b23bda3eda8>`() const;
		bool :target:`mergeEdge<doxid-class_edge_1aac507ec09278984acd1c1e310f3301c0>`(Edge& edge);
	
		void :target:`dimDecrementbyValue<doxid-class_edge_1a1985ae5e4af1cd324cd8afc379a2d070>`(
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` num,
			int value
			);
	
		void :target:`dimDecrement<doxid-class_edge_1a6c0eb035e38fb9797d6bbaf82d7846d5>`(
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` num
			);
	
		void :target:`dimIncrementByEdge<doxid-class_edge_1a95b113a49138b9c41cfca3389f0f9d6d>`(Edge& edge);
	
		void :target:`getEdgeMap<doxid-class_edge_1a4ae0c3303634e528292af50651c044da>`(
			Edge& edge,
			size_t* mask
			);
	
		void :target:`mul<doxid-class_edge_1ac7cf7d9f6e7e0235eadf9d157de33fc2>`(
			Edge& edge,
			size_t* mask_array
			);
	
		int :target:`getRank<doxid-class_edge_1acd311f2212b3467ef60210edadc4664b>`() const;
		:ref:`ComplexTensor<doxid-class_complex_tensor>` :target:`getComplexTensor<doxid-class_edge_1a5ee7e6b47fd6e1e95e9c7a87d7b4006d>`() const;
		:ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` :target:`getElem<doxid-class_edge_1a30211f42fd630eb53442f111e9aa0aa2>`(:ref:`VerticeMatrix<doxid-class_vertice_matrix>`& vertice);
		void :target:`setComplexTensor<doxid-class_edge_1a77448af71af78da6d5f036f966930634>`(:ref:`ComplexTensor<doxid-class_complex_tensor>`& tensor);
		void :target:`getContectVertice<doxid-class_edge_1aba8b05ef7e1dfac5c6cd18268aa1614c>`(std::vector<std::pair<:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`>>& connect_vertice) const;
		void :target:`setContectVerticeVector<doxid-class_edge_1ae00966da6e5153385c28f236b6747af8>`(const :ref:`qubit_vector_t<doxid-_tensor_node_8h_1af892fbee44ef3346256861d11383f4a1>`& contect_vertice);
	
		void :target:`setContectVertice<doxid-class_edge_1af67cc0d2fdccad25ecc2a864181b2cda>`(
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit,
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` src_num,
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` des_num
			);
	};
