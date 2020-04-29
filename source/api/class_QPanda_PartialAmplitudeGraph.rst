.. index:: pair: class; QPanda::PartialAmplitudeGraph
.. _doxid-class_q_panda_1_1_partial_amplitude_graph:

class QPanda::PartialAmplitudeGraph
===================================

.. toctree::
	:hidden:

Partial Amplitude Graph.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <PartialAmplitudeGraph.h>
	
	class PartialAmplitudeGraph
	{
	public:
		// fields
	
		uint32_t :target:`m_qubit_num<doxid-class_q_panda_1_1_partial_amplitude_graph_1ad6404c39c5bb831839762bc6db164ed3>`;
		uint32_t :target:`m_spilt_num<doxid-class_q_panda_1_1_partial_amplitude_graph_1a469797f7b051bd7b0881cb2724846b8a>`;
		std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`> :target:`m_circuit<doxid-class_q_panda_1_1_partial_amplitude_graph_1abd6edf7be3247b59522e09b8b76016af>`;
		std::vector<std::map<bool, std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`>>> :target:`m_circuit_vec<doxid-class_q_panda_1_1_partial_amplitude_graph_1a348455f73a9c4af3792258feb7cca423>`;

		// methods
	
		size_t :target:`getMapVecSize<doxid-class_q_panda_1_1_partial_amplitude_graph_1a0ccea71440d27d16e74d81d64e51f981>`();
		void :target:`init<doxid-class_q_panda_1_1_partial_amplitude_graph_1a83fd342a2936bffd33792d1a5f2e9af9>`(uint32_t qubit_num);
	
		void :target:`traversalMap<doxid-class_q_panda_1_1_partial_amplitude_graph_1a132462e6a912010d98895d604c4af2df>`(
			std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`>&,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`*
			);
	
		bool :target:`isCorssNode<doxid-class_q_panda_1_1_partial_amplitude_graph_1a9f009d8ffe9adfb259b8caf380798277>`(
			size_t,
			size_t
			);
	
		void :target:`traversalQlist<doxid-class_q_panda_1_1_partial_amplitude_graph_1a790d0358dfbbf7f38123f9bf3f22e35e>`(std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`>&);
		void :target:`splitQlist<doxid-class_q_panda_1_1_partial_amplitude_graph_1a7c3627ec2a69a4d29c434dc7f0051569>`(std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`>&);
	};
