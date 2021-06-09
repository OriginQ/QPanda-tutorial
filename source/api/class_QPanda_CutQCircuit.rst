.. index:: pair: class; QPanda::CutQCircuit
.. _doxid-class_q_panda_1_1_cut_q_circuit:

class QPanda::CutQCircuit
=========================

.. toctree::
	:hidden:

	struct_QPanda_CutQCircuit_CutFragment.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CutQC.h>
	
	class CutQCircuit
	{
	public:
		// structs
	
		struct :ref:`CutFragment<doxid-struct_q_panda_1_1_cut_q_circuit_1_1_cut_fragment>`;

		// construction
	
		:target:`CutQCircuit<doxid-class_q_panda_1_1_cut_q_circuit_1a29ba332b5eab5e7c11a21e96149cff34>`(const :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& prog_dag);

		// methods
	
		void :target:`cut_circuit<doxid-class_q_panda_1_1_cut_q_circuit_1a52d9ed9f87a9a9ad638c0694eaa327a5>`(
			const std::map<uint32_t, std::vector<uint32_t>>& cut_pos,
			const std::vector<std::vector<uint32_t>>& sub_graph_vertice,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);
	
		void :target:`generate_subcircuits<doxid-class_q_panda_1_1_cut_q_circuit_1ac66ff2886ca74d945348cd113b24fd46>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm);
		const std::vector<:ref:`SubCircuit<doxid-struct_q_panda_1_1_sub_circuit>`>& :target:`get_cutted_sub_circuits<doxid-class_q_panda_1_1_cut_q_circuit_1a4d376dd8d478c7e07e3e5b5126f5e016>`(std::vector<uint32_t>& qubit_permutation);
		std::vector<:ref:`StitchesInfo<doxid-struct_q_panda_1_1_stitches_info>`> :target:`get_stitches<doxid-class_q_panda_1_1_cut_q_circuit_1aad40c1f691d25181520e0e1a7852f573>`(const std::map<uint32_t, std::vector<uint32_t>>& cut_pos);
	};
