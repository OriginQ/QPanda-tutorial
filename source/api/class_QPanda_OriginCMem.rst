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
		// construction
	
		:target:`OriginCMem<doxid-class_q_panda_1_1_origin_c_mem_1ac68231a25bfc8e7994b60776bf237f1a>`(size_t maxMem);

		// methods
	
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_origin_c_mem_1a27635c8b914a2e8b01e680e7a2ad731d>`();
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_origin_c_mem_1a167dbc305426029d1e474d8bed1e4db7>`(size_t);
		virtual size_t :ref:`getMaxMem<doxid-class_q_panda_1_1_origin_c_mem_1a395c37bbc93334fa149a969c9803da48>`() const;
		virtual size_t :ref:`getIdleMem<doxid-class_q_panda_1_1_origin_c_mem_1ad51e7b4636026398a487b001c5b1d42f>`() const;
		virtual void :ref:`Free_CBit<doxid-class_q_panda_1_1_origin_c_mem_1a5c4c393aeb4042869582ec59d0b0defb>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*);
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_origin_c_mem_1ae9bd193eb67a5d51cb9b4e61b055e16a>`();
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

