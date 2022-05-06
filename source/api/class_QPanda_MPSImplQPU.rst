.. index:: pair: class; QPanda::MPSImplQPU
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u:

class QPanda::MPSImplQPU
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QPU implementation by MPS model. :ref:`More...<details-class_q_panda_1_1_m_p_s_impl_q_p_u>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <MPSImplQPU.h>
	
	class MPSImplQPU: public :ref:`QPUImpl<doxid-class_q_p_u_impl>`
	{
	public:
		// fields
	
		std::vector<:ref:`MPS_Tensor<doxid-class_m_p_s___tensor>`> :ref:`m_qubits_tensor<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a4177a567c0847c3862a8509789311444>`;
		std::vector<:ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`> :ref:`m_lambdas<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1acff6e9301157771849970a243fb2f099>`;

		// methods
	
		size_t :target:`get_qubit_num<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a3633937fc41fe6bbf68577631f163602>`();
		virtual bool :target:`qubitMeasure<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a2243b75173466d330d29bb8a51281352>`(size_t qn);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`pMeasure<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a78d90167c3e935519516e8ff814d8329>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`initState<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a4d7a5a024b3b08dc7ea9cc674f5aefea>`(
			size_t head_rank,
			size_t rank_size,
			size_t qubit_num
			);
	
		void :target:`initState<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a6c4263b8c23fec5f6467c250fc879aa6>`(const MPSImplQPU& other);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`initState<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1afaa1796c60606e269dd50ee344572a75>`(
			size_t qubit_num,
			const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& state = {}
			);
	
		void :ref:`initState_from_matrix<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a59de06132c0460f46ce8287da8cfefb5>`(size_t num_qubits, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1aa6fbee340ea0f6ba9c6db9ec2d09cccc>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a7b905c2b1b33a2ddb4c935f4ba726994>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a4ca05e827d2e27f7473b5bb38a90be36>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a422cc477aca1e1f7f1af561a43b927f3>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a0da50982b3322da7cce65fe69467bf09>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a59f168807624e698df54caf07d37bef8>`(size_t qn);
		size_t :ref:`get_qubit_index<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a20bb4c8b31a599cd4e89c7be36a11336>`(size_t index) const;
		void :ref:`change_qubits_location<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a5dc06d8c2b179114483fc49d077159bc>`(size_t src, size_t dst);
		void :ref:`swap_qubits_location<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1ad628319764e400f6ef8e16c4af0110c4>`(size_t index_A, size_t index_B);
		bool :ref:`measure_one_collapsing<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a6bc770db40b9d280e26ac20645d89f76>`(size_t qubit);
		std::vector<std::vector<size_t>> :ref:`measure_all_noncollapsing<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a10abb872a7a1f3d8f2ba4ba8c62addec>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` measure_qubits, int shots);
		:ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>` :ref:`mul_v_by_s<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1aa21344607cac37da4db3c72681772793>`(const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat, const :ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& lambda);
		:ref:`MPS_Tensor<doxid-class_m_p_s___tensor>` :ref:`convert_qstate_to_mps_form<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a83f6ba3379f146ff833cab001d63899d>`(size_t first_index, size_t last_index);
		void :ref:`centralize_and_sort_qubits<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1aec9f860c3b99eb41335a335447e14d9e>`(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& sorted_indices, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& centralized_qubits);
		void :ref:`move_all_qubits_to_sorted_ordering<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a90042d22202dfc73554d74faa83ef7c7>`();
		void :ref:`move_qubits_to_right_end<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a1c3d07de1001000731ebbd2bbad34d7b>`(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& target_qubits, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& actual_indices);
		void :ref:`execute_one_qubit_gate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a1d3010aa70bfd5b88074c88cafc06dcd>`(size_t qn, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat);
		void :ref:`execute_two_qubit_gate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1abef0952b71cee3548c30ea3d1d5ce782>`(size_t qn_0, size_t qn_1, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat);
		void :ref:`execute_multi_qubit_gate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a623c56e9a2d2853f98bba4c7cdaa2da5>`(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat);
		:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` :target:`expectation_value_pauli<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a9a3af752abc9f1a3ae18f5f279771ace>`(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits);
	
		:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` :target:`expectation_value_pauli_internal<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a4406f3a0cfe4f42d2a67a886cb9810f5>`(
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits,
			const std::vector<:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`>& matrices,
			size_t first_index,
			size_t last_index,
			size_t num_Is
			);
	
		bool :target:`apply_measure<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a913288c374d43f48219c4f7112977591>`(size_t qubit);
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` :target:`apply_measure<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a8defed524f15c624e92bd13e3b06affa>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` qubits);
		:ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>` :target:`density_matrix<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a22f1b6f579d35dd7f2828cd88a0c9f38>`(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits);
	
		double :target:`expectation_value<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a9e3281167641660509e04e6e08f59a9c>`(
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits,
			const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& matrix
			);
	
		double :target:`single_expectation_value<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a24aa82c2771ed710fc701dfe40d19140>`(
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits,
			const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& matrix
			);
	
		double :target:`double_expectation_value<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1ac51f60efc5269371afa7256cc89da2c7>`(
			const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits,
			const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& matrix
			);
	
		void :target:`unitaryQubitGate<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a1dd31741ca11201b71e3023436f4d9aa>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` qubits,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` matrix,
			bool isConjugate
			);
	
		:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` :target:`pmeasure_bin_index<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a8e2b256940c567704c5e5cd2163fc663>`(std::string str);
		:ref:`qcomplex_t<doxid-_q_panda_namespace_8h_1a71506c06f9e4329b5ecaba7a6473a661>` :target:`pmeasure_dec_index<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1ab2cbc5d99e98ff29c190025c0b006602>`(std::string str);
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`pmeasure_bin_subset<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1ad1e574b36389f77897b67b3cc9d44a66>`(const std::vector<std::string>& bin_strs);
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`pmeasure_dec_subset<doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a381b73b5cbe9a78bd922b7bd81f7ab0d>`(const std::vector<std::string>& dec_strs);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual bool :ref:`qubitMeasure<doxid-class_q_p_u_impl_1a8231dac2a0406c20032c871de6f45df3>`(size_t qn) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`pMeasure<doxid-class_q_p_u_impl_1a7b81f6f6dd6e1d3e56b812335cd26e5f>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`initState<doxid-class_q_p_u_impl_1a2fb637028cde700f9b415a9f0770eb02>`(size_t head_rank, size_t rank_size, size_t qubit_num) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`initState<doxid-class_q_p_u_impl_1a4caf9a31a84bb94def033f9686477041>`(size_t qubit_num, const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& state = {}) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_q_p_u_impl_1a5d4651b69e9ddcf7f3180b577a80ea22>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_q_p_u_impl_1ad1d0629c91a42e06e079d6d6c215c0a9>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ad5f00e8ccf36ca66f48f4c63b3650e61>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ac164d4305076d2d34f61997ef63a1f34>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_p_u_impl_1aa4152648b4001296305ee546a1136abc>`() = 0;
		virtual void :ref:`set_random_engine<doxid-class_q_p_u_impl_1ae8d102f1acac09f453c26f096d0e62ea>`(:ref:`RandomEngine<doxid-class_random_engine>`* rng);
		virtual double :ref:`get_random_double<doxid-class_q_p_u_impl_1a25c1af43b633e913810831a5bfd7c90d>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_q_p_u_impl_1a9087cb5109b90f3215093165b11b4218>`(size_t qn) = 0;

