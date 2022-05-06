.. index:: pair: class; QPanda::FrontLayer
.. _doxid-class_q_panda_1_1_front_layer:

class QPanda::FrontLayer
========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitMapping.h>
	
	class FrontLayer
	{
	public:
		// methods
	
		const :ref:`pPressedCirNode<doxid-namespace_q_panda_1a0c66eb4b29f78788a53807281eae451c>`& :target:`operator []<doxid-class_q_panda_1_1_front_layer_1ab4d9486043046e59403d89eb4fadd807>` (uint32_t i) const;
		uint32_t :target:`size<doxid-class_q_panda_1_1_front_layer_1a7502fea16b5b834ea01e403d87244e39>`() const;
		const std::vector<:ref:`pPressedCirNode<doxid-namespace_q_panda_1a0c66eb4b29f78788a53807281eae451c>`>& :target:`get_front_layer_nodes<doxid-class_q_panda_1_1_front_layer_1a98ca8c1a54ea36ac533303f99082351d>`() const;
		void :target:`remove_node<doxid-class_q_panda_1_1_front_layer_1a8814f0a9a6873446358eca3eef8eff1d>`(:ref:`pPressedCirNode<doxid-namespace_q_panda_1a0c66eb4b29f78788a53807281eae451c>` p_node);
		uint32_t :target:`remove_node<doxid-class_q_panda_1_1_front_layer_1a9d555177aba5272622f5d9f63601aa87>`(uint32_t i);
	};
