.. index:: pair: class; QPanda::CMemFactory
.. _doxid-class_q_panda_1_1_c_mem_factory:

class QPanda::CMemFactory
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`CMem <doxid-class_q_panda_1_1_c_mem>`. :ref:`More...<details-class_q_panda_1_1_c_mem_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CMemFactory.h>
	
	class CMemFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`CMem<doxid-class_q_panda_1_1_c_mem>`*(size_t)> :target:`size_constructor_t<doxid-class_q_panda_1_1_c_mem_factory_1a81b2fcb4ace420fe5646d2aa36ef61f6>`;
		typedef std::map<std::string, :ref:`size_constructor_t<doxid-class_q_panda_1_1_c_mem_factory_1a81b2fcb4ace420fe5646d2aa36ef61f6>`> :target:`size_constructor_stack_t<doxid-class_q_panda_1_1_c_mem_factory_1a7850a5139dcc0b1a7b4b79ec84e84034>`;

		// fields
	
		:ref:`size_constructor_stack_t<doxid-class_q_panda_1_1_c_mem_factory_1a7850a5139dcc0b1a7b4b79ec84e84034>` :target:`_CMem_Constructor<doxid-class_q_panda_1_1_c_mem_factory_1afad66c4feb3f9745b370dc5e6f6c828b>`;

		// methods
	
		:ref:`CMem<doxid-class_q_panda_1_1_c_mem>`* :target:`GetInstanceFromSize<doxid-class_q_panda_1_1_c_mem_factory_1a5bb213b171f9f0c627448c73d4c8435c>`(size_t);
	
		void :target:`registerclass_size_<doxid-class_q_panda_1_1_c_mem_factory_1a3a3a2824c7b1dc9f1f71403d773d6b26>`(
			std::string&,
			:ref:`size_constructor_t<doxid-class_q_panda_1_1_c_mem_factory_1a81b2fcb4ace420fe5646d2aa36ef61f6>`
			);
	
		static CMemFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_c_mem_factory_1a3dc95164dcd537417b589d2696ebcd88>`();
	};
.. _details-class_q_panda_1_1_c_mem_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`CMem <doxid-class_q_panda_1_1_c_mem>`.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_c_mem_factory_1a3dc95164dcd537417b589d2696ebcd88:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static CMemFactory& GetFactoryInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`CMemFactory <doxid-class_q_panda_1_1_c_mem_factory>` &