.. _details-class_q_panda_1_1_m_p_s_impl_q_p_u:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPU implementation by MPS model.

Fields
------

.. index:: pair: variable; m_qubits_tensor
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a4177a567c0847c3862a8509789311444:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`MPS_Tensor<doxid-class_m_p_s___tensor>`> m_qubits_tensor

the tensor of qubits.

.. index:: pair: variable; m_lambdas
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1acff6e9301157771849970a243fb2f099:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`> m_lambdas

lambdas between tensors.

Methods
-------

.. index:: pair: function; initState_from_matrix
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a59de06132c0460f46ce8287da8cfefb5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void initState_from_matrix(size_t num_qubits, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat)

init state from matrix



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- number of qubits

	*
		- cmatrix_t

		- matrix

.. index:: pair: function; unitarySingleQubitGate
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1aa6fbee340ea0f6ba9c6db9ec2d09cccc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitarySingleQubitGate(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`)

unitary single qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

	*
		- QStat&

		- matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; controlunitarySingleQubitGate
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a7b905c2b1b33a2ddb4c935f4ba726994:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitarySingleQubitGate(
		size_t qn,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

controlunitary single qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

	*
		- Qnum&

		- control qubit addresses

	*
		- QStat

		- & matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; unitaryDoubleQubitGate
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a4ca05e827d2e27f7473b5bb38a90be36:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

unitary double qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- first qubit address

	*
		- size_t

		- second qubit address

	*
		- QStat&

		- matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; controlunitaryDoubleQubitGate
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a422cc477aca1e1f7f1af561a43b927f3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

controlunitary double qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- first qubit address

	*
		- size_t

		- second qubit address

	*
		- Qnum&

		- control qubit addresses

	*
		- QStat&

		- quantum states

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; getQState
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a0da50982b3322da7cce65fe69467bf09:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getQState()

get quantum states



.. rubric:: Returns:

QStat quantum states

.. index:: pair: function; Reset
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a59f168807624e698df54caf07d37bef8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` Reset(size_t qn)

reset qubit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

.. index:: pair: function; get_qubit_index
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a20bb4c8b31a599cd4e89c7be36a11336:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t get_qubit_index(size_t index) const

gets the position of the qubits in MPS form



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubits index



.. rubric:: Returns:

size_t the position on m_qubits_location

.. index:: pair: function; change_qubits_location
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a5dc06d8c2b179114483fc49d077159bc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void change_qubits_location(size_t src, size_t dst)

change two qubits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- src qubit location

	*
		- size_t

		- dst qubit location

.. index:: pair: function; swap_qubits_location
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1ad628319764e400f6ef8e16c4af0110c4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void swap_qubits_location(size_t index_A, size_t index_B)

execute SWAP gate, the state of swapping two qubits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- A qubit index

	*
		- size_t

		- B qubit index

.. index:: pair: function; measure_one_collapsing
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a6bc770db40b9d280e26ac20645d89f76:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool measure_one_collapsing(size_t qubit)

measure one qubit collapsing



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- the qubit position of the measurement



.. rubric:: Returns:

bool the measurement results

.. index:: pair: function; measure_all_noncollapsing
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a10abb872a7a1f3d8f2ba4ba8c62addec:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::vector<size_t>> measure_all_noncollapsing(
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>` measure_qubits,
		int shots
		)

