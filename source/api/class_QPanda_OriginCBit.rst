.. index:: pair: class; QPanda::OriginCBit
.. _doxid-class_q_panda_1_1_origin_c_bit:

class QPanda::OriginCBit
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`. :ref:`More...<details-class_q_panda_1_1_origin_c_bit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginCBit: public :ref:`QPanda::CBit<doxid-class_q_panda_1_1_c_bit>`
	{
	public:
		// construction
	
		:target:`OriginCBit<doxid-class_q_panda_1_1_origin_c_bit_1ac8ba9d25d5a8500553964992f4cf720c>`(std::string name);

		// methods
	
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_origin_c_bit_1af569ca8358f2b07816fc7d8b7b06bb38>`() const;
		virtual void :ref:`setOccupancy<doxid-class_q_panda_1_1_origin_c_bit_1af7568a94d1d2bc2adfcc02f5d625feae>`(bool);
		virtual std::string :ref:`getName<doxid-class_q_panda_1_1_origin_c_bit_1ab5169c6b1870442c9534c631205841d3>`() const;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`getValue<doxid-class_q_panda_1_1_origin_c_bit_1a398668e0e9c798941fd12f026fe23860>`() const;
		virtual void :ref:`setValue<doxid-class_q_panda_1_1_origin_c_bit_1a7461d85dfbcdc5496ec11e518168b6f9>`(const :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` cbit_size_t);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_c_bit_1a6fafe5bdee6c3903becfdd1af16e8157>`() const = 0;
		virtual std::string :ref:`getName<doxid-class_q_panda_1_1_c_bit_1a62ffbca9662222da8582aa60b41d9d63>`() const = 0;
		virtual void :ref:`setOccupancy<doxid-class_q_panda_1_1_c_bit_1ac24ec9e2a5b8bc32d0f0766c0d93ca9d>`(bool) = 0;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`getValue<doxid-class_q_panda_1_1_c_bit_1ab8a0183794d68e924233374e03807b7a>`() const = 0;
		virtual void :ref:`setValue<doxid-class_q_panda_1_1_c_bit_1a5a45642e44f0ceb077b155100bafcb5d>`(const cbit_size_t) = 0;

.. _details-class_q_panda_1_1_origin_c_bit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`.

Methods
-------

.. index:: pair: function; getOccupancy
.. _doxid-class_q_panda_1_1_origin_c_bit_1af569ca8358f2b07816fc7d8b7b06bb38:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getOccupancy() const

get the occupancy status of this bit



.. rubric:: Returns:

bool ture: occupancy

.. index:: pair: function; setOccupancy
.. _doxid-class_q_panda_1_1_origin_c_bit_1af7568a94d1d2bc2adfcc02f5d625feae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setOccupancy(bool)

set the occupancy status of this bit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- occupancy status

.. index:: pair: function; getName
.. _doxid-class_q_panda_1_1_origin_c_bit_1ab5169c6b1870442c9534c631205841d3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getName() const

get the name of this bit



.. rubric:: Returns:

std::string

.. index:: pair: function; getValue
.. _doxid-class_q_panda_1_1_origin_c_bit_1a398668e0e9c798941fd12f026fe23860:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` getValue() const

get the value of this bit



.. rubric:: Returns:

cbit_size_t

.. index:: pair: function; setValue
.. _doxid-class_q_panda_1_1_origin_c_bit_1a7461d85dfbcdc5496ec11e518168b6f9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setValue(const :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` cbit_size_t)

set the value of this bit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cbit_size_t

		- value

