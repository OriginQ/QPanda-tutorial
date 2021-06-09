.. index:: pair: struct; QPanda::TracebackInfo
.. _doxid-struct_q_panda_1_1_traceback_info:

struct QPanda::TracebackInfo
============================

.. toctree::
	:hidden:

Necessary information for getting the combinations in phase 2.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OBMTQMapping.h>
	
	struct TracebackInfo
	{
		// fields
	
		:ref:`Mapping<doxid-namespace_q_panda_1a7b5fe6d8f00345359e7ae23d05af5e24>` :target:`m<doxid-struct_q_panda_1_1_traceback_info_1aad73c2e4a63c749804271ee406223969>`;
		uint32_t :target:`parent<doxid-struct_q_panda_1_1_traceback_info_1aed6cb32b4ab4eee2d0511a27c69619e4>`;
		uint32_t :target:`mappingCost<doxid-struct_q_panda_1_1_traceback_info_1ade4c30e942ba75cec349167dc62ecfc2>`;
		uint32_t :target:`swapEstimatedCost<doxid-struct_q_panda_1_1_traceback_info_1a9675cdb15ce87649993273c7cecacf03>`;
		double :target:`mappingReliability<doxid-struct_q_panda_1_1_traceback_info_1a3f4882b585dd55505cd713f2d2aa6f21>`;
		double :target:`swapEstimatedReliability<doxid-struct_q_panda_1_1_traceback_info_1a5cd998e18dcd1109a97503cb6727796a>`;
	};
