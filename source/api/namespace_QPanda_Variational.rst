.. index:: pair: namespace; QPanda::Variational
.. _doxid-namespace_q_panda_1_1_variational:

namespace QPanda::Variational
=============================

.. toctree::
	:hidden:

	enum_QPanda_Variational_OptimizerMode.rst
	enum_QPanda_Variational_back_flags.rst
	enum_QPanda_Variational_op_type.rst
	struct_QPanda_Variational_impl.rst
	struct_QPanda_Variational_impl_qop_pmeasure.rst
	struct_QPanda_Variational_impl_qop_pmeasure_real_chip.rst
	struct_QPanda_Variational_impl_stack.rst
	struct_QPanda_Variational_impl_subscript.rst
	struct_QPanda_Variational_impl_vqp.rst
	struct_QPanda_Variational_impl_vqp_real_chip.rst
	class_QPanda_Variational_AdaGradOptimizer.rst
	class_QPanda_Variational_AdamOptimizer.rst
	class_QPanda_Variational_MomentumOptimizer.rst
	class_QPanda_Variational_RMSPropOptimizer.rst
	class_QPanda_Variational_VanillaGradientDescentOptimizer.rst
	class_QPanda_Variational_VariationalQuantumCircuit.rst
	class_QPanda_Variational_VariationalQuantumGate.rst
	class_QPanda_Variational_VariationalQuantumGate_CNOT.rst
	class_QPanda_Variational_VariationalQuantumGate_CRX.rst
	class_QPanda_Variational_VariationalQuantumGate_CRY.rst
	class_QPanda_Variational_VariationalQuantumGate_CRZ.rst
	class_QPanda_Variational_VariationalQuantumGate_CZ.rst
	class_QPanda_Variational_VariationalQuantumGate_H.rst
	class_QPanda_Variational_VariationalQuantumGate_RX.rst
	class_QPanda_Variational_VariationalQuantumGate_RY.rst
	class_QPanda_Variational_VariationalQuantumGate_RZ.rst
	class_QPanda_Variational_VariationalQuantumGate_X.rst
	class_QPanda_Variational_var.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace Variational {

	// typedefs

	typedef :ref:`VariationalQuantumGate_H<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___h>` :target:`VQG_H<doxid-namespace_q_panda_1_1_variational_1a3e7cb5dd85497d940fb93b431fca0b71>`;
	typedef :ref:`VariationalQuantumGate_X<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___x>` :target:`VQG_X<doxid-namespace_q_panda_1_1_variational_1a8fe5fb201557ade4dfee6b88b82c734e>`;
	typedef :ref:`VariationalQuantumGate_RX<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_x>` :target:`VQG_RX<doxid-namespace_q_panda_1_1_variational_1aa7b18d00bdd49849689def2ad3f17be8>`;
	typedef :ref:`VariationalQuantumGate_RY<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_y>` :target:`VQG_RY<doxid-namespace_q_panda_1_1_variational_1ad620b15304a681177a4833dee85d4b6a>`;
	typedef :ref:`VariationalQuantumGate_RZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z>` :target:`VQG_RZ<doxid-namespace_q_panda_1_1_variational_1aa9edc37ede25104791ad08fe63760be9>`;
	typedef :ref:`VariationalQuantumGate_CNOT<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_n_o_t>` :target:`VQG_CNOT<doxid-namespace_q_panda_1_1_variational_1ad0a1c8267a732155a6bd235a1790b4b8>`;
	typedef :ref:`VariationalQuantumGate_CZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_z>` :target:`VQG_CZ<doxid-namespace_q_panda_1_1_variational_1aa5173ab4320d31ffb558cfcea95779ae>`;
	typedef :ref:`VariationalQuantumGate_CRX<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_x>` :target:`VQG_CRX<doxid-namespace_q_panda_1_1_variational_1a64855907681e1fd543abb57fe1af21f9>`;
	typedef :ref:`VariationalQuantumGate_CRY<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_y>` :target:`VQG_CRY<doxid-namespace_q_panda_1_1_variational_1a1479e48fc2ddf18dd951f64873024ec3>`;
	typedef :ref:`VariationalQuantumGate_CRZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_z>` :target:`VQG_CRZ<doxid-namespace_q_panda_1_1_variational_1acc051a96e18b4139f0d7fc60a6c1c148>`;
	typedef :ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>` :target:`VQG<doxid-namespace_q_panda_1_1_variational_1ae66af481d96918a10ad48881855f745c>`;
	typedef :ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>` :target:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>`;

	// enums

	enum :ref:`OptimizerMode<doxid-namespace_q_panda_1_1_variational_1a71962dc3e476a494d016aaee332062c1>`;
	enum :ref:`back_flags<doxid-namespace_q_panda_1_1_variational_1ab6e702288c07b79bbd3402d0810e7895>`;
	enum :ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>`;

	// structs

	struct :ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl>`;
	struct :ref:`impl_qop_pmeasure<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure>`;
	struct :ref:`impl_qop_pmeasure_real_chip<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure__real__chip>`;
	struct :ref:`impl_stack<doxid-struct_q_panda_1_1_variational_1_1impl__stack>`;
	struct :ref:`impl_subscript<doxid-struct_q_panda_1_1_variational_1_1impl__subscript>`;
	struct :ref:`impl_vqp<doxid-struct_q_panda_1_1_variational_1_1impl__vqp>`;
	struct :ref:`impl_vqp_real_chip<doxid-struct_q_panda_1_1_variational_1_1impl__vqp__real__chip>`;

	// classes

	class :ref:`AdaGradOptimizer<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer>`;
	class :ref:`AdamOptimizer<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer>`;
	class :ref:`Double<doxid-class_q_panda_1_1_variational_1_1_double>`;
	class :ref:`MomentumOptimizer<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer>`;
	class :ref:`Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`;
	class :ref:`RMSPropOptimizer<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer>`;
	class :ref:`VanillaGradientDescentOptimizer<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer>`;
	class :ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`;
	class :ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`;
	class :ref:`VariationalQuantumGate_CNOT<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_n_o_t>`;
	class :ref:`VariationalQuantumGate_CRX<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_x>`;
	class :ref:`VariationalQuantumGate_CRY<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_y>`;
	class :ref:`VariationalQuantumGate_CRZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_z>`;
	class :ref:`VariationalQuantumGate_CZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_z>`;
	class :ref:`VariationalQuantumGate_H<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___h>`;
	class :ref:`VariationalQuantumGate_RX<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_x>`;
	class :ref:`VariationalQuantumGate_RY<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_y>`;
	class :ref:`VariationalQuantumGate_RZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z>`;
	class :ref:`VariationalQuantumGate_X<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___x>`;
	class :ref:`expression<doxid-class_q_panda_1_1_variational_1_1expression>`;
	class :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`;

	// global functions

	MatrixXd :target:`eval<doxid-namespace_q_panda_1_1_variational_1a202db9d470734cd080bf3c1bb2526fb3>`(
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v,
		bool iter
		);

	void :target:`back<doxid-namespace_q_panda_1_1_variational_1a6b45a30cdb1de41c60b24383d98c8741>`(
		const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`&,
		std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>&
		);

	void :target:`back<doxid-namespace_q_panda_1_1_variational_1a13bec0fc45c5b1ace1374b09ffdc498a>`(
		:ref:`expression<doxid-class_q_panda_1_1_variational_1_1expression>`&,
		std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>&
		);

	void :target:`back<doxid-namespace_q_panda_1_1_variational_1a5126c88174246226f10f966ff5d97d19>`(
		const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`&,
		std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>&,
		const std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&
		);

	void :target:`back<doxid-namespace_q_panda_1_1_variational_1a1d5a4dd315830d9a8336bbdac6722f7e>`(
		:ref:`expression<doxid-class_q_panda_1_1_variational_1_1expression>`&,
		std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>&,
		const std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&
		);

	int :target:`numOpArgs<doxid-namespace_q_panda_1_1_variational_1a89f19f1cab77ba49a655394dbe6eae5a>`(:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` op);
	:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`& :target:`VariationalQuantumCircuit::insert< std::shared_ptr< VariationalQuantumGate > ><doxid-namespace_q_panda_1_1_variational_1ab5acaea57c45f7f5fa24c7e5c2502cff>`(std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> gate);

	template <typename... V>
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`pack_expression<doxid-namespace_q_panda_1_1_variational_1acfa924240b72b69e07d6827d67e2287d>`(
		:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` op,
		V&... args
		);

	template <typename... V>
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`pack_expression<doxid-namespace_q_panda_1_1_variational_1a4a5aaefa65b411bfa4d80be4c2b14216>`(
		:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` op,
		int axis,
		V&... args
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`operator +<doxid-namespace_q_panda_1_1_variational_1a3336129fdc0616037646bfe4bafbdad4>` (
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lhs,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` rhs
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`operator -<doxid-namespace_q_panda_1_1_variational_1a0302516cbed6526ceee03cff8cfb8ba1>` (
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lhs,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` rhs
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`operator *<doxid-namespace_q_panda_1_1_variational_1a938fbc7664ae4fdedf415a19a9a62c97>` (
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lhs,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` rhs
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`operator/<doxid-namespace_q_panda_1_1_variational_1aa04b94d606f400b744ad3481cdea04ea>` (
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lhs,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` rhs
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`exp<doxid-namespace_q_panda_1_1_variational_1a4ae4c653d423905e0de7d3d9965aa3bd>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v);
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`sigmoid<doxid-namespace_q_panda_1_1_variational_1ae344d72a2c9e889beb8a693e2433ec00>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v);
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`log<doxid-namespace_q_panda_1_1_variational_1aeb155a29339e517e3b693cdcf3e2b937>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`poly<doxid-namespace_q_panda_1_1_variational_1ae82607af1644938b726950759ca67cd1>`(
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` power
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`dot<doxid-namespace_q_panda_1_1_variational_1a2332c026bc86e2a455500447b82f9ec5>`(
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lhs,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` rhs
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`inverse<doxid-namespace_q_panda_1_1_variational_1a1a3ac05ba36e8c790052edcba883e9cb>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v);
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`transpose<doxid-namespace_q_panda_1_1_variational_1a4e1b071216a97817f9565c75478d6ed8>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v);
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`sum<doxid-namespace_q_panda_1_1_variational_1a52a994ab01aa6902dc51bae2e38e71e8>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v);
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`softmax<doxid-namespace_q_panda_1_1_variational_1a83a17926be29697ad7292237077c03ac>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` v);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`crossEntropy<doxid-namespace_q_panda_1_1_variational_1a17a3f832cacff638edf83caa499b9dab>`(
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lhs,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` rhs
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`dropout<doxid-namespace_q_panda_1_1_variational_1a8d3607fe94f547ada9508cb05122c3d8>`(
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lhs,
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` rhs
		);

	template <typename ... T>
	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`stack<doxid-namespace_q_panda_1_1_variational_1ac61fe0c93fca877f8dc5c7af085e8e2e>`(
		int axis,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`&... v
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`qop<doxid-namespace_q_panda_1_1_variational_1af4de21568c122d20b6c7ddbac7260c33>`(
		:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`& circuit,
		:ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` Hamiltonian,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
		std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> measure_qubits
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`qop_real_chip<doxid-namespace_q_panda_1_1_variational_1aa72123ff6837acd815693ad961357390>`(
		:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`& circuit,
		:ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` Hamiltonian,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
		std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> measure_qubits,
		int shots
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`qop<doxid-namespace_q_panda_1_1_variational_1a561e43718fbf9c8c24c0033e93802634>`(
		:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`& circuit,
		:ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` Hamiltonian,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
		std::map<size_t, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> measure_qubits
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`qop_pmeasure<doxid-namespace_q_panda_1_1_variational_1a2b7b6ffa6decb23a61f05879b8dab02d>`(
		:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`& circuit,
		std::vector<size_t> components,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
		std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> measure_qubits
		);

	const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`qop_pmeasure_real_chip<doxid-namespace_q_panda_1_1_variational_1afebea176e92c6d1617f362a673fba4cb>`(
		:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`& circuit,
		std::vector<size_t> components,
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
		std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> measure_qubits,
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> cbits,
		size_t shots
		);

	bool :target:`_is_scalar<doxid-namespace_q_panda_1_1_variational_1a0297a6d9a55dbea4032b2b90ad4a8aae>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& v);
	bool :target:`_is_matrix<doxid-namespace_q_panda_1_1_variational_1a2864c0fe0962bbbe4941ab25d4bc4b15>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& v);
	bool :target:`_is_vector<doxid-namespace_q_panda_1_1_variational_1ab5e44e41beebe7b3601b63b13689a06a>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& v);
	double :target:`_sval<doxid-namespace_q_panda_1_1_variational_1ab137aeb6331d5b4821b3e2de9ce29e82>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& v);
	MatrixXd :target:`_mval<doxid-namespace_q_panda_1_1_variational_1a4331404341bf5ee2e178b8f1a55b8764>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& v);
	MatrixXd :target:`scalar<doxid-namespace_q_panda_1_1_variational_1ae47b317f2fc90931620d9fd519a3676b>`(double num);
	MatrixXd :target:`vector2mat<doxid-namespace_q_panda_1_1_variational_1a0f5ca2e9f7414078cfac2ff6de96611d>`(std::vector<double> data);
	MatrixXd :target:`zeros_like<doxid-namespace_q_panda_1_1_variational_1aec2d11186fa2c7edd71ef96c52517a45>`(const MatrixXd& like);
	MatrixXd :target:`zeros_like<doxid-namespace_q_panda_1_1_variational_1acce687ef1f36539da7fe98e49fd33ad9>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& like);
	MatrixXd :target:`ones_like<doxid-namespace_q_panda_1_1_variational_1acca7b7bad615c33c76df88ffe7d02761>`(const MatrixXd& like);
	MatrixXd :target:`ones_like<doxid-namespace_q_panda_1_1_variational_1a28eb94e78d8736064119d4353195a77e>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& like);

	} // namespace Variational
