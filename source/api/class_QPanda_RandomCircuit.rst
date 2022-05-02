.. index:: pair: class; QPanda::RandomCircuit
.. _doxid-class_q_panda_1_1_random_circuit:

class QPanda::RandomCircuit
===========================

.. toctree::
	:hidden:

	struct_QPanda_RandomCircuit_QubitInformation.rst

Generate random quantum circuit.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <RandomCircuit.h>
	
	class RandomCircuit
	{
	public:
		// typedefs
	
		typedef std::vector<std::vector<:ref:`QubitInformation<doxid-struct_q_panda_1_1_random_circuit_1_1_qubit_information>`>> :target:`LayerInfo<doxid-class_q_panda_1_1_random_circuit_1a7c129d5afb6d253e20a932cbdfce275e>`;
		typedef std::function<bool(int, int, :ref:`LayerInfo<doxid-class_q_panda_1_1_random_circuit_1a7c129d5afb6d253e20a932cbdfce275e>`&)> :target:`SetLayerFunc<doxid-class_q_panda_1_1_random_circuit_1aa815baad3542b90aff3f3f49cb5a0f92>`;

		// structs
	
		struct :ref:`QubitInformation<doxid-struct_q_panda_1_1_random_circuit_1_1_qubit_information>`;

		// construction
	
		:target:`RandomCircuit<doxid-class_q_panda_1_1_random_circuit_1a55123fedc9a7fc196a10598edc60e3e4>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv
			);

		// methods
	
		void :target:`random_circuit<doxid-class_q_panda_1_1_random_circuit_1a40316e8ea96284efc1539b0b1fc05c74>`(
			int qbitRow,
			int qbitColumn,
			int depth
			);
	
		std::string :target:`get_random_originir<doxid-class_q_panda_1_1_random_circuit_1a2d66d9c64aceacf08d258315a515f601>`();
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`get_random_qprog<doxid-class_q_panda_1_1_random_circuit_1ad9fed01379483f7dd4a93374c313c948>`();
	};
