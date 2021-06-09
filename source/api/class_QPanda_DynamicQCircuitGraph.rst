.. index:: pair: class; QPanda::DynamicQCircuitGraph
.. _doxid-class_q_panda_1_1_dynamic_q_circuit_graph:

class QPanda::DynamicQCircuitGraph
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitMapping.h>
	
	class DynamicQCircuitGraph
	{
	public:
		// construction
	
		:target:`DynamicQCircuitGraph<doxid-class_q_panda_1_1_dynamic_q_circuit_graph_1ad21dc28ba726ddafdf4d9e93fd9fb891>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog);
		:target:`DynamicQCircuitGraph<doxid-class_q_panda_1_1_dynamic_q_circuit_graph_1a8258c697229b91e6676b88340293f271>`(const DynamicQCircuitGraph& c);

		// methods
	
		:ref:`FrontLayer<doxid-class_q_panda_1_1_front_layer>`& :target:`get_front_layer<doxid-class_q_panda_1_1_dynamic_q_circuit_graph_1ac87d68106e71bdb5b326cfa991298ed9>`();
		const :ref:`FrontLayer<doxid-class_q_panda_1_1_front_layer>`& :target:`get_front_layer_c<doxid-class_q_panda_1_1_dynamic_q_circuit_graph_1afa2db808914405b374d913bb37e035da>`() const;
		const :ref:`PressedTopoSeq<doxid-namespace_q_panda_1afdb6ed2767180c064e12c1a38a4201c3>`& :target:`get_layer_topo_seq<doxid-class_q_panda_1_1_dynamic_q_circuit_graph_1a84224253e7c0289fca35be1aa0f383a1>`() const;
	};
