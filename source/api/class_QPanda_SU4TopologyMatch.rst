.. index:: pair: class; QPanda::SU4TopologyMatch
.. _doxid-class_q_panda_1_1_s_u4_topology_match:

class QPanda::SU4TopologyMatch
==============================

.. toctree::
	:hidden:

	struct_QPanda_SU4TopologyMatch_gate.rst
	struct_QPanda_SU4TopologyMatch_gates_digraph.rst
	struct_QPanda_SU4TopologyMatch_node.rst
	struct_QPanda_SU4TopologyMatch_node_cmp.rst

Overview
~~~~~~~~

Su4 quantum circuit matches the topology of the physical qubits. :ref:`More...<details-class_q_panda_1_1_s_u4_topology_match>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <SU4TopologyMatch.h>
	
	class SU4TopologyMatch
	{
	public:
		// structs
	
		struct :ref:`gate<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate>`;
		struct :ref:`gates_digraph<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gates__digraph>`;
		struct :ref:`node<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node>`;
		struct :ref:`node_cmp<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node__cmp>`;

		// construction
	
		:target:`SU4TopologyMatch<doxid-class_q_panda_1_1_s_u4_topology_match_1a82367e3ffd34e572c451bbfa3babc9e3>`(
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* machine,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qv,
			:ref:`ArchType<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2a>` arch_type = :ref:`IBM_QX5_ARCH<doxid-namespace_q_panda_1aa47c4caa285ab72dca1885b13d182a2aa1d998a495737ef4502e83b080f3dada0>`
			);

		// methods
	
		void :ref:`mapping_qprog<doxid-class_q_panda_1_1_s_u4_topology_match_1a623be5524634c5f9151aabd5aa6aa2f6>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog);
	};
.. _details-class_q_panda_1_1_s_u4_topology_match:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Su4 quantum circuit matches the topology of the physical qubits.

Methods
-------

.. index:: pair: function; mapping_qprog
.. _doxid-class_q_panda_1_1_s_u4_topology_match_1a623be5524634c5f9151aabd5aa6aa2f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void mapping_qprog(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& mapped_prog)

Mapping qubits in a quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qprog

		- quantum program

	*
		- Qprog&

		- the mapped quantum program



.. rubric:: Returns:

void

