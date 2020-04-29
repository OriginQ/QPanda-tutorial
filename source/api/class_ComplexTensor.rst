.. index:: pair: class; ComplexTensor
.. _doxid-class_complex_tensor:

class ComplexTensor
===================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorNode.h>
	
	class ComplexTensor
	{
	public:
		// construction
	
		:target:`ComplexTensor<doxid-class_complex_tensor_1a69fb4b246fcaaa95832a130d799cb6eb>`(const ComplexTensor& old);
	
		:target:`ComplexTensor<doxid-class_complex_tensor_1a4c0a8ca9cb767457fd4a9790b4323a63>`(
			int rank,
			:ref:`qstate_t<doxid-_tensor_node_8h_1a3d31874fe5c5e054c8c3eb07f19aa84b>`& tensor
			);
	
		:target:`ComplexTensor<doxid-class_complex_tensor_1a96a3175b6fda6a47ebfe424cef09d48d>`(
			int rank,
			:ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>`* tensor
			);

		// methods
	
		int :target:`getRank<doxid-class_complex_tensor_1a5e15272000a26e1e72e5aebd9dd7af1e>`() const;
		:ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>` :target:`getElem<doxid-class_complex_tensor_1ac88b552516b461e91103d9c4d0e7c24e>`(size_t num);
	
		void :target:`mulElem<doxid-class_complex_tensor_1ad180442c81ab2cefb1689bc7e86e0114>`(
			size_t,
			:ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>`
			);
	
		void :target:`dimIncrement<doxid-class_complex_tensor_1aedc4602c6528f4ab96c8810dc384563c>`(size_t);
	
		void :target:`getSubTensor<doxid-class_complex_tensor_1a08c3680d1d2d77908737885382a477df>`(
			size_t num,
			int value
			);
	
		void :target:`dimDecrement<doxid-class_complex_tensor_1a6ec283aec1f2e0da983b5e4549d8438e>`(size_t num);
	
		void :target:`swap<doxid-class_complex_tensor_1a13e87e9609712b8b7bad6a644fec9648>`(
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`,
			:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`
			);
	
		:ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>`* :target:`get_tensor<doxid-class_complex_tensor_1a83c5389a5326dec8db4644ea27cacfe3>`();
		ComplexTensor& :target:`operator *<doxid-class_complex_tensor_1af32fdceba5eb041afd595278382ae040>` (ComplexTensor&);
		ComplexTensor& :target:`operator =<doxid-class_complex_tensor_1a5b319b802715f8ccf49880dce1a7b22f>` (const ComplexTensor&);
	};
