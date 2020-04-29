.. index:: pair: class; QPanda::PhysicalQubitFactory
.. _doxid-class_q_panda_1_1_physical_qubit_factory:

class QPanda::PhysicalQubitFactory
==================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>`. :ref:`More...<details-class_q_panda_1_1_physical_qubit_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <PhysicalQubitFactory.h>
	
	class PhysicalQubitFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`*()> :target:`constructor_t<doxid-class_q_panda_1_1_physical_qubit_factory_1ab8cac735bf59a04052ec1f00a4b7dfec>`;
		typedef std::map<std::string, :ref:`constructor_t<doxid-class_q_panda_1_1_physical_qubit_factory_1ab8cac735bf59a04052ec1f00a4b7dfec>`> :target:`constructor_Map_t<doxid-class_q_panda_1_1_physical_qubit_factory_1a44926d46ef990e1091c66c58105fc0d0>`;

		// fields
	
		:ref:`constructor_Map_t<doxid-class_q_panda_1_1_physical_qubit_factory_1a44926d46ef990e1091c66c58105fc0d0>` :target:`_Physical_Qubit_Constructor<doxid-class_q_panda_1_1_physical_qubit_factory_1a0f85cc74f37274850517fa3e08c92ab2>`;

		// methods
	
		static PhysicalQubitFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_physical_qubit_factory_1a06b2f057e56aa3942f63f008b01d509a>`();
		:ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* :target:`GetInstance<doxid-class_q_panda_1_1_physical_qubit_factory_1a601eb1afd228fa0368e9730fe23a0ff9>`();
	
		void :target:`registerclass<doxid-class_q_panda_1_1_physical_qubit_factory_1a772f8bedc861a7624457530f06584809>`(
			std::string&,
			:ref:`constructor_t<doxid-class_q_panda_1_1_physical_qubit_factory_1ab8cac735bf59a04052ec1f00a4b7dfec>` constructor
			);
	};
.. _details-class_q_panda_1_1_physical_qubit_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>`.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_physical_qubit_factory_1a06b2f057e56aa3942f63f008b01d509a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static PhysicalQubitFactory& GetFactoryInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`PhysicalQubitFactory <doxid-class_q_panda_1_1_physical_qubit_factory>` &

