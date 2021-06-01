.. index:: pair: class; QPanda::OriginCMem
.. _doxid-class_q_panda_1_1_origin_c_mem:

class QPanda::OriginCMem
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`CMem <doxid-class_q_panda_1_1_c_mem>`. :ref:`More...<details-class_q_panda_1_1_origin_c_mem>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginCMem: public :ref:`QPanda::CMem<doxid-class_q_panda_1_1_c_mem>`
	{
	public:
		// methods
	
		static OriginCMem* :target:`get_instance<doxid-class_q_panda_1_1_origin_c_mem_1a503c645dc807b1c2fc4d0588a3e2b791>`();
		:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :target:`get_cbit_by_addr<doxid-class_q_panda_1_1_origin_c_mem_1a1806da14e31861f671ecae1d1624fc63>`(size_t caddr);
		size_t :target:`get_capacity<doxid-class_q_panda_1_1_origin_c_mem_1af71383738126bf09bdabf0d53754f6ec>`();
		void :target:`set_capacity<doxid-class_q_panda_1_1_origin_c_mem_1aa1be9c9bee312a32f9c19e6957528a3b>`(size_t capacity_num);
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_origin_c_mem_1a27635c8b914a2e8b01e680e7a2ad731d>`();
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_origin_c_mem_1a167dbc305426029d1e474d8bed1e4db7>`(size_t);
		virtual size_t :ref:`getMaxMem<doxid-class_q_panda_1_1_origin_c_mem_1a395c37bbc93334fa149a969c9803da48>`() const;
		virtual size_t :ref:`getIdleMem<doxid-class_q_panda_1_1_origin_c_mem_1ad51e7b4636026398a487b001c5b1d42f>`() const;
		virtual void :ref:`Free_CBit<doxid-class_q_panda_1_1_origin_c_mem_1a5c4c393aeb4042869582ec59d0b0defb>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*);
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_origin_c_mem_1ae9bd193eb67a5d51cb9b4e61b055e16a>`();
		virtual size_t :ref:`get_allocate_cbits<doxid-class_q_panda_1_1_origin_c_mem_1a57cf999d5dd126a206a0152202cb25bc>`(std::vector<:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*>&);
		:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :target:`cAlloc<doxid-class_q_panda_1_1_origin_c_mem_1ab2af5f4e82b3ac8a61c39d6c5e644e5d>`();
		:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :target:`cAlloc<doxid-class_q_panda_1_1_origin_c_mem_1a93b9e9451334ac9e35015078b21a89e6>`(size_t);
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :target:`cAllocMany<doxid-class_q_panda_1_1_origin_c_mem_1a9d9573676ba2cb887d09a68313acb8f0>`(size_t);
		void :target:`cFree<doxid-class_q_panda_1_1_origin_c_mem_1a22f7570b4f6f6af9f7a85f1cb5aeff15>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*);
		void :target:`cFreeAll<doxid-class_q_panda_1_1_origin_c_mem_1a572e2b978e2c3a6568e00acb297308c4>`(std::vector<:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*>&);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_c_mem_1a1c84549b71ef21df3183729c51282266>`() = 0;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_c_mem_1aa8665f1d7d17412ad248b6e457a20fad>`(size_t) = 0;
		virtual size_t :ref:`getMaxMem<doxid-class_q_panda_1_1_c_mem_1a4bf9d89ec9426cd9e93a5564909d44e2>`() const = 0;
		virtual size_t :ref:`getIdleMem<doxid-class_q_panda_1_1_c_mem_1ac26cf626fa7860bd8c9ee943328b08ac>`() const = 0;
		virtual void :ref:`Free_CBit<doxid-class_q_panda_1_1_c_mem_1a1fa4061f315050163260e32160df38ed>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*) = 0;
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_c_mem_1a145989c3b5caec7476f3924aa0ea5551>`() = 0;
		virtual size_t :ref:`get_allocate_cbits<doxid-class_q_panda_1_1_c_mem_1ab6dabe80bb6ef1e4dd3111c89f3f9a40>`(std::vector<:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*>&) = 0;

.. _details-class_q_panda_1_1_origin_c_mem:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`CMem <doxid-class_q_panda_1_1_c_mem>`.

Methods
-------

.. index:: pair: function; Allocate_CBit
.. _doxid-class_q_panda_1_1_origin_c_mem_1a27635c8b914a2e8b01e680e7a2ad731d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* Allocate_CBit()

allocate a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`



.. rubric:: Returns:

CBit\*

.. index:: pair: function; Allocate_CBit
.. _doxid-class_q_panda_1_1_origin_c_mem_1a167dbc305426029d1e474d8bed1e4db7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* Allocate_CBit(size_t)

allocate a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` by bit address



.. rubric:: Returns:

CBit\*

.. index:: pair: function; getMaxMem
.. _doxid-class_q_panda_1_1_origin_c_mem_1a395c37bbc93334fa149a969c9803da48:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getMaxMem() const

get size of the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` vector



.. rubric:: Returns:

size_t

.. index:: pair: function; getIdleMem
.. _doxid-class_q_panda_1_1_origin_c_mem_1ad51e7b4636026398a487b001c5b1d42f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getIdleMem() const

get size of the idle position



.. rubric:: Returns:

size_t

.. index:: pair: function; Free_CBit
.. _doxid-class_q_panda_1_1_origin_c_mem_1a5c4c393aeb4042869582ec59d0b0defb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_CBit(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*)

free a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- CBit\*

		-

.. index:: pair: function; clearAll
.. _doxid-class_q_panda_1_1_origin_c_mem_1ae9bd193eb67a5d51cb9b4e61b055e16a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearAll()

clear the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` vector

.. index:: pair: function; get_allocate_cbits
.. _doxid-class_q_panda_1_1_origin_c_mem_1a57cf999d5dd126a206a0152202cb25bc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_allocate_cbits(std::vector<:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*>&)

get allocate cbits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<CBit

		- \*>&



.. rubric:: Returns:

size_t allocate cbits size

