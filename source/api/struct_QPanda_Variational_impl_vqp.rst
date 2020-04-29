.. index:: pair: struct; QPanda::Variational::impl_vqp
.. _doxid-struct_q_panda_1_1_variational_1_1impl__vqp:

struct QPanda::Variational::impl_vqp
====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	struct impl_vqp: public :ref:`QPanda::Variational::impl<doxid-struct_q_panda_1_1_variational_1_1impl>`
	{
		// construction
	
		:target:`impl_vqp<doxid-struct_q_panda_1_1_variational_1_1impl__vqp_1ad782236efd7f6e7d0757bb4606e73929>`(
			:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`,
			:ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*,
			std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>
			);
	
		:target:`impl_vqp<doxid-struct_q_panda_1_1_variational_1_1impl__vqp_1a21e0f8bc4fe939ca1bfe7a85b941f3a8>`(
			:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`,
			:ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*,
			std::map<size_t, :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>
			);

		// methods
	
		double :target:`_get_gradient<doxid-struct_q_panda_1_1_variational_1_1impl__vqp_1a53f947f2178c45531b543db2c95875f1>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` _var);
	
		double :target:`_get_gradient_one_term<doxid-struct_q_panda_1_1_variational_1_1impl__vqp_1ae4d787f0d0e2bf5e07dbdb4f9e56c0fe>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` _var,
			:ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`
			);
	
		double :target:`_get_expectation_one_term<doxid-struct_q_panda_1_1_variational_1_1impl__vqp_1a30434cc6f897cd68bf73d771dae68f71>`(
			:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`,
			:ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`
			);
	
		double :target:`_get_expectation<doxid-struct_q_panda_1_1_variational_1_1impl__vqp_1a2f60ca935ea2d45d208406768b73254f>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// fields
	
		MatrixXd :ref:`val<doxid-struct_q_panda_1_1_variational_1_1impl_1a192110dfe5013d1fd808aab4f262e241>`;
		bool :ref:`m_is_differentiable<doxid-struct_q_panda_1_1_variational_1_1impl_1ad7bb7cb00dd81ad05e29767d35ae2c4a>`;
		:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` :ref:`op<doxid-struct_q_panda_1_1_variational_1_1impl_1a48c4c2d47ded74e71bf3615945943e3b>`;
		std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :ref:`children<doxid-struct_q_panda_1_1_variational_1_1impl_1ab9026462afdd43c59bfe64fff032691f>`;
		std::vector<std::weak_ptr<:ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl>`>> :ref:`parents<doxid-struct_q_panda_1_1_variational_1_1impl_1a9cd6c23efd4e542bb77b9ad85f1e9529>`;
		MatrixXd :ref:`m_prob<doxid-struct_q_panda_1_1_variational_1_1impl_1af9668071cafbb85c671d03ef55065c87>`;

