.. index:: pair: namespace; GATEGPU
.. _doxid-namespace_g_a_t_e_g_p_u:

namespace GATEGPU
=================

.. toctree::
	:hidden:

	struct_GATEGPU_QState.rst
	struct_GATEGPU_probability.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace GATEGPU {

	// structs

	struct :ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`;
	struct :ref:`probability<doxid-struct_g_a_t_e_g_p_u_1_1probability>`;

	// global functions

	int :target:`devicecount<doxid-namespace_g_a_t_e_g_p_u_1a9234cf5c75b313bdedf1df450033d25e>`();

	bool :target:`initstate<doxid-namespace_g_a_t_e_g_p_u_1a46e7d9160f3a8528fb68dc0749c7edba>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psigpu,
		size_t
		);

	bool :target:`destroyState<doxid-namespace_g_a_t_e_g_p_u_1a12eb3155da86e5ec21d4fe289a2781c0>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psigpu,
		size_t sQnum
		);

	bool :target:`clearState<doxid-namespace_g_a_t_e_g_p_u_1a4b4ae04d2338989af16aea08fcb4bbff>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psigpu,
		size_t sQnum
		);

	bool :target:`Hadamard<doxid-namespace_g_a_t_e_g_p_u_1acf8cd6030a714bd8d6fbbd1c09b1956f>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`Hadamardnew<doxid-namespace_g_a_t_e_g_p_u_1a7012715fb4b61d19167206923dafea5f>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlHadamard<doxid-namespace_g_a_t_e_g_p_u_1af7d0583bd99e73fe45f7d3fe6bcdbdaf>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`X<doxid-namespace_g_a_t_e_g_p_u_1ad5779c84203560772495153dfd51466e>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlX<doxid-namespace_g_a_t_e_g_p_u_1a6427ad2b9261cab696b5a3bcdff73b94>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`Y<doxid-namespace_g_a_t_e_g_p_u_1ab3611cc3423f5512101d0f3da51beb43>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlY<doxid-namespace_g_a_t_e_g_p_u_1a9996bd0e1d6f8cb67a0a80ef99566049>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`Z<doxid-namespace_g_a_t_e_g_p_u_1a7d664455631798ca4c54ec737fc02c61>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlZ<doxid-namespace_g_a_t_e_g_p_u_1a8c2e2266daac4b87f3b55666c00a7050>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`S<doxid-namespace_g_a_t_e_g_p_u_1adfcaf0a8f926432adad090c1d85593a5>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlS<doxid-namespace_g_a_t_e_g_p_u_1a115d6c1f486b99b889e7db1e6e870765>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`T<doxid-namespace_g_a_t_e_g_p_u_1a092ade882756e58db4a38f7523dbf349>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlT<doxid-namespace_g_a_t_e_g_p_u_1a9ffe430fd4e20100a908f165903f98ba>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`RX<doxid-namespace_g_a_t_e_g_p_u_1ad4b95abc19cb6b684627418c2ba1c918>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlRX<doxid-namespace_g_a_t_e_g_p_u_1a60f644f4e4d0ecbe592ba17c16d26549>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`RY<doxid-namespace_g_a_t_e_g_p_u_1a4c0e4a443fa4c09906c88db36724fe72>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlRY<doxid-namespace_g_a_t_e_g_p_u_1a19d0b5f4b4fe7f9c3266365a7bd45f33>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`RZ<doxid-namespace_g_a_t_e_g_p_u_1a3719d0874a780936e3dd407101b49938>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlRZ<doxid-namespace_g_a_t_e_g_p_u_1a4977b6c7a002544c034c6c6b8624e4d6>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`CNOT<doxid-namespace_g_a_t_e_g_p_u_1a42e21424a80f201c9d7fd3a75ec5e4fe>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlCNOT<doxid-namespace_g_a_t_e_g_p_u_1adf0537cef1c1402ca3d31857e1f8e229>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`CZ<doxid-namespace_g_a_t_e_g_p_u_1adbf6d20650a4d82b80668a74c9a1b876>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlCZ<doxid-namespace_g_a_t_e_g_p_u_1a5bc126903aba2dcb561e23084d675ad2>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`CR<doxid-namespace_g_a_t_e_g_p_u_1afe05c062caafcb409d0f3fb7f7a8961d>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		double thete,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlCR<doxid-namespace_g_a_t_e_g_p_u_1a24af7cfdfdd247ec301d3ca9adf4d010>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`iSWAP<doxid-namespace_g_a_t_e_g_p_u_1a652c023ea2f25dc389cd187c3bf330f6>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		double thete,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controliSWAP<doxid-namespace_g_a_t_e_g_p_u_1a8b0b9e530b1807804e63597c4d631b2d>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		double theta,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`unitarysingle<doxid-namespace_g_a_t_e_g_p_u_1ad8aff4ceac5158d94ed6f58ccc32d297>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& matr,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlunitarysingle<doxid-namespace_g_a_t_e_g_p_u_1a2135208d77fff0668771091e104de2e4>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& matr,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`unitarydouble<doxid-namespace_g_a_t_e_g_p_u_1a0bbcae41cac23e73e663c74f284396e9>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t qn_0,
		size_t qn_1,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& matr,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`controlunitarydouble<doxid-namespace_g_a_t_e_g_p_u_1a6997181f114b96a4d68aebb5eb2e5e49>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& matr,
		bool isConjugate,
		double error_rate = 0
		);

	bool :target:`qbReset<doxid-namespace_g_a_t_e_g_p_u_1aab139dc69055abc8e6e9c7917b6c5654>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		size_t,
		double error_rate = 0
		);

	bool :target:`pMeasurenew<doxid-namespace_g_a_t_e_g_p_u_1a2cf1550ea4ae1ea5cd925c0d23a62087>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`&,
		:ref:`touple_prob<doxid-_g_p_u_struct_8h_1a6f3c3b9b86a1c5f31c541051760b64fe>`&,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&,
		int
		);

	bool :target:`getState<doxid-namespace_g_a_t_e_g_p_u_1aa264b4316fe7bc9a8103ec26b8652141>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psi,
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psigpu,
		size_t qnum
		);

	int :target:`qubitmeasure<doxid-namespace_g_a_t_e_g_p_u_1a736d650d772ba9f1ec9976703786d505>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`& psigpu,
		:ref:`gpu_qsize_t<doxid-_g_p_u_struct_8h_1aa4a2f82378db335373525d1ddc735a61>` Block,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* resultgpu,
		:ref:`gpu_qstate_t<doxid-_g_p_u_struct_8h_1a7cb9b1fe2e7d0267ca51a8ecfe7461f7>`* probgpu
		);

	bool :target:`pMeasure_no_index<doxid-namespace_g_a_t_e_g_p_u_1a7813e5ba918d943086c6ced0e4cef652>`(
		:ref:`QState<doxid-struct_g_a_t_e_g_p_u_1_1_q_state>`&,
		:ref:`vec_prob<doxid-_g_p_u_struct_8h_1a9e7ff63ce19e8c10cc6912f1bbe27d6e>`& mResult,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`&
		);

	void :target:`gpuFree<doxid-namespace_g_a_t_e_g_p_u_1a482d143b103dd976bf28672a63318bed>`(void* memory);

	} // namespace GATEGPU
