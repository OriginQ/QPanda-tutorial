.. index:: pair: struct; QubitVertice
.. _doxid-struct_qubit_vertice:

struct QubitVertice
===================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorEngine.h>
	
	struct QubitVertice
	{
		// fields
	
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`m_qubit_id<doxid-struct_qubit_vertice_1ae0d18812cf57dce50bbf6ba7bbd691c4>`;
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`m_num<doxid-struct_qubit_vertice_1a99fc468807308a60d38d237040b6b031>`;
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`m_max<doxid-struct_qubit_vertice_1a24fc36edfff4c75ab1c60be15cd2d8eb>`;
		int :target:`m_count<doxid-struct_qubit_vertice_1a9e53bfa83dfdcc6302489b6dca6cc4b6>`;

		// construction
	
		:target:`QubitVertice<doxid-struct_qubit_vertice_1a1f3adfc34c2c974f8b7284783c145b79>`(const QubitVertice& old);
		:target:`QubitVertice<doxid-struct_qubit_vertice_1a654897ded0bbe7362f54191622c2593c>`();

		// methods
	
		QubitVertice :target:`operator =<doxid-struct_qubit_vertice_1abddf22be226685599d7618a8982c22aa>` (const QubitVertice& old);
	};
