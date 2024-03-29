.. index:: pair: class; QPanda::OriginQubitPool
.. _doxid-class_q_panda_1_1_origin_qubit_pool:

class QPanda::OriginQubitPool
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginQubitPool: public :ref:`QPanda::QubitPool<doxid-class_q_panda_1_1_qubit_pool>`
	{
	public:
		// methods
	
		static OriginQubitPool* :target:`get_instance<doxid-class_q_panda_1_1_origin_qubit_pool_1ab6c7e61c6edcff3693ab7f856f7503d3>`();
		size_t :target:`get_capacity<doxid-class_q_panda_1_1_origin_qubit_pool_1ae490bc21960f0c2134a36de8ce7c32a2>`();
		void :target:`set_capacity<doxid-class_q_panda_1_1_origin_qubit_pool_1ab6a8b4a825f8cb444c04130594f2870f>`(size_t);
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :target:`get_qubit_by_addr<doxid-class_q_panda_1_1_origin_qubit_pool_1ae7fa036fe155a6f1aba1069ec721b25b>`(size_t qaddr);
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_origin_qubit_pool_1a3daa08ee90ec03ac9583d4341f25e28f>`();
		virtual size_t :ref:`getMaxQubit<doxid-class_q_panda_1_1_origin_qubit_pool_1ae21b8c3c6a90a2063ebae8ca77501e9f>`() const;
		virtual size_t :ref:`getIdleQubit<doxid-class_q_panda_1_1_origin_qubit_pool_1aa86d390b6c4948eb44f6a38ebd711268>`() const;
		virtual size_t :ref:`get_max_usedqubit_addr<doxid-class_q_panda_1_1_origin_qubit_pool_1a4ec5765f7b12c8415b0152778e455055>`() const;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubit<doxid-class_q_panda_1_1_origin_qubit_pool_1a095b5c0a89a5083923ee11ab5504eac4>`();
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughPhyAddress<doxid-class_q_panda_1_1_origin_qubit_pool_1a584a025d186468c8d603569cf75db937>`(size_t);
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`allocateQubitThroughVirAddress<doxid-class_q_panda_1_1_origin_qubit_pool_1aa56a2b1954f9b9834b0477a9d66ec5ec>`(size_t qubit_num);
		virtual void :ref:`Free_Qubit<doxid-class_q_panda_1_1_origin_qubit_pool_1a01f41389cffce42427fccc14b3737fb4>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual size_t :ref:`getPhysicalQubitAddr<doxid-class_q_panda_1_1_origin_qubit_pool_1aee2d5e5a0f1b40b105af4302bc3d96c2>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		virtual size_t :ref:`getVirtualQubitAddress<doxid-class_q_panda_1_1_origin_qubit_pool_1a38b608356530b3b192f813f69796251b>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) const;
		virtual size_t :ref:`get_allocate_qubits<doxid-class_q_panda_1_1_origin_qubit_pool_1a52b60312a570c04a361e44f4b8508ed0>`(std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>&) const;
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :target:`qAlloc<doxid-class_q_panda_1_1_origin_qubit_pool_1a60362266261312096764664770d224ce>`();
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`qAllocMany<doxid-class_q_panda_1_1_origin_qubit_pool_1aabf9792efd510d1e8946b1b2b661abb1>`(size_t);
		void :target:`qFree<doxid-class_q_panda_1_1_origin_qubit_pool_1a062278f8c4252217a2ac478c8f0d354c>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		void :target:`qFreeAll<doxid-class_q_panda_1_1_origin_qubit_pool_1ad85a812a1a4722171cda81840a87100e>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
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

.. _details-class_q_panda_1_1_origin_qubit_pool:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; clearAll
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1a3daa08ee90ec03ac9583d4341f25e28f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearAll()

clear the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector

.. index:: pair: function; getMaxQubit
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1ae21b8c3c6a90a2063ebae8ca77501e9f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getMaxQubit() const

get size of the :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` vector



.. rubric:: Returns:

size_t

.. index:: pair: function; getIdleQubit
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1aa86d390b6c4948eb44f6a38ebd711268:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getIdleQubit() const

get size of the idle position



.. rubric:: Returns:

size_t

.. index:: pair: function; get_max_usedqubit_addr
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1a4ec5765f7b12c8415b0152778e455055:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_max_usedqubit_addr() const

Gets the largest address in the used physical qubit.



.. rubric:: Returns:

size_t

.. index:: pair: function; allocateQubit
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1a095b5c0a89a5083923ee11ab5504eac4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubit()

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughPhyAddress
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1a584a025d186468c8d603569cf75db937:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughPhyAddress(size_t)

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through physical address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; allocateQubitThroughVirAddress
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1aa56a2b1954f9b9834b0477a9d66ec5ec:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* allocateQubitThroughVirAddress(size_t qubit_num)

allocate a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` through virtual address



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; Free_Qubit
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1a01f41389cffce42427fccc14b3737fb4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_Qubit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

free a :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`

.. index:: pair: function; getPhysicalQubitAddr
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1aee2d5e5a0f1b40b105af4302bc3d96c2:

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
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1a38b608356530b3b192f813f69796251b:

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
.. _doxid-class_q_panda_1_1_origin_qubit_pool_1a52b60312a570c04a361e44f4b8508ed0:

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

