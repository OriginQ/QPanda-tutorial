.. index:: pair: class; QPanda::QubitPoolFactory
.. _doxid-class_q_panda_1_1_qubit_pool_factory:

class QPanda::QubitPoolFactory
==============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>`. :ref:`More...<details-class_q_panda_1_1_qubit_pool_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitPoolFactory.h>
	
	class QubitPoolFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`QubitPool<doxid-class_q_panda_1_1_qubit_pool>`*(size_t)> :target:`size_constructor_t<doxid-class_q_panda_1_1_qubit_pool_factory_1a61d6f4596ac13fde1243259ed974b443>`;
		typedef std::map<std::string, :ref:`size_constructor_t<doxid-class_q_panda_1_1_qubit_pool_factory_1a61d6f4596ac13fde1243259ed974b443>`> :target:`size_constructor_stack_t<doxid-class_q_panda_1_1_qubit_pool_factory_1abb93d1f40e620ebbc1cfe35c39529bf0>`;

		// fields
	
		:ref:`size_constructor_stack_t<doxid-class_q_panda_1_1_qubit_pool_factory_1abb93d1f40e620ebbc1cfe35c39529bf0>` :target:`_Qubit_Pool_Constructor<doxid-class_q_panda_1_1_qubit_pool_factory_1a531846332ef12bb10e7f45ff77205fb8>`;

		// methods
	
		static QubitPoolFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_qubit_pool_factory_1af63998737beedaf91580cf34dd30c05f>`();
		:ref:`QubitPool<doxid-class_q_panda_1_1_qubit_pool>`* :target:`GetPoolWithoutTopology<doxid-class_q_panda_1_1_qubit_pool_factory_1a5899838f647665e138936f89a6ae9c59>`(size_t);
	
		void :target:`registerclass_size_<doxid-class_q_panda_1_1_qubit_pool_factory_1a8a2e63f4781fc6a2d08deabb2bb2f635>`(
			std::string&,
			:ref:`size_constructor_t<doxid-class_q_panda_1_1_qubit_pool_factory_1a61d6f4596ac13fde1243259ed974b443>` constructor
			);
	};
.. _details-class_q_panda_1_1_qubit_pool_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>`.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_qubit_pool_factory_1af63998737beedaf91580cf34dd30c05f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QubitPoolFactory& GetFactoryInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QubitPoolFactory <doxid-class_q_panda_1_1_qubit_pool_factory>` &

