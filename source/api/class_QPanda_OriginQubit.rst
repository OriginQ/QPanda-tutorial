.. index:: pair: class; QPanda::OriginQubit
.. _doxid-class_q_panda_1_1_origin_qubit:

class QPanda::OriginQubit
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`. :ref:`More...<details-class_q_panda_1_1_origin_qubit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginQubit: public :ref:`QPanda::Qubit<doxid-class_q_panda_1_1_qubit>`
	{
	public:
		// construction
	
		:target:`OriginQubit<doxid-class_q_panda_1_1_origin_qubit_1ad158c0010d48a528da0f07c42a68a85d>`(:ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`*);

		// methods
	
		virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* :ref:`getPhysicalQubitPtr<doxid-class_q_panda_1_1_origin_qubit_1abb1c1b19f7d07496799dac961730dbf2>`();
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_origin_qubit_1a12ebbda1fa9cee68cd1fe898cd2dfb77>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* :ref:`getPhysicalQubitPtr<doxid-class_q_panda_1_1_qubit_1a05b7dd4dcfe023c3f341fc8d09d90943>`() = 0;
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_qubit_1a50abaaae859256175922cae0e07ea9f6>`() = 0;

.. _details-class_q_panda_1_1_origin_qubit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`Qubit <doxid-class_q_panda_1_1_qubit>`.

Methods
-------

.. index:: pair: function; getPhysicalQubitPtr
.. _doxid-class_q_panda_1_1_origin_qubit_1abb1c1b19f7d07496799dac961730dbf2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* getPhysicalQubitPtr()

Get physical qubit pointer.



.. rubric:: Returns:

:ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` \*

.. index:: pair: function; getOccupancy
.. _doxid-class_q_panda_1_1_origin_qubit_1a12ebbda1fa9cee68cd1fe898cd2dfb77:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getOccupancy()

get the occupancy status of this qubit



.. rubric:: Returns:

:ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` \*

