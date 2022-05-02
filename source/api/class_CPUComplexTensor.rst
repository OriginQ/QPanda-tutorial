.. index:: pair: class; CPUComplexTensor
.. _doxid-class_c_p_u_complex_tensor:

class CPUComplexTensor
======================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Tensor.h>
	
	class CPUComplexTensor: public :ref:`AbstractComplexTensor<doxid-class_abstract_complex_tensor>`
	{
	public:
		// construction
	
		:target:`CPUComplexTensor<doxid-class_c_p_u_complex_tensor_1adfa6a52ee919124c5aef44ee999add59>`(const CPUComplexTensor& old);
	
		:target:`CPUComplexTensor<doxid-class_c_p_u_complex_tensor_1acda89b73dcc98310229dc2046072b9ed>`(
			size_t rank,
			:ref:`qstate_t<doxid-_tensor_8h_1ad438ac446c53cb863102efc403f33f84>`& tensor,
			size_t max_rank
			);
	
		:target:`CPUComplexTensor<doxid-class_c_p_u_complex_tensor_1aa145c1b9bbf6749d7a5bcdc4c40718ae>`(
			size_t rank,
			:ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`* tensor,
			size_t max_rank
			);

		// methods
	
		virtual size_t :target:`getRank<doxid-class_c_p_u_complex_tensor_1a55c50daf029e17594e98a5ee1ae6fc15>`() const;
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` :target:`getElem<doxid-class_c_p_u_complex_tensor_1a375e11c3f830ca047f5a25b8ae3b87b8>`(size_t num);
		virtual size_t :target:`getMaxRank<doxid-class_c_p_u_complex_tensor_1a57161df8fb23b74697f0e000b00121ca>`() const;
		virtual void :target:`dimIncrement<doxid-class_c_p_u_complex_tensor_1a3b950063675d9927dbb00254946c76de>`(size_t increment_size);
	
		virtual void :target:`getSubTensor<doxid-class_c_p_u_complex_tensor_1a98e2436c70a6e3bb8e58f09d691f26df>`(
			size_t num,
			int value
			);
	
		virtual void :target:`dimDecrement<doxid-class_c_p_u_complex_tensor_1ac5158450a4a8bfb04dc81fae0ea32291>`(size_t num);
		virtual :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>`* :target:`getTensor<doxid-class_c_p_u_complex_tensor_1a27ca67453318bd54832c9ac0474e4b74>`();
	
		virtual void :target:`mul<doxid-class_c_p_u_complex_tensor_1acf912f74f0321921ecb05b8f15ea73a5>`(
			:ref:`ComplexTensor<doxid-class_complex_tensor>`& other,
			size_t* mask_array
			);
	
		virtual :ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>` :target:`getBackend<doxid-class_c_p_u_complex_tensor_1a2e98a1b4beb21b5be7f08a850ec030b8>`();
	
		void :target:`mulElem<doxid-class_c_p_u_complex_tensor_1a2442e84de54a79e236131046ec2d3ebf>`(
			size_t num,
			:ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` elem
			);
	
		CPUComplexTensor& :target:`operator =<doxid-class_c_p_u_complex_tensor_1a6843a67552753d9b3d84b54b6f815e6b>` (const CPUComplexTensor& old);
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
		virtual void :ref:`mul<doxid-class_abstract_complex_tensor_1a3d9432e3c63db33bd0c8d4b117752919>`(:ref:`ComplexTensor<doxid-class_complex_tensor>`& other, size_t* mask_array) = 0;
		virtual :ref:`ComputeBackend<doxid-_tensor_8h_1af82b80e30eed153c54317ba8ccfb5f00>` :ref:`getBackend<doxid-class_abstract_complex_tensor_1a84d0c5c0b8baa52ff132757aafd075b5>`() = 0;

