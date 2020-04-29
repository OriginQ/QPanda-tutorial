.. index:: pair: class; QPanda::CMem
.. _doxid-class_q_panda_1_1_c_mem:

class QPanda::CMem
==================

.. toctree::
	:hidden:

Overview
~~~~~~~~

:ref:`CMem <doxid-class_q_panda_1_1_c_mem>` abstract class, this class is considered as the container of the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`. :ref:`More...<details-class_q_panda_1_1_c_mem>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CMemFactory.h>
	
	class CMem
	{
	public:
		// methods
	
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_c_mem_1a1c84549b71ef21df3183729c51282266>`() = 0;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_c_mem_1aa8665f1d7d17412ad248b6e457a20fad>`(size_t) = 0;
		virtual size_t :ref:`getMaxMem<doxid-class_q_panda_1_1_c_mem_1a4bf9d89ec9426cd9e93a5564909d44e2>`() const = 0;
		virtual size_t :ref:`getIdleMem<doxid-class_q_panda_1_1_c_mem_1ac26cf626fa7860bd8c9ee943328b08ac>`() const = 0;
		virtual void :ref:`Free_CBit<doxid-class_q_panda_1_1_c_mem_1a1fa4061f315050163260e32160df38ed>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*) = 0;
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_c_mem_1a145989c3b5caec7476f3924aa0ea5551>`() = 0;
	};

	// direct descendants

	class :ref:`OriginCMem<doxid-class_q_panda_1_1_origin_c_mem>`;
.. _details-class_q_panda_1_1_c_mem:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`CMem <doxid-class_q_panda_1_1_c_mem>` abstract class, this class is considered as the container of the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`.

Methods
-------

.. index:: pair: function; Allocate_CBit
.. _doxid-class_q_panda_1_1_c_mem_1a1c84549b71ef21df3183729c51282266:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* Allocate_CBit() = 0

allocate a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`



.. rubric:: Returns:

CBit\*

.. index:: pair: function; Allocate_CBit
.. _doxid-class_q_panda_1_1_c_mem_1aa8665f1d7d17412ad248b6e457a20fad:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* Allocate_CBit(size_t) = 0

allocate a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` by bit address



.. rubric:: Returns:

CBit\*

.. index:: pair: function; getMaxMem
.. _doxid-class_q_panda_1_1_c_mem_1a4bf9d89ec9426cd9e93a5564909d44e2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getMaxMem() const = 0

get size of the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` vector



.. rubric:: Returns:

size_t

.. index:: pair: function; getIdleMem
.. _doxid-class_q_panda_1_1_c_mem_1ac26cf626fa7860bd8c9ee943328b08ac:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getIdleMem() const = 0

get size of the idle position



.. rubric:: Returns:

size_t

.. index:: pair: function; Free_CBit
.. _doxid-class_q_panda_1_1_c_mem_1a1fa4061f315050163260e32160df38ed:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void Free_CBit(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*) = 0

free a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- CBit\*

		-

.. index:: pair: function; clearAll
.. _doxid-class_q_panda_1_1_c_mem_1a145989c3b5caec7476f3924aa0ea5551:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearAll() = 0

clear the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` vector

