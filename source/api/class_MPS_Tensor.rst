.. index:: pair: class; MPS_Tensor
.. _doxid-class_m_p_s___tensor:

class MPS_Tensor
================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <MPSTensor.h>
	
	class MPS_Tensor
	{
	public:
		// fields
	
		std::vector<:ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`> :target:`m_physical_index<doxid-class_m_p_s___tensor_1a8e8a1ad3666b6b91bdad1679a0b8d13e>`;

		// construction
	
		:target:`MPS_Tensor<doxid-class_m_p_s___tensor_1a2116c456e8b8fa5fa016dcbade14dd60>`();
	
		:target:`MPS_Tensor<doxid-class_m_p_s___tensor_1ae06100c5af5ae172139af881178bcad4>`(
			const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& data0,
			const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& data1
			);

		// methods
	
		size_t :target:`get_dim<doxid-class_m_p_s___tensor_1a05343ce4ce23ea4c3e9428c1855eacc0>`() const;
		std::vector<:ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`> :target:`get_data<doxid-class_m_p_s___tensor_1a52f891a57fe51703dc50875c7669ca43>`() const;
		:ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>` :target:`get_data<doxid-class_m_p_s___tensor_1a59c13348f083d2c4a43da3454be81210>`(size_t i) const;
		void :target:`apply_swap<doxid-class_m_p_s___tensor_1a3441ec032bf3225d6f8a32a8ffa19a06>`();
	
		void :target:`apply_matrix<doxid-class_m_p_s___tensor_1abac94639902c865ea741004f68aaad01>`(
			const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat,
			bool swapped = false
			);
	
		void :target:`mul_gamma_by_left_lambda<doxid-class_m_p_s___tensor_1ae1532f2c54c2dff00f534c38e12f450f>`(const :ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& Lambda);
		void :target:`mul_gamma_by_right_lambda<doxid-class_m_p_s___tensor_1a74504d5144f6979027b33155add5d95f>`(const :ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& Lambda);
		void :target:`div_gamma_by_left_lambda<doxid-class_m_p_s___tensor_1a2df79577dd32103ef174d991e3a01310>`(const :ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& Lambda);
		void :target:`div_gamma_by_right_lambda<doxid-class_m_p_s___tensor_1ab17a742b2c9f730c710d7ab3e6cc5279>`(const :ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& Lambda);
		void :target:`apply_pauli<doxid-class_m_p_s___tensor_1abef1102ed949d25fc659c597662eba3d>`(:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` gate);
	
		static MPS_Tensor :target:`contract<doxid-class_m_p_s___tensor_1ac7500206d4a74b9244821ca8a256ca16>`(
			const MPS_Tensor& left_gamma,
			const :ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& lambda,
			const MPS_Tensor& right_gamma
			);
	
		static void :target:`decompose<doxid-class_m_p_s___tensor_1a8f8e39c7a7f3c07f25a685913eb27cc9>`(
			MPS_Tensor& temp,
			MPS_Tensor& left_gamma,
			:ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& lambda,
			MPS_Tensor& right_gamma
			);
	
		static void :target:`contract_2_dimensions<doxid-class_m_p_s___tensor_1abecf0477ff9dd72ce3d0766ac0be3a81>`(
			const MPS_Tensor& left_gamma,
			const MPS_Tensor& right_gamma,
			:ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& result
			);
	};
