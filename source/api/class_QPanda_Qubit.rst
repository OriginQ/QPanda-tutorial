.. index:: pair: class; QPanda::Qubit
.. _doxid-class_q_panda_1_1_qubit:

class QPanda::Qubit
===================

.. toctree::
	:hidden:

Overview
~~~~~~~~

:ref:`Qubit <doxid-class_q_panda_1_1_qubit>` abstract class. :ref:`More...<details-class_q_panda_1_1_qubit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitFactory.h>
	
	class Qubit
	{
	public:
		// methods
	
		virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* :ref:`getPhysicalQubitPtr<doxid-class_q_panda_1_1_qubit_1ab5238f42f6dbbc19b127d80979ee654a>`() const = 0;
		virtual size_t :ref:`get_phy_addr<doxid-class_q_panda_1_1_qubit_1a3dbdbfb4b2ba305204e703b75e95d7f9>`() const;
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_qubit_1a50abaaae859256175922cae0e07ea9f6>`() = 0;
	};

	// direct descendants

	class :ref:`OriginQubit<doxid-class_q_panda_1_1_origin_qubit>`;
	class :ref:`QubitReference<doxid-class_q_panda_1_1_qubit_reference>`;
.. _details-class_q_panda_1_1_qubit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`Qubit <doxid-class_q_panda_1_1_qubit>` abstract class.

Methods
-------

.. index:: pair: function; getPhysicalQubitPtr
.. _doxid-class_q_panda_1_1_qubit_1ab5238f42f6dbbc19b127d80979ee654a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* getPhysicalQubitPtr() const = 0

Get physical qubit pointer.



.. rubric:: Returns:

:ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` \*

.. index:: pair: function; get_phy_addr
.. _doxid-class_q_panda_1_1_qubit_1a3dbdbfb4b2ba305204e703b75e95d7f9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_phy_addr() const

Get physical addr.



.. rubric:: Returns:

size_t

.. index:: pair: function; getOccupancy
.. _doxid-class_q_panda_1_1_qubit_1a50abaaae859256175922cae0e07ea9f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getOccupancy() = 0

get the occupancy status of this qubit



.. rubric:: Returns:

:ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` \*

