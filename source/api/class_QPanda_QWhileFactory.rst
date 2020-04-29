.. index:: pair: class; QPanda::QWhileFactory
.. _doxid-class_q_panda_1_1_q_while_factory:

class QPanda::QWhileFactory
===========================

.. toctree::
	:hidden:

QWhile factory.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class QWhileFactory
	{
	public:
		// methods
	
		void :target:`registClass<doxid-class_q_panda_1_1_q_while_factory_1a66520d8a0df5a1940df59bb27a66a893>`(
			std::string name,
			:ref:`CreateQWhile_cb<doxid-namespace_q_panda_1a36f049facff04a87084023a0cd28f40a>` method
			);
	
		:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`* :target:`getQWhile<doxid-class_q_panda_1_1_q_while_factory_1a35b3e71c9be0fba89066fc06eec7df66>`(
			std::string&,
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`
			);
	
		static QWhileFactory& :target:`getInstance<doxid-class_q_panda_1_1_q_while_factory_1a5a2d3b67d496eb576ece8d5a1d6cc631>`();
	};
