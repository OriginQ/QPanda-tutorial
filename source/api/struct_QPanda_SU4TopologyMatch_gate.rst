.. index:: pair: struct; QPanda::SU4TopologyMatch::gate
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate:

struct QPanda::SU4TopologyMatch::gate
=====================================

.. toctree::
	:hidden:

Store quantum gate information.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct gate
	{
		// fields
	
		int :target:`target<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate_1a00d80d8261973f6c2741305229453f18>`;
		int :target:`control<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate_1a81b3e1a1922dd8d6fffa940ad8d76f41>`;
		int :target:`type<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate_1a12fe51ea2cb5519adcead78043eb50bf>`;
		bool :target:`is_dagger<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate_1a80d59335fce0805dbacf05959afa6c64>`;
		bool :target:`is_flip<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate_1a7a581e66b339adc1ca466c5bbbf1d42d>`;
		std::vector<double> :target:`param<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1gate_1a45667cef216503742ddb02226385e1d8>`;
	};
