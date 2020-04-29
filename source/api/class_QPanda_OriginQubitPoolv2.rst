.. index:: pair: class; QPanda::OriginQubitPoolv2
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2:

class QPanda::OriginQubitPoolv2
===============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>`. :ref:`More...<details-class_q_panda_1_1_origin_qubit_poolv2>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginQubitPoolv2: public :ref:`QPanda::QubitPool<doxid-class_q_panda_1_1_qubit_pool>`
	{
	public:
		// construction
	
		:target:`OriginQubitPoolv2<doxid-class_q_panda_1_1_origin_qubit_poolv2_1ad7354c748f96264ba9c249e385ba4bc5>`(size_t maxQubit);

		// methods
	
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_origin_qubit_poolv2_1a2a3a5dfdc29c871efb978ef0c3167a24>`();
		virtual size_t :ref:`getMaxQubit<doxid-class_q_panda_1_1_origin_qubit_poolv2_1a6544b917f0e7b8a27c948b4beb84dd60>`() const;
		virtual size_t :ref:`getIdleQubit<doxid-class_q_panda_1_1_origin_qubit_poolv2_1a99bdb2b34f6d55e74418cd416b708b7b>`() const;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubit<doxid-class_q_panda_1_1_origin_qubit_poolv2_1ac142d7e11ffde291e8ddfba27b223e0b>`();
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_origin_qubit_poolv2_1a10ca7ae8cde018daf296d9074a30a2c5>`(size_t);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_origin_qubit_poolv2_1a6ccba68bdfd98c0773efe2910224a47f>`(size_t qubit_num);
		virtual void :ref:`Free_Qubit<doxid-class_q_panda_1_1_origin_qubit_poolv2_1ae6ea9cb3db525cb4b39832192b5d1a14>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual size_t :ref:`getPhysicalQubitAddr<doxid-class_q_panda_1_1_origin_qubit_poolv2_1a299a96ee5241fa63805dec2733118d56>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_origin_qubit_poolv2_1a34b9a22f99fb9496083464c6da189d73>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

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

.. _details-class_q_panda_1_1_origin_qubit_poolv2:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>`.

Methods
-------

.. index:: pair: function; clearAll
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1a2a3a5dfdc29c871efb978ef0c3167a24:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearAll()

clear the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector

.. index:: pair: function; getMaxQubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1a6544b917f0e7b8a27c948b4beb84dd60:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getMaxQubit() const

get size of the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector



.. rubric:: Returns:

size_t

.. index:: pair: function; getIdleQubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1a99bdb2b34f6d55e74418cd416b708b7b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getIdleQubit() const

get size of the idle position



.. rubric:: Returns:

size_t

.. index:: pair: function; allocateQubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1ac142d7e11ffde291e8ddfba27b223e0b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubit()

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughPhyAddress
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1a10ca7ae8cde018daf296d9074a30a2c5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughPhyAddress(size_t)

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through physical address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughVirAddress
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1a6ccba68bdfd98c0773efe2910224a47f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughVirAddress(size_t qubit_num)

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through virtual address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; Free_Qubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1ae6ea9cb3db525cb4b39832192b5d1a14:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

free a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`

.. index:: pair: function; getPhysicalQubitAddr
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1a299a96ee5241fa63805dec2733118d56:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getPhysicalQubitAddr(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

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
.. _doxid-class_q_panda_1_1_origin_qubit_poolv2_1a34b9a22f99fb9496083464c6da189d73:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getVirtualQubitAddress(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const

get virtual qubit address



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- 



.. rubric:: Returns:

size_t

