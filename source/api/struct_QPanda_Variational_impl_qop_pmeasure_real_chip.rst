.. index:: pair: struct; QPanda::Variational::impl_qop_pmeasure_real_chip
.. _doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure__real__chip:

struct QPanda::Variational::impl_qop_pmeasure_real_chip
=======================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	struct impl_qop_pmeasure_real_chip: public :ref:`QPanda::Variational::impl<doxid-struct_q_panda_1_1_variational_1_1impl>`
	{
		// construction
	
		:target:`impl_qop_pmeasure_real_chip<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure__real__chip_1a033d75b1012940afc32dd77e3ac58bcf>`(
			:ref:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit>`,
			std::vector<size_t>,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*,
			std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>,
			std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>,
			size_t shots
			);

		// methods
	
		std::vector<double> :target:`_get_gradient<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure__real__chip_1aae4acc69d8df31f479ef1e2b08297c78>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` _var);
		std::vector<double> :target:`_get_value<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure__real__chip_1ac9b2553811a688499351953618070886>`();
		std::vector<double> :target:`_get_circuit_value<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure__real__chip_1af566788dc997688abde02d0b14c74750>`(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`);
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