measure all qubits collapsing



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- the qubit position of the measurement



.. rubric:: Returns:

std::vector<std::vector<size_t>> the measurement results

.. index:: pair: function; mul_v_by_s
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1aa21344607cac37da4db3c72681772793:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>` mul_v_by_s(const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat, const :ref:`rvector_t<doxid-_m_p_s_tensor_8h_1a0e3ae2c20c3a6f0c2b27dcfe25536bdd>`& lambda)

after the SVD decomposition , The product of S and V



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cmatrix_t

		- V matrix

	*
		- rvector_t

		- S vector



.. rubric:: Returns:

cmatrix_t product

.. index:: pair: function; convert_qstate_to_mps_form
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a83f6ba3379f146ff833cab001d63899d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`MPS_Tensor<doxid-class_m_p_s___tensor>` convert_qstate_to_mps_form(size_t first_index, size_t last_index)

convert to MPS form



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- starting position

	*
		- size_t

		- end position



.. rubric:: Returns:

:ref:`MPS_Tensor <doxid-class_m_p_s___tensor>` MPS form tensor

.. index:: pair: function; centralize_and_sort_qubits
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1aec9f860c3b99eb41335a335447e14d9e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void centralize_and_sort_qubits(
		const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& sorted_indices,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& centralized_qubits
		)

sort qubits location, and centralize qubits locations



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qnum

		- original qubits location

	*
		- Qnum

		- sorted indices

	*
		- Qnum

		- centralized qubits location

.. index:: pair: function; move_all_qubits_to_sorted_ordering
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a90042d22202dfc73554d74faa83ef7c7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void move_all_qubits_to_sorted_ordering()

move all qubits to sorted ordering

.. index:: pair: function; move_qubits_to_right_end
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a1c3d07de1001000731ebbd2bbad34d7b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void move_qubits_to_right_end(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& target_qubits, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& actual_indices)

move qubits to right_end location



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qnum

		- original qubits location

	*
		- Qnum

		- target qubits location

	*
		- actual

		- indices

.. index:: pair: function; execute_one_qubit_gate
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a1d3010aa70bfd5b88074c88cafc06dcd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void execute_one_qubit_gate(size_t qn, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat)

execute one qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- target qubit

	*
		- cmatrix_t

		- gate matrix

.. index:: pair: function; execute_two_qubit_gate
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1abef0952b71cee3548c30ea3d1d5ce782:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void execute_two_qubit_gate(size_t qn_0, size_t qn_1, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat)

execute two qubits gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- control qubit

	*
		- size_t

		- target qubit

	*
		- cmatrix_t

		- gate matrix

.. index:: pair: function; execute_multi_qubit_gate
.. _doxid-class_q_panda_1_1_m_p_s_impl_q_p_u_1a623c56e9a2d2853f98bba4c7cdaa2da5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void execute_multi_qubit_gate(const :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qubits, const :ref:`cmatrix_t<doxid-_m_p_s_tensor_8h_1a7be001f23f22e79d4c8e8fb6ad0a1aee>`& mat)

execute multi qubits gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- control and target qubits, target qubit in the tail

	*
		- cmatrix_t

		- gate matrix

