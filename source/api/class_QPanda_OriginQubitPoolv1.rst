.. index:: pair: class; QPanda::OriginQubitPoolv1
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1:

class QPanda::OriginQubitPoolv1
===============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>`. :ref:`More...<details-class_q_panda_1_1_origin_qubit_poolv1>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginQubitPoolv1: public :ref:`QPanda::QubitPool<doxid-class_q_panda_1_1_qubit_pool>`
	{
	public:
		// construction
	
		:target:`OriginQubitPoolv1<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a2355153b2e2fc6b866b939f40214f39f>`(size_t maxQubit);

		// methods
	
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a37cea3a8205698740f12ff1cb5d2d90a>`();
		virtual size_t :ref:`getMaxQubit<doxid-class_q_panda_1_1_origin_qubit_poolv1_1aabd1df8f128dd6dd1f62e2109faf100a>`() const;
		virtual size_t :ref:`getIdleQubit<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a9de8a59eb256972bf1ec086ff64c97f6>`() const;
		virtual size_t :ref:`get_max_usedqubit_addr<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a901204b9dbc3eb83d80792bee6064aa0>`() const;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubit<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a3890f2f8d63f49fef7597b3d81579718>`();
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a9b8ff5635e9a435ba88ab6a7e08b4c94>`(size_t);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a0c696701f0f3e5958f3ebb787727006f>`(size_t qubit_num);
		virtual void :ref:`Free_Qubit<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a5dcba974f17441bd48ff32a54533e264>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual size_t :ref:`getPhysicalQubitAddr<doxid-class_q_panda_1_1_origin_qubit_poolv1_1aac993411b59fa1586d3a185e7b8c7619>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a6d77800cedabe868718ee746413b0920>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const;
		virtual size_t :ref:`get_allocate_qubits<doxid-class_q_panda_1_1_origin_qubit_poolv1_1a563956bccc5813575e5e5380faa94f85>`(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>&) const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual size_t :ref:`getMaxQubit<doxid-class_q_panda_1_1_qubit_pool_1a557d6530da78875d35467979c7390017>`() const = 0;
		virtual size_t :ref:`get_max_usedqubit_addr<doxid-class_q_panda_1_1_qubit_pool_1aa784fee5f1552fa751ff4da58ddd363b>`() const = 0;
		virtual size_t :ref:`getIdleQubit<doxid-class_q_panda_1_1_qubit_pool_1ad6a5eba3ef747bea033d58ef8e9325d2>`() const = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubit<doxid-class_q_panda_1_1_qubit_pool_1a257710c139f9a9df2e7c98f8e8947f84>`() = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_qubit_pool_1affdaf4de13f5af779dc57c8f295f0493>`(size_t) = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_qubit_pool_1a9a7fa308c4ada8ab53b1761249e5615b>`(size_t qubit_num) = 0;
		virtual void :ref:`Free_Qubit<doxid-class_q_panda_1_1_qubit_pool_1aa7e5fa58ef884931215ce6e7f6c89141>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_qubit_pool_1a7962635e7aba3c82037bb9e5c4c5179d>`() = 0;
		virtual size_t :ref:`getPhysicalQubitAddr<doxid-class_q_panda_1_1_qubit_pool_1a0a2c2fbeb5f26eff65322e2809da4d6d>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_qubit_pool_1a99572216322ec218e12cbc651002dc4a>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const = 0;
		virtual size_t :ref:`get_allocate_qubits<doxid-class_q_panda_1_1_qubit_pool_1ac7914ab31598ef8d7f6b7a717f0856e7>`(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>&) const = 0;

.. _details-class_q_panda_1_1_origin_qubit_poolv1:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QubitPool <doxid-class_q_panda_1_1_qubit_pool>`.

Methods
-------

.. index:: pair: function; clearAll
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a37cea3a8205698740f12ff1cb5d2d90a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearAll()

clear the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector

.. index:: pair: function; getMaxQubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1aabd1df8f128dd6dd1f62e2109faf100a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getMaxQubit() const

get size of the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector



.. rubric:: Returns:

size_t

.. index:: pair: function; getIdleQubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a9de8a59eb256972bf1ec086ff64c97f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getIdleQubit() const

get size of the idle position



.. rubric:: Returns:

size_t

.. index:: pair: function; get_max_usedqubit_addr
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a901204b9dbc3eb83d80792bee6064aa0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_max_usedqubit_addr() const

Gets the largest address in the used physical qubit.



.. rubric:: Returns:

size_t

.. index:: pair: function; allocateQubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a3890f2f8d63f49fef7597b3d81579718:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubit()

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughPhyAddress
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a9b8ff5635e9a435ba88ab6a7e08b4c94:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughPhyAddress(size_t)

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through physical address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughVirAddress
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a0c696701f0f3e5958f3ebb787727006f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughVirAddress(size_t qubit_num)

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through virtual address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; Free_Qubit
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a5dcba974f17441bd48ff32a54533e264:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

free a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`

.. index:: pair: function; getPhysicalQubitAddr
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1aac993411b59fa1586d3a185e7b8c7619:

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
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a6d77800cedabe868718ee746413b0920:

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

.. index:: pair: function; get_allocate_qubits
.. _doxid-class_q_panda_1_1_origin_qubit_poolv1_1a563956bccc5813575e5e5380faa94f85:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_allocate_qubits(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>&) const

get allocate qubits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- 



.. rubric:: Returns:

size_t

