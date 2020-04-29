.. index:: pair: class; VerticeMatrix
.. _doxid-class_vertice_matrix:

class VerticeMatrix
===================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorNode.h>
	
	class VerticeMatrix
	{
	public:
		// construction
	
		:target:`VerticeMatrix<doxid-class_vertice_matrix_1acf31a42f92ad9f24fbe445d0b2f8f442>`();
		:target:`VerticeMatrix<doxid-class_vertice_matrix_1af88bfcdaa4a0e4e00a9ad51a2b4cf349>`(const VerticeMatrix&);

		// methods
	
		VerticeMatrix :target:`operator =<doxid-class_vertice_matrix_1a5079aaa12520fb70692efb3c5129670a>` (const VerticeMatrix&);
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getQubitCount<doxid-class_vertice_matrix_1a3c8845c2a54d7a4909c7fe3179d6d74c>`() const;
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getVerticeCount<doxid-class_vertice_matrix_1a2e00fae27feb65ff8704ccf500c3fd64>`() const;
		void :target:`subVerticeCount<doxid-class_vertice_matrix_1ad8295d7c58c2eaf495198d8a9c1b2bfa>`();
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`addVertice<doxid-class_vertice_matrix_1a6f0f81a1493a1050db52ea42cc1c37a7>`(:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`);
	
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`addVertice<doxid-class_vertice_matrix_1ac662cb5d0d7b4a06427bd2772ad74eac>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`addVertice<doxid-class_vertice_matrix_1a1d2ca3595f39ab3f4bc3f68e99dc488b>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`Vertice<doxid-class_vertice>`&
			);
	
		int :target:`getVerticeValue<doxid-class_vertice_matrix_1a4a35ba0cd088d4160d82ca68ecd43384>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getEmptyVertice<doxid-class_vertice_matrix_1a10bd89beb81549ff08221279efff9092>`();
	
		void :target:`setVerticeValue<doxid-class_vertice_matrix_1a7244c69049d1031d8f1f536972c154c5>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			int
			);
	
		void :target:`initVerticeMatrix<doxid-class_vertice_matrix_1a43d73f10975eed15bb6493e78da4ea81>`(:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`);
	
		map<:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`Vertice<doxid-class_vertice>`>::iterator :target:`deleteVertice<doxid-class_vertice_matrix_1a597e289b1df8916e154ad53a53bd3088>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getQubitVerticeLastID<doxid-class_vertice_matrix_1a93c33edc6336d5cecdf57213e3ec5034>`(:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`);
	
		vector<:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`>& :target:`getContectEdge<doxid-class_vertice_matrix_1a0fb10e2d370a97b628a299d2a02ac8d9>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		vertice_matrix_t::iterator :target:`begin<doxid-class_vertice_matrix_1aa59b2d24d974e17b37bf8097d7f5cabd>`();
		vertice_matrix_t::iterator :target:`end<doxid-class_vertice_matrix_1a9205e5121dcd7bd8ff2f4599e3b4eb55>`();
		vertice_matrix_t::iterator :target:`getQubitMapIter<doxid-class_vertice_matrix_1a3267715b0641de47951cd2bed2eae73b>`(:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit);
		vertice_map_t::iterator :target:`getQubitMapIterBegin<doxid-class_vertice_matrix_1ad5f0d814570cd034598a9d22c99e305e>`(:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit);
		vertice_map_t::iterator :target:`getQubitMapIterEnd<doxid-class_vertice_matrix_1a0b99eea45cd0e7d9d4e2528bab9cd38f>`(:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit);
	
		vertice_map_t::iterator :target:`getVertice<doxid-class_vertice_matrix_1a94f36c50df40691f487f7b7dc37f3470>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		void :target:`addContectEdge<doxid-class_vertice_matrix_1a99d0bb9bcc365954ca549f0fafbb1dad>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		void :target:`changeContectEdge<doxid-class_vertice_matrix_1a37cd2023085b113ab495a1ce7f68ed68>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		void :target:`deleteContectEdge<doxid-class_vertice_matrix_1a18f1fdd9e13a28864201a2ed40b16b81>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		void :target:`clearVertice<doxid-class_vertice_matrix_1a799b9f8bc0b68a88bdfc7597e3bbce0b>`();
		bool :target:`isEmpty<doxid-class_vertice_matrix_1a43c27f7587c613517e8b4cf8191734e8>`();
		void :target:`clear<doxid-class_vertice_matrix_1a400b3f0795e65905c44eef1609f29193>`();
	};
