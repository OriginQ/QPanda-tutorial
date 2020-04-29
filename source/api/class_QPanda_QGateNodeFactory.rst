.. index:: pair: class; QPanda::QGateNodeFactory
.. _doxid-class_q_panda_1_1_q_gate_node_factory:

class QPanda::QGateNodeFactory
==============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`QGate <doxid-class_q_panda_1_1_q_gate>`. :ref:`More...<details-class_q_panda_1_1_q_gate_node_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QGate.h>
	
	class QGateNodeFactory
	{
	public:
		// methods
	
		static QGateNodeFactory* :ref:`getInstance<doxid-class_q_panda_1_1_q_gate_node_factory_1ae46d7ac6c641011f2aefec5de2897598>`();
	
		template <typename ... Targs>
		:ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :target:`getGateNode<doxid-class_q_panda_1_1_q_gate_node_factory_1abf2b14a9da434f00f0c9c535b224de7d>`(
			const std::string& name,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qs,
			Targs&&... args
			);
	};
.. _details-class_q_panda_1_1_q_gate_node_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`QGate <doxid-class_q_panda_1_1_q_gate>`.

Methods
-------

.. index:: pair: function; getInstance
.. _doxid-class_q_panda_1_1_q_gate_node_factory_1ae46d7ac6c641011f2aefec5de2897598:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QGateNodeFactory* getInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QGateNodeFactory <doxid-class_q_panda_1_1_q_gate_node_factory>` \*

