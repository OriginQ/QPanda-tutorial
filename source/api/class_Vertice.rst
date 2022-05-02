.. index:: pair: class; Vertice
.. _doxid-class_vertice:

class Vertice
=============

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorNode.h>
	
	class Vertice
	{
	public:
		// construction
	
		:target:`Vertice<doxid-class_vertice_1a9dd7cf987cddf248b9d4e3d31bf8822b>`();
	
		:target:`Vertice<doxid-class_vertice_1a0e0a48082836b4b56e7f1a078628f934>`(
			int value,
			std::vector<:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`>& contect_edge
			);

		// methods
	
		std::vector<:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`>& :target:`getContectEdge<doxid-class_vertice_1a7f5580f83c313e198972239979d86fa2>`();
		void :target:`addContectEdge<doxid-class_vertice_1a0c3fb5627f9eb82e94685170c3083f91>`(:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`);
	
		void :target:`setContectEdge<doxid-class_vertice_1a28d0375a1a278618e2015e5c3c57e57a>`(
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		void :target:`setContectEdgebyID<doxid-class_vertice_1a1e4b0a3724b9332fb4ee2f702272934c>`(
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` id,
			:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` value
			);
	
		void :target:`deleteContectEdge<doxid-class_vertice_1a153a8354cf01a45cbbfb7f73f171aa2e>`(:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`);
		int :target:`getValue<doxid-class_vertice_1a077fa14a46298b4c32fa55ca7a366a7a>`() const;
		void :target:`setValue<doxid-class_vertice_1a26ac84d5a876d84092ac54da522676ce>`(int);
		void :target:`setNum<doxid-class_vertice_1a5538403f9e2852d0816f9f35d1e99a4d>`(size_t num);
		size_t :target:`getNum<doxid-class_vertice_1a0d1596c7c0a2d761f7319ab6641f3da9>`();
	};
