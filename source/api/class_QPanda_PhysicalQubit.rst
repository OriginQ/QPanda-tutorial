.. index:: pair: class; QPanda::PhysicalQubit
.. _doxid-class_q_panda_1_1_physical_qubit:

class QPanda::PhysicalQubit
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Physical :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` abstract class. :ref:`More...<details-class_q_panda_1_1_physical_qubit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <PhysicalQubitFactory.h>
	
	class PhysicalQubit
	{
	public:
		// methods
	
		virtual size_t :ref:`getQubitAddr<doxid-class_q_panda_1_1_physical_qubit_1a59dc876e5d4ef1a7626bfba6bcde7752>`() = 0;
		virtual void :ref:`setQubitAddr<doxid-class_q_panda_1_1_physical_qubit_1a71c515f87d4c308472f28226e6212f49>`(size_t) = 0;
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_physical_qubit_1a255b36c8151510d8cce3794e63778871>`() const = 0;
		virtual void :ref:`setOccupancy<doxid-class_q_panda_1_1_physical_qubit_1a26a63093fd834f86439800bebe9a8c42>`(bool) = 0;
	};

	// direct descendants

	class :ref:`OriginPhysicalQubit<doxid-class_q_panda_1_1_origin_physical_qubit>`;
.. _details-class_q_panda_1_1_physical_qubit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Physical :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` abstract class.

Methods
-------

.. index:: pair: function; getQubitAddr
.. _doxid-class_q_panda_1_1_physical_qubit_1a59dc876e5d4ef1a7626bfba6bcde7752:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getQubitAddr() = 0

get qubit address



.. rubric:: Returns:

size_t

.. index:: pair: function; setQubitAddr
.. _doxid-class_q_panda_1_1_physical_qubit_1a71c515f87d4c308472f28226e6212f49:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setQubitAddr(size_t) = 0

set qubit address



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

.. index:: pair: function; getOccupancy
.. _doxid-class_q_panda_1_1_physical_qubit_1a255b36c8151510d8cce3794e63778871:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getOccupancy() const = 0

get the occupancy status of this qubit



.. rubric:: Returns:

bool ture: occupancy

.. index:: pair: function; setOccupancy
.. _doxid-class_q_panda_1_1_physical_qubit_1a26a63093fd834f86439800bebe9a8c42:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setOccupancy(bool) = 0

set the occupancy status of this qubit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- occupancy status

