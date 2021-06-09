.. index:: pair: class; QPanda::AbstractCirOptimizer
.. _doxid-class_q_panda_1_1_abstract_cir_optimizer:

class QPanda::AbstractCirOptimizer
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitOptimize.h>
	
	class AbstractCirOptimizer
	{
	public:
		// methods
	
		virtual void :target:`do_optimize<doxid-class_q_panda_1_1_abstract_cir_optimizer_1afa4a904822e0b84ff3645d0c96d31685>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` src_prog,
			:ref:`OptimizerSink<doxid-namespace_q_panda_1a751da7aaa7cac46c55057a59f2285e73>`& gates_sink,
			:ref:`SinkPos<doxid-namespace_q_panda_1abc2b1c5d350f40cf0a262e7bc6de8822>`& sink_size,
			std::vector<:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`>& replace_to_cir_vec
			) = 0;
	
		virtual bool :target:`is_same_controled<doxid-class_q_panda_1_1_abstract_cir_optimizer_1a45cd6ac38002f380896fb6b1efdf2414>`(
			:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>` first_node,
			:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>` second_node
			);
	};
