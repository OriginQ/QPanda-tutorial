.. index:: pair: class; QPanda::QubitFactory
.. _doxid-class_q_panda_1_1_qubit_factory:

class QPanda::QubitFactory
==========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`. :ref:`More...<details-class_q_panda_1_1_qubit_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitFactory.h>
	
	class QubitFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*(:ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`*)> :target:`constructor_t<doxid-class_q_panda_1_1_qubit_factory_1a68bd5cfc9f0f31b03e8d18c189c55a49>`;
		typedef std::map<std::string, :ref:`constructor_t<doxid-class_q_panda_1_1_qubit_factory_1a68bd5cfc9f0f31b03e8d18c189c55a49>`> :target:`constructor_Map_t<doxid-class_q_panda_1_1_qubit_factory_1a3869840623fce57af201328f690f12f4>`;

		// fields
	
		:ref:`constructor_Map_t<doxid-class_q_panda_1_1_qubit_factory_1a3869840623fce57af201328f690f12f4>` :target:`_Qubit_Constructor<doxid-class_q_panda_1_1_qubit_factory_1a967372591168e314426ab992542f7fc9>`;

		// methods
	
		static QubitFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_qubit_factory_1a123507a68770571469df98b89ddb84de>`();
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :target:`GetInstance<doxid-class_q_panda_1_1_qubit_factory_1a6c14d75cc05dc3645a46dd786c64cda8>`(:ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`*);
	
		void :target:`registerclass<doxid-class_q_panda_1_1_qubit_factory_1a4fef0ae259fe538d29d6a60818602863>`(
			std::string&,
			:ref:`constructor_t<doxid-class_q_panda_1_1_qubit_factory_1a68bd5cfc9f0f31b03e8d18c189c55a49>` constructor
			);
	};
.. _details-class_q_panda_1_1_qubit_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_qubit_factory_1a123507a68770571469df98b89ddb84de:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QubitFactory& GetFactoryInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QubitFactory <doxid-class_q_panda_1_1_qubit_factory>` &

