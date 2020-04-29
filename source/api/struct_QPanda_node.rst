.. index:: pair: struct; QPanda::node
.. _doxid-struct_q_panda_1_1node:

struct QPanda::node
===================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	struct node
	{
		// fields
	
		int :target:`cost_fixed<doxid-struct_q_panda_1_1node_1a5ee82df6e6ba33d6d0a4ff8f0aa7e11a>`;
		int :target:`cost_heur<doxid-struct_q_panda_1_1node_1a8bf5a20caa203f606469afd88b032c2d>`;
		int :target:`cost_heur2<doxid-struct_q_panda_1_1node_1a5a1da106d161e9924e455148136cc41b>`;
		int :target:`depth<doxid-struct_q_panda_1_1node_1a988f5f7627409aa51ca868bfb1b2edf3>`;
		std::vector<int> :target:`qubits<doxid-struct_q_panda_1_1node_1acd2dee442458b6bdb6e6115cbfd038c0>`;
		std::vector<int> :target:`locations<doxid-struct_q_panda_1_1node_1ae803f4ba5e76ee0d24095218f25b5aca>`;
		int :target:`nswaps<doxid-struct_q_panda_1_1node_1acf277fc3d48acdc72b9f069b90bee1d6>`;
		int :target:`done<doxid-struct_q_panda_1_1node_1abebaca2093f42c7852172e27b20dc741>`;
		std::vector<std::vector<:ref:`edge<doxid-struct_q_panda_1_1edge>`>> :target:`swaps<doxid-struct_q_panda_1_1node_1a4cb34d0442d63a3704f110f82b093419>`;
	};
