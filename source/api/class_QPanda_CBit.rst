.. index:: pair: class; QPanda::CBit
.. _doxid-class_q_panda_1_1_c_bit:

class QPanda::CBit
==================

.. toctree::
	:hidden:

Overview
~~~~~~~~

:ref:`CBit <doxid-class_q_panda_1_1_c_bit>` abstract class. :ref:`More...<details-class_q_panda_1_1_c_bit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CBitFactory.h>
	
	class CBit
	{
	public:
		// methods
	
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_c_bit_1a6fafe5bdee6c3903becfdd1af16e8157>`() const = 0;
		virtual std::string :ref:`getName<doxid-class_q_panda_1_1_c_bit_1a62ffbca9662222da8582aa60b41d9d63>`() const = 0;
		virtual void :ref:`setOccupancy<doxid-class_q_panda_1_1_c_bit_1ac24ec9e2a5b8bc32d0f0766c0d93ca9d>`(bool) = 0;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`getValue<doxid-class_q_panda_1_1_c_bit_1ab8a0183794d68e924233374e03807b7a>`() const = 0;
		virtual void :ref:`setValue<doxid-class_q_panda_1_1_c_bit_1a5a45642e44f0ceb077b155100bafcb5d>`(const cbit_size_t) = 0;
	};

	// direct descendants

	class :ref:`OriginCBit<doxid-class_q_panda_1_1_origin_c_bit>`;
.. _details-class_q_panda_1_1_c_bit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`CBit <doxid-class_q_panda_1_1_c_bit>` abstract class.

Methods
-------

.. index:: pair: function; getOccupancy
.. _doxid-class_q_panda_1_1_c_bit_1a6fafe5bdee6c3903becfdd1af16e8157:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getOccupancy() const = 0

get the occupancy status of this bit



.. rubric:: Returns:

bool ture: occupancy

.. index:: pair: function; getName
.. _doxid-class_q_panda_1_1_c_bit_1a62ffbca9662222da8582aa60b41d9d63:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getName() const = 0

get the name of this bit



.. rubric:: Returns:

std::string

.. index:: pair: function; setOccupancy
.. _doxid-class_q_panda_1_1_c_bit_1ac24ec9e2a5b8bc32d0f0766c0d93ca9d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setOccupancy(bool) = 0

set the occupancy status of this bit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- occupancy status

.. index:: pair: function; getValue
.. _doxid-class_q_panda_1_1_c_bit_1ab8a0183794d68e924233374e03807b7a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` getValue() const = 0

get the value of this bit



.. rubric:: Returns:

cbit_size_t

.. index:: pair: function; setValue
.. _doxid-class_q_panda_1_1_c_bit_1a5a45642e44f0ceb077b155100bafcb5d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setValue(const cbit_size_t) = 0

set the value of this bit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cbit_size_t

		- value

