.. index:: pair: class; QPanda::OriginCMemv2
.. _doxid-class_q_panda_1_1_origin_c_memv2:

class QPanda::OriginCMemv2
==========================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginCMemv2: public :ref:`QPanda::CMem<doxid-class_q_panda_1_1_c_mem>`
	{
	public:
		// construction
	
		:target:`OriginCMemv2<doxid-class_q_panda_1_1_origin_c_memv2_1a72d24d1175b83f758997705b83b1d8a4>`(size_t maxMem);

		// methods
	
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_origin_c_memv2_1af0e10fe72a60dcfcb98f2113a2213af4>`();
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`Allocate_CBit<doxid-class_q_panda_1_1_origin_c_memv2_1a47a055272495ac97b17e2c789b6735d7>`(size_t);
		virtual size_t :ref:`getMaxMem<doxid-class_q_panda_1_1_origin_c_memv2_1a9d5e9ef8e7b1fa1f70bd8e74f3ff6e67>`() const;
		virtual size_t :ref:`getIdleMem<doxid-class_q_panda_1_1_origin_c_memv2_1aabe9b6d917ddbea5e29bd18f8c4fcfda>`() const;
		virtual void :ref:`Free_CBit<doxid-class_q_panda_1_1_origin_c_memv2_1a306117651888874ffcbae9298acd20d5>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*);
		virtual void :ref:`clearAll<doxid-class_q_panda_1_1_origin_c_memv2_1a5b8ed3775f5ccdf8d13446490310f4d5>`();
		virtual size_t :ref:`get_allocate_cbits<doxid-class_q_panda_1_1_origin_c_memv2_1a448f9817fabcc89ce0d76462e4e14078>`(std::vector<:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*>&);
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

.. _details-class_q_panda_1_1_origin_c_memv2:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; Allocate_CBit
.. _doxid-class_q_panda_1_1_origin_c_memv2_1af0e10fe72a60dcfcb98f2113a2213af4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* Allocate_CBit()

allocate a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>`



.. rubric:: Returns:

CBit\*

.. index:: pair: function; Allocate_CBit
.. _doxid-class_q_panda_1_1_origin_c_memv2_1a47a055272495ac97b17e2c789b6735d7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* Allocate_CBit(size_t)

allocate a :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` by bit address



.. rubric:: Returns:

CBit\*

.. index:: pair: function; getMaxMem
.. _doxid-class_q_panda_1_1_origin_c_memv2_1a9d5e9ef8e7b1fa1f70bd8e74f3ff6e67:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getMaxMem() const

get size of the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` vector



.. rubric:: Returns:

size_t

.. index:: pair: function; getIdleMem
.. _doxid-class_q_panda_1_1_origin_c_memv2_1aabe9b6d917ddbea5e29bd18f8c4fcfda:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getIdleMem() const

get size of the idle position



.. rubric:: Returns:

size_t

.. index:: pair: function; Free_CBit
.. _doxid-class_q_panda_1_1_origin_c_memv2_1a306117651888874ffcbae9298acd20d5:

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
.. _doxid-class_q_panda_1_1_origin_c_memv2_1a5b8ed3775f5ccdf8d13446490310f4d5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearAll()

clear the :ref:`CBit <doxid-class_q_panda_1_1_c_bit>` vector

.. index:: pair: function; get_allocate_cbits
.. _doxid-class_q_panda_1_1_origin_c_memv2_1a448f9817fabcc89ce0d76462e4e14078:

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

