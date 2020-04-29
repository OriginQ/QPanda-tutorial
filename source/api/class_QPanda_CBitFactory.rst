.. index:: pair: class; QPanda::CBitFactory
.. _doxid-class_q_panda_1_1_c_bit_factory:

class QPanda::CBitFactory
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`. :ref:`More...<details-class_q_panda_1_1_c_bit_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CBitFactory.h>
	
	class CBitFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*(std::string)> :target:`name_constructor_t<doxid-class_q_panda_1_1_c_bit_factory_1aea55deb35dbcaab2c5a98fae1eaea5a9>`;
		typedef std::map<std::string, :ref:`name_constructor_t<doxid-class_q_panda_1_1_c_bit_factory_1aea55deb35dbcaab2c5a98fae1eaea5a9>`> :target:`name_constructor_stack_t<doxid-class_q_panda_1_1_c_bit_factory_1a09e6510764b00b90fa67b91360d37c49>`;

		// fields
	
		:ref:`name_constructor_stack_t<doxid-class_q_panda_1_1_c_bit_factory_1a09e6510764b00b90fa67b91360d37c49>` :target:`_CBit_Constructor<doxid-class_q_panda_1_1_c_bit_factory_1aa177112f623eb24bb2749b32349cf729>`;

		// methods
	
		static CBitFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_c_bit_factory_1ab8987e04b4e2f194ec0f25814de067b5>`();
	
		void :target:`registerclass_name_<doxid-class_q_panda_1_1_c_bit_factory_1a7f224a54d23b34682b3bde70ecee784e>`(
			std::string&,
			:ref:`name_constructor_t<doxid-class_q_panda_1_1_c_bit_factory_1aea55deb35dbcaab2c5a98fae1eaea5a9>` constructor
			);
	
		:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :target:`CreateCBitFromName<doxid-class_q_panda_1_1_c_bit_factory_1a3b34721d062ef7aea5efdf937430372b>`(std::string);
	};
.. _details-class_q_panda_1_1_c_bit_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_c_bit_factory_1ab8987e04b4e2f194ec0f25814de067b5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static CBitFactory& GetFactoryInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`CBitFactory <doxid-class_q_panda_1_1_c_bit_factory>` &

