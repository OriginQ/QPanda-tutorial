.. index:: pair: class; QPanda::QIfRegisterAction
.. _doxid-class_q_panda_1_1_q_if_register_action:

class QPanda::QIfRegisterAction
===============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QIf program register action. :ref:`More...<details-class_q_panda_1_1_q_if_register_action>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ControlFlow.h>
	
	class QIfRegisterAction
	{
	public:
		// construction
	
		:ref:`QIfRegisterAction<doxid-class_q_panda_1_1_q_if_register_action_1a6c8f122a01429dea66af9d5767ee8516>`(std::string class_name, :ref:`CreateQIfTrueFalse_cb<doxid-namespace_q_panda_1a7000829c94e35e8ec34754dcf3ab0285>` create_callback);
		:ref:`QIfRegisterAction<doxid-class_q_panda_1_1_q_if_register_action_1a1e5e2951ee0e2407093e77c4f4509822>`(std::string class_name, :ref:`CreateQIfTrueOnly_cb<doxid-namespace_q_panda_1a7788fff614f34e49856571d7a6e67bac>` create_callback);
	};
.. _details-class_q_panda_1_1_q_if_register_action:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QIf program register action.

Provide :ref:`QIfFactory <doxid-class_q_panda_1_1_q_if_factory>` class registration interface for the outside

Construction
------------

.. index:: pair: function; QIfRegisterAction
.. _doxid-class_q_panda_1_1_q_if_register_action_1a6c8f122a01429dea66af9d5767ee8516:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QIfRegisterAction(std::string class_name, :ref:`CreateQIfTrueFalse_cb<doxid-namespace_q_panda_1a7000829c94e35e8ec34754dcf3ab0285>` create_callback)

Construct a new :ref:`QIfRegisterAction <doxid-class_q_panda_1_1_q_if_register_action>` object Call QIfFactory`s registClass interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- class_name

		- :ref:`AbstractControlFlowNode <doxid-class_q_panda_1_1_abstract_control_flow_node>` Implementation class name

	*
		- create_callback

		- The Constructor of Implementation class for :ref:`AbstractControlFlowNode <doxid-class_q_panda_1_1_abstract_control_flow_node>` which have true and false branch

.. index:: pair: function; QIfRegisterAction
.. _doxid-class_q_panda_1_1_q_if_register_action_1a1e5e2951ee0e2407093e77c4f4509822:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QIfRegisterAction(std::string class_name, :ref:`CreateQIfTrueOnly_cb<doxid-namespace_q_panda_1a7788fff614f34e49856571d7a6e67bac>` create_callback)

Construct a new :ref:`QIfRegisterAction <doxid-class_q_panda_1_1_q_if_register_action>` object Call QIfFactory`s registClass interface.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- class_name

		- :ref:`AbstractControlFlowNode <doxid-class_q_panda_1_1_abstract_control_flow_node>` Implementation class name

	*
		- create_callback

		- The Constructor of Implementation class for :ref:`AbstractControlFlowNode <doxid-class_q_panda_1_1_abstract_control_flow_node>` which only have branch

