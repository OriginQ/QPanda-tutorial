.. index:: pair: class; AbstractComplexTensor
.. _doxid-class_abstract_complex_tensor:

class AbstractComplexTensor
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Tensor.h>
	
	class AbstractComplexTensor
	{
	public:
		// methods
	
		virtual size_t :target:`getRank<doxid-class_abstract_complex_tensor_1a1232370371487bbd0f2922240de8e343>`() const = 0;
		virtual size_t :target:`getMaxRank<doxid-class_abstract_complex_tensor_1a7050c9d008fc2ef97eae0ed3b200f754>`() const = 0;
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` :target:`getElem<doxid-class_abstract_complex_tensor_1ad41d90639278a437624207fb6eb79ede>`(size_t num) = 0;
		virtual void :target:`dimIncrement<doxid-class_abstract_complex_tensor_1ab7c8e8ea757d298026a3c4693588b84a>`(size_t) = 0;
	
		virtual void :target:`getSubTensor<doxid-class_abstract_complex_tensor_1ae440f33fbbd7f8fce6ee40d926bdf258>`(
			size_t num,
			int value
			) = 0;
	
		virtual void :target:`dimDecrement<doxid-class_abstract_complex_tensor_1a6c68852212a2afef797afe6f531b9055>`(size_t num) = 0;
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`* :target:`getTensor<doxid-class_abstract_complex_tensor_1a51d01298304e9ccf97d3b2b290187e46>`() = 0;
	
		virtual void :target:`mul<doxid-class_abstract_complex_tensor_1a3d9432e3c63db33bd0c8d4b117752919>`(
			:ref:`ComplexTensor<doxid-class_complex_tensor>`& other,
			size_t* mask_array
			) = 0;
	
		virtual :ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>` :target:`getBackend<doxid-class_abstract_complex_tensor_1a84d0c5c0b8baa52ff132757aafd075b5>`() = 0;
	};

	// direct descendants

	class :ref:`ComplexTensor<doxid-class_complex_tensor>`;
	class :ref:`CPUComplexTensor<doxid-class_c_p_u_complex_tensor>`;
