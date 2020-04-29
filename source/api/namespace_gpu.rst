.. index:: pair: namespace; gpu
.. _doxid-namespacegpu:

namespace gpu
=============

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace gpu {

	// global functions

	__global__ void :target:`unitarysingle<doxid-namespacegpu_1a21ed195eb96d75b279bd0cf0c94d8639>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Block,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real00,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real01,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real10,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real11,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag00,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag01,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag10,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag11
		);

	__global__ void :target:`controlunitarysingle<doxid-namespacegpu_1aeb9a3fbf261337b548196a1c28d3de1d>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` target_qubit,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` controller_mask,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real00,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real01,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real10,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_real11,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag00,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag01,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag10,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` matrix_imag11
		);

	__global__ void :target:`unitarydouble<doxid-namespacegpu_1aa27428ac981d45c9f1cb0f7871856330>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Block1,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Block2,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0111,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1111,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0111,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1111
		);

	__global__ void :target:`controlunitarydouble<doxid-namespacegpu_1a5e363098add5eea331075ace510fbdb8>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` controller_mask,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` control_qubit,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` target_qubit,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real0111,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` real1111,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag0111,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1000,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1001,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1010,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1011,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1100,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1101,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1110,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` imag1111
		);

	__global__ void :target:`initState<doxid-namespacegpu_1a9a05e5a5886e690b8b0036d63e205942>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim
		);

	__global__ void :target:`qubitprob<doxid-namespacegpu_1a8335da687b2bd3e29b8cf7ec4a102d69>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Block,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* pr
		);

	__global__ void :target:`probsum<doxid-namespacegpu_1a1ebee2c6fe9eec7c90f9025ff59c7b43>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* pr,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* prob
		);

	__global__ void :target:`qubitcollapse0<doxid-namespacegpu_1a692a56b9a63053b02258ef44017c5ba1>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Block,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` coef
		);

	__global__ void :target:`qubitcollapse1<doxid-namespacegpu_1aab09cdf09e3b7358a9233716c4934781>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Block,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>` coef
		);

	__global__ void :target:`multiprob<doxid-namespacegpu_1aa0018628bddaa4bb71c83b2f1d1ddb69>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* pro,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>`* block,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` m,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` dec
		);

	__global__ void :target:`probsumnew1<doxid-namespacegpu_1aa7b0ca8f94a0a716c7946463f4a91322>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* probtemp,
		size_t num1,
		size_t m,
		size_t Dim,
		size_t* block
		);

	__global__ void :target:`pmeasure_many_target<doxid-namespacegpu_1afff28041bfeedfc1576826bca27e3992>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		double* result,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` qnum_mask,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` result_size,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim
		);

	__global__ void :target:`pmeasure_one_target<doxid-namespacegpu_1a875a263106ce31ef3a907d6bc6998e3a>`(
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psireal,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* psiimag,
		double* result,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` qnum_mask,
		size_t result_idx,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` result_dim,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Dim
		);

	double :target:`randGenerator<doxid-namespacegpu_1a2dc6082b10a3fd32fd4eff59bf9f911d>`();

	} // namespace gpu
