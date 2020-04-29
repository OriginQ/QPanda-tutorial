.. index:: pair: class; QPanda::QubitPool
.. _doxid-class_q_panda_1_1_qubit_pool:

class QPanda::QubitPool
=======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

:ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>` abstract class It is the container of the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>`. :ref:`More...<details-class_q_panda_1_1_qubit_pool>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitPoolFactory.h>
	
	class QubitPool
	{
	public:
		// methods
	
		virtual size_t :ref:`getMaxQubit<doxid-class_q_panda_1_1_qubit_pool_1a557d6530da78875d35467979c7390017>`() const = 0;
		virtual size_t :ref:`getIdleQubit<doxid-class_q_panda_1_1_qubit_pool_1ad6a5eba3ef747bea033d58ef8e9325d2>`() const = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubit<doxid-class_q_panda_1_1_qubit_pool_1a257710c139f9a9df2e7c98f8e8947f84>`() = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_qubit_pool_1affdaf4de13f5af779dc57c8f295f0493>`(size_t) = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_qubit_pool_1a9a7fa308c4ada8ab53b1761249e5615b>`(size_t qubit_num) = 0;
		virtual void :ref:`Free_Qubit<doxid-class_q_panda_1_1_qubit_pool_1aa7e5fa58ef884931215ce6e7f6c89141>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_qubit_pool_1a7962635e7aba3c82037bb9e5c4c5179d>`() = 0;
		virtual size_t :ref:`getPhysicalQubitAddr<doxid-class_q_panda_1_1_qubit_pool_1a0a2c2fbeb5f26eff65322e2809da4d6d>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_qubit_pool_1a99572216322ec218e12cbc651002dc4a>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const = 0;
	};

	// direct descendants

	class :ref:`OriginQubitPool<doxid-class_q_panda_1_1_origin_qubit_pool>`;
	class :ref:`OriginQubitPoolv2<doxid-class_q_panda_1_1_origin_qubit_poolv2>`;
.. _details-class_q_panda_1_1_qubit_pool:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>` abstract class It is the container of the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>`.

Methods
-------

.. index:: pair: function; getMaxQubit
.. _doxid-class_q_panda_1_1_qubit_pool_1a557d6530da78875d35467979c7390017:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getMaxQubit() const = 0

get size of the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector



.. rubric:: Returns:

size_t

.. index:: pair: function; getIdleQubit
.. _doxid-class_q_panda_1_1_qubit_pool_1ad6a5eba3ef747bea033d58ef8e9325d2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getIdleQubit() const = 0

get size of the idle position



.. rubric:: Returns:

size_t

.. index:: pair: function; allocateQubit
.. _doxid-class_q_panda_1_1_qubit_pool_1a257710c139f9a9df2e7c98f8e8947f84:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubit() = 0

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughPhyAddress
.. _doxid-class_q_panda_1_1_qubit_pool_1affdaf4de13f5af779dc57c8f295f0493:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughPhyAddress(size_t) = 0

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through physical address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughVirAddress
.. _doxid-class_q_panda_1_1_qubit_pool_1a9a7fa308c4ada8ab53b1761249e5615b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughVirAddress(size_t qubit_num) = 0

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through virtual address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; Free_Qubit
.. _doxid-class_q_panda_1_1_qubit_pool_1aa7e5fa58ef884931215ce6e7f6c89141:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0

free a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`

.. index:: pair: function; clearAll
.. _doxid-class_q_panda_1_1_qubit_pool_1a7962635e7aba3c82037bb9e5c4c5179d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearAll() = 0

clear the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector

.. index:: pair: function; getPhysicalQubitAddr
.. _doxid-class_q_panda_1_1_qubit_pool_1a0a2c2fbeb5f26eff65322e2809da4d6d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getPhysicalQubitAddr(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0

get physical qubit address



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- 



.. rubric:: Returns:

size_t

.. index:: pair: function; getVirtualQubitAddress
.. _doxid-class_q_panda_1_1_qubit_pool_1a99572216322ec218e12cbc651002dc4a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getVirtualQubitAddress(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const = 0

get virtual qubit address



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- 



.. rubric:: Returns:

size_t

