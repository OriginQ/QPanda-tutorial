.. index:: pair: class; QPanda::Variational::VariationalQuantumCircuit
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit:

class QPanda::Variational::VariationalQuantumCircuit
====================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	class VariationalQuantumCircuit
	{
	public:
		// construction
	
		:target:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a506fac0b75144da39ca12b57d9a445e5>`();
		:target:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a8246385f771f44719b9dfc8541bc4373>`(const VariationalQuantumCircuit&);
		:target:`VariationalQuantumCircuit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a810ece5beb358dfd531b5759c1608276>`(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`);

		// methods
	
		std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& :target:`get_vars<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1ad9a3d10d7f17e61b66692a6dfbd0697d>`();
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a4b1e5495537a04b9867f6fb794a860f8>`(const std::vector<std::tuple<std::weak_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`>, size_t, double>>) const;
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a5d721bede056b570ce701a492202a6b4>`() const;
		std::vector<std::weak_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`>> :target:`get_var_in_which_gate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1aba1b09d90271583c586383bcd38b1929>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`&) const;
	
		template <typename VQG_Ty>
		VariationalQuantumCircuit& :target:`insert<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a4e5c7f642953427d62f318da5435c843>`(VQG_Ty gate);
	
		VariationalQuantumCircuit& :target:`insert<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1acfdc6e7d342684724ba8142b7a3f5a99>`(VariationalQuantumCircuit circuit);
		VariationalQuantumCircuit& :target:`insert<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a2dd8a7ae1fc3ffa8fc15a2796a5c2b77>`(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate);
		VariationalQuantumCircuit& :target:`insert<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1aea10f78be35fa4fc389f9ac8ea24d33c>`(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` gate);
		VariationalQuantumCircuit& :target:`insert<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_circuit_1a7c2333f56928074af8bcd90e5341988e>`(:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` c);
	};
