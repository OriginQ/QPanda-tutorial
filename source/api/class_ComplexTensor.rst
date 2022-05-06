.. index:: pair: class; ComplexTensor
.. _doxid-class_complex_tensor:

class ComplexTensor
===================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Tensor.h>
	
	class ComplexTensor: public :ref:`AbstractComplexTensor<doxid-class_abstract_complex_tensor>`
	{
	public:
		// construction
	
		:target:`ComplexTensor<doxid-class_complex_tensor_1a4102343253592131da3b25a95599ffd9>`(std::shared_ptr<:ref:`AbstractComplexTensor<doxid-class_abstract_complex_tensor>`> tensor);
		:target:`ComplexTensor<doxid-class_complex_tensor_1a69fb4b246fcaaa95832a130d799cb6eb>`(const ComplexTensor& old);
	
		:target:`ComplexTensor<doxid-class_complex_tensor_1afe010df660a7c521f588478ebab08834>`(
			:ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>` backend,
			size_t rank,
			:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& tensor,
			size_t max_rank
			);
	
		:target:`ComplexTensor<doxid-class_complex_tensor_1a1ae78280c2157ec1fb3910593d17d895>`(
			:ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>` backend,
			size_t rank,
			:ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`* tensor,
			size_t max_rank
			);

		// methods
	
		virtual size_t :target:`getRank<doxid-class_complex_tensor_1a19720224916411ac7616e4a864be8d7a>`() const;
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` :target:`getElem<doxid-class_complex_tensor_1aee47e59b56fd104e1e3964d3f627ac67>`(size_t num);
		virtual void :target:`dimIncrement<doxid-class_complex_tensor_1a6e37d3fd0d138a4961a666ea6c02b626>`(size_t num);
	
		virtual void :target:`getSubTensor<doxid-class_complex_tensor_1afb53d2d0c22200c4e278637d88e38665>`(
			size_t num,
			int value
			);
	
		virtual void :target:`dimDecrement<doxid-class_complex_tensor_1a0203214955abe29618de412bb2afd708>`(size_t num);
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`* :target:`getTensor<doxid-class_complex_tensor_1a9495258f0281295fbf75f4ea51399421>`();
	
		virtual void :target:`mul<doxid-class_complex_tensor_1a510cc3f4c534c270c7757ef1fa91f818>`(
			ComplexTensor& other,
			size_t* mask_array
			);
	
		virtual size_t :target:`getMaxRank<doxid-class_complex_tensor_1a4f464cbea4115f9946eeadc065db60db>`() const;
		virtual :ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>` :target:`getBackend<doxid-class_complex_tensor_1a460080093f4ac71ae87a1ca247cc7a69>`();
		ComplexTensor& :target:`operator =<doxid-class_complex_tensor_1a18c31615a46e192df521f600b1299209>` (const ComplexTensor& old);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual size_t :ref:`getRank<doxid-class_abstract_complex_tensor_1a1232370371487bbd0f2922240de8e343>`() const = 0;
		virtual size_t :ref:`getMaxRank<doxid-class_abstract_complex_tensor_1a7050c9d008fc2ef97eae0ed3b200f754>`() const = 0;
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` :ref:`getElem<doxid-class_abstract_complex_tensor_1ad41d90639278a437624207fb6eb79ede>`(size_t num) = 0;
		virtual void :ref:`dimIncrement<doxid-class_abstract_complex_tensor_1ab7c8e8ea757d298026a3c4693588b84a>`(size_t) = 0;
		virtual void :ref:`getSubTensor<doxid-class_abstract_complex_tensor_1ae440f33fbbd7f8fce6ee40d926bdf258>`(size_t num, int value) = 0;
		virtual void :ref:`dimDecrement<doxid-class_abstract_complex_tensor_1a6c68852212a2afef797afe6f531b9055>`(size_t num) = 0;
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`* :ref:`getTensor<doxid-class_abstract_complex_tensor_1a51d01298304e9ccf97d3b2b290187e46>`() = 0;
		virtual void :ref:`mul<doxid-class_abstract_complex_tensor_1a3d9432e3c63db33bd0c8d4b117752919>`(ComplexTensor& other, size_t* mask_array) = 0;
		virtual :ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>` :ref:`getBackend<doxid-class_abstract_complex_tensor_1a84d0c5c0b8baa52ff132757aafd075b5>`() = 0;

