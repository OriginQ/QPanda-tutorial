.. index:: pair: class; QPanda::PartialAmplitudeGraph
.. _doxid-class_q_panda_1_1_partial_amplitude_graph:

class QPanda::PartialAmplitudeGraph
===================================

.. toctree::
	:hidden:

Partial Amplitude :ref:`Graph <doxid-class_q_panda_1_1_graph>`.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <PartialAmplitudeGraph.h>
	
	class PartialAmplitudeGraph
	{
	public:
		// fields
	
		uint32_t :target:`m_spilt_num<doxid-class_q_panda_1_1_partial_amplitude_graph_1a469797f7b051bd7b0881cb2724846b8a>`;
		uint32_t :target:`m_qubit_num<doxid-class_q_panda_1_1_partial_amplitude_graph_1ad6404c39c5bb831839762bc6db164ed3>`;
		std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`> :target:`m_circuit<doxid-class_q_panda_1_1_partial_amplitude_graph_1abd6edf7be3247b59522e09b8b76016af>`;
		std::vector<std::vector<:ref:`cir_type<doxid-namespace_q_panda_1aad8fc9fe4ec5bfe6e66b9d5cc83b3ba0>`>> :target:`m_sub_graph<doxid-class_q_panda_1_1_partial_amplitude_graph_1a73c50cec9d716e73e1f39205dd9cdacb>`;

		// methods
	
		void :target:`reset<doxid-class_q_panda_1_1_partial_amplitude_graph_1adb6f08bdb3fcfab8ce4d8b9445f3759d>`(size_t qubit_num);
	
		void :target:`computing_graph<doxid-class_q_panda_1_1_partial_amplitude_graph_1afc63b3ce94cc16a43fe770e48130f266>`(
			const :ref:`cir_type<doxid-namespace_q_panda_1aad8fc9fe4ec5bfe6e66b9d5cc83b3ba0>`&,
			:ref:`QPUImpl<doxid-class_q_p_u_impl>`*
			);
	
		bool :target:`is_corss_node<doxid-class_q_panda_1_1_partial_amplitude_graph_1af7c0cc48c512571cf60637f4eeb3d18a>`(
			size_t,
			size_t
			);
	
		void :target:`traversal<doxid-class_q_panda_1_1_partial_amplitude_graph_1a49f9088702aff95b8793d1a20cdd2ca4>`(std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`>&);
		void :target:`split_circuit<doxid-class_q_panda_1_1_partial_amplitude_graph_1aa2d3c3497b52ec0b525693c0ec987081>`(std::vector<:ref:`QGateNode<doxid-struct_q_panda_1_1_q_gate_node>`>&);
	};
