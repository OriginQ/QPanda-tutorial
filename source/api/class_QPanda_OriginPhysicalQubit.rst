.. index:: pair: class; QPanda::OriginPhysicalQubit
.. _doxid-class_q_panda_1_1_origin_physical_qubit:

class QPanda::OriginPhysicalQubit
=================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>`. :ref:`More...<details-class_q_panda_1_1_origin_physical_qubit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginPhysicalQubit: public :ref:`QPanda::PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`
	{
	public:
		// methods
	
		virtual size_t :ref:`getQubitAddr<doxid-class_q_panda_1_1_origin_physical_qubit_1aa92805374589a1b9bfdd531a94312168>`();
		virtual void :ref:`setQubitAddr<doxid-class_q_panda_1_1_origin_physical_qubit_1a571d6785e881a7bb5ef0121406808695>`(size_t);
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_origin_physical_qubit_1ae1870170a2429c77b0000fd0a481a898>`() const;
		virtual void :ref:`setOccupancy<doxid-class_q_panda_1_1_origin_physical_qubit_1accbe26032df20d4d45997c30437aebe2>`(bool);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual size_t :ref:`getQubitAddr<doxid-class_q_panda_1_1_physical_qubit_1a59dc876e5d4ef1a7626bfba6bcde7752>`() = 0;
		virtual void :ref:`setQubitAddr<doxid-class_q_panda_1_1_physical_qubit_1a71c515f87d4c308472f28226e6212f49>`(size_t) = 0;
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_physical_qubit_1a255b36c8151510d8cce3794e63778871>`() const = 0;
		virtual void :ref:`setOccupancy<doxid-class_q_panda_1_1_physical_qubit_1a26a63093fd834f86439800bebe9a8c42>`(bool) = 0;

.. _details-class_q_panda_1_1_origin_physical_qubit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>`.

Methods
-------

.. index:: pair: function; getQubitAddr
.. _doxid-class_q_panda_1_1_origin_physical_qubit_1aa92805374589a1b9bfdd531a94312168:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getQubitAddr()

get qubit address



.. rubric:: Returns:

size_t

.. index:: pair: function; setQubitAddr
.. _doxid-class_q_panda_1_1_origin_physical_qubit_1a571d6785e881a7bb5ef0121406808695:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setQubitAddr(size_t)

set qubit address



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

.. index:: pair: function; getOccupancy
.. _doxid-class_q_panda_1_1_origin_physical_qubit_1ae1870170a2429c77b0000fd0a481a898:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getOccupancy() const

get the occupancy status of this qubit



.. rubric:: Returns:

bool ture: occupancy

.. index:: pair: function; setOccupancy
.. _doxid-class_q_panda_1_1_origin_physical_qubit_1accbe26032df20d4d45997c30437aebe2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setOccupancy(bool)

set the occupancy status of this qubit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- occupancy status

