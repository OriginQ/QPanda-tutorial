.. index:: pair: class; QPanda::QIfFactory
.. _doxid-class_q_panda_1_1_q_if_factory:

class QPanda::QIfFactory
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`AbstractControlFlowNode <doxid-class_q_panda_1_1_abstract_control_flow_node>`. :ref:`More...<details-class_q_panda_1_1_q_if_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class QIfFactory
	{
	public:
		// methods
	
		void :target:`registClass<doxid-class_q_panda_1_1_q_if_factory_1affe3ba4c85a13b9e9d46b6460946f355>`(
			std::string name,
			:ref:`CreateQIfTrueFalse_cb<doxid-namespace_q_panda_1a7000829c94e35e8ec34754dcf3ab0285>` method
			);
	
		void :target:`registClass<doxid-class_q_panda_1_1_q_if_factory_1a1bed1fe659709e2791935bb75981bbae>`(
			std::string name,
			:ref:`CreateQIfTrueOnly_cb<doxid-namespace_q_panda_1a7788fff614f34e49856571d7a6e67bac>` method
			);
	
		:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`* :target:`getQIf<doxid-class_q_panda_1_1_q_if_factory_1a72554acb830a5d69473a351e93eaed29>`(
			std::string& class_name,
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& classical_condition,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` true_node,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` false_node
			);
	
		:ref:`AbstractControlFlowNode<doxid-class_q_panda_1_1_abstract_control_flow_node>`* :target:`getQIf<doxid-class_q_panda_1_1_q_if_factory_1a6253b7288e097b5f5c8ee52f6521fe4e>`(
			std::string& name,
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& classical_cond,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` node
			);
	
		static QIfFactory& :ref:`getInstance<doxid-class_q_panda_1_1_q_if_factory_1aa6ed38f5337a06f5fbf3e317edc24a34>`();
	};
.. _details-class_q_panda_1_1_q_if_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`AbstractControlFlowNode <doxid-class_q_panda_1_1_abstract_control_flow_node>`.

Methods
-------

.. index:: pair: function; getInstance
.. _doxid-class_q_panda_1_1_q_if_factory_1aa6ed38f5337a06f5fbf3e317edc24a34:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QIfFactory& getInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QIfFactory <doxid-class_q_panda_1_1_q_if_factory>` &

