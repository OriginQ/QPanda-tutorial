.. index:: pair: class; QPanda::TransformQGateType
.. _doxid-class_q_panda_1_1_transform_q_gate_type:

class QPanda::TransformQGateType
================================

.. toctree::
	:hidden:

Classes for tranform gate type and gate name.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TranformQGateTypeStringAndEnum.h>
	
	class TransformQGateType
	{
	public:
		// methods
	
		static TransformQGateType& :target:`getInstance<doxid-class_q_panda_1_1_transform_q_gate_type_1a163d218c1789175156ebecf7b5e7a677>`();
		std::string :target:`operator []<doxid-class_q_panda_1_1_transform_q_gate_type_1ab618b62f10d3c8dc9636f9cf0122532c>` (:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :target:`operator []<doxid-class_q_panda_1_1_transform_q_gate_type_1a04085485a30e7ffe201bb1a5c18c3f9f>` (std::string gate_name);
	};
