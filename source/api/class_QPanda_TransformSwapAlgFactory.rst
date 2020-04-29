.. index:: pair: class; QPanda::TransformSwapAlgFactory
.. _doxid-class_q_panda_1_1_transform_swap_alg_factory:

class QPanda::TransformSwapAlgFactory
=====================================

.. toctree::
	:hidden:

swap qubit location algorithm factory


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TopologyMatch.h>
	
	class TransformSwapAlgFactory
	{
	public:
		// methods
	
		:ref:`TransformSwapAlg<doxid-class_q_panda_1_1_transform_swap_alg>`* :target:`CreateByType<doxid-class_q_panda_1_1_transform_swap_alg_factory_1a3aab6ec8fb7ca9a96661f3b2b7805a00>`(:ref:`SwapQubitsMethod<doxid-namespace_q_panda_1a7f591622bab3f78555ae0db8d6919b73>` type);
		static TransformSwapAlgFactory& :target:`GetFactoryInstance<doxid-class_q_panda_1_1_transform_swap_alg_factory_1ab2fd8aea48fbc57e5d268796bffb0124>`();
	};
