.. index:: pair: class; QPanda::BasicGridDevice
.. _doxid-class_q_panda_1_1_basic_grid_device:

class QPanda::BasicGridDevice
=============================

.. toctree::
	:hidden:

	struct_QPanda_BasicGridDevice_PhysicalQubit.rst

Overview
~~~~~~~~

A BasicGirdDevice is a device model that qubits put on nodes of a rectangular grid It is a virtual class because we haven't dicided how qubits connecting with each other For the simpliest situation, see :ref:`SimpleGridDevice <doxid-class_q_panda_1_1_simple_grid_device>`. :ref:`More...<details-class_q_panda_1_1_basic_grid_device>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <GridDevice.h>
	
	class BasicGridDevice
	{
	public:
		// structs
	
		struct :ref:`PhysicalQubit<doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit>`;

		// construction
	
		:ref:`BasicGridDevice<doxid-class_q_panda_1_1_basic_grid_device_1a1e09ced2a5c390a0e129caa02d8c8419>`(int m, int n);

		// methods
	
		void :ref:`clear<doxid-class_q_panda_1_1_basic_grid_device_1a09714a4863204df35d7eb25b8cf62659>`();
		int :target:`getM<doxid-class_q_panda_1_1_basic_grid_device_1a4580350edef0102343846a7859ae8660>`();
		int :target:`getN<doxid-class_q_panda_1_1_basic_grid_device_1a7a8225fdebcd7613e91b7e90f66c8f42>`();
		auto& :ref:`getQubit<doxid-class_q_panda_1_1_basic_grid_device_1a5a459002641fd59163c9e401432f3067>`(int i, int j);
		bool :ref:`canApplyGate<doxid-class_q_panda_1_1_basic_grid_device_1a8503407bf9a2886c42df382a06ab8d26>`(int i1, int j1, int i2, int j2, int);
		bool :ref:`canApplyGate<doxid-class_q_panda_1_1_basic_grid_device_1a1742ac2b23467a88d610d0126dc75cae>`(int i, int j, int);
	
		bool :target:`canSwap<doxid-class_q_panda_1_1_basic_grid_device_1a76a46b2811d866d2091f218f90674e03>`(
			int i1,
			int j1,
			int i2,
			int j2
			);
	
		void :ref:`applySingleGate<doxid-class_q_panda_1_1_basic_grid_device_1a8009420486f96cc0d115dfe8c8529a45>`(int i, int j);
		void :ref:`applyGate<doxid-class_q_panda_1_1_basic_grid_device_1a80b82b2592f6c40f0aa6198b60f7a299>`(int i1, int j1, int i2, int j2, int time);
	
		void :target:`applyDoubleGate<doxid-class_q_panda_1_1_basic_grid_device_1a3e3eae315a5215d359b061bc9a204d54>`(
			int i1,
			int j1,
			int i2,
			int j2
			);
	
		void :target:`applySwap<doxid-class_q_panda_1_1_basic_grid_device_1ad29ed551bb09088370097b93e3987f30>`(
			int i1,
			int j1,
			int i2,
			int j2
			);
	
		virtual bool :ref:`isNearBy<doxid-class_q_panda_1_1_basic_grid_device_1ad876b3453ae76379e449267a8cfcb3f4>`(int i1, int j1, int i2, int j2) = 0;
		virtual int :ref:`getDistance<doxid-class_q_panda_1_1_basic_grid_device_1aae022b1fcadc203e9d3a92b9ab57afe5>`(int i1, int j1, int i2, int j2) = 0;
		void :ref:`map<doxid-class_q_panda_1_1_basic_grid_device_1acf0aea261a0e455057e23901c170b78e>`(int dest, int i, int j);
		void :ref:`resetTime<doxid-class_q_panda_1_1_basic_grid_device_1a4e341e62b3a245f3a7dba6607458a2a9>`();
		void :ref:`nextCycle<doxid-class_q_panda_1_1_basic_grid_device_1af9af37dfc8f684a1a42fdcef19509ede>`();
		int :ref:`maxTime<doxid-class_q_panda_1_1_basic_grid_device_1a809242f417ef1be38236a72963553cae>`();
		int :target:`getTime<doxid-class_q_panda_1_1_basic_grid_device_1af8e0c15aa673ab3ddc97674bda1b638c>`();
		bool :ref:`isQubitFree<doxid-class_q_panda_1_1_basic_grid_device_1ae55c1f5d2e3f711d775ad7c2ea1a2e5b>`(int i, int j);
		bool :ref:`isAllQubitFree<doxid-class_q_panda_1_1_basic_grid_device_1a5397662e8b72e6e7d7578f4ee9bb74a7>`();
		bool :target:`isSimpleGridDevice<doxid-class_q_panda_1_1_basic_grid_device_1a31d1b5609b7ae5054a52fcc60bc21563>`();
		bool :target:`isSupportSwapGate<doxid-class_q_panda_1_1_basic_grid_device_1a3d340361c313fd45466f2971e8fce525>`();
	};

	// direct descendants

	class :ref:`ExGridDevice<doxid-class_q_panda_1_1_ex_grid_device>`;
	class :ref:`SimpleGridDevice<doxid-class_q_panda_1_1_simple_grid_device>`;
.. _details-class_q_panda_1_1_basic_grid_device:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A BasicGirdDevice is a device model that qubits put on nodes of a rectangular grid It is a virtual class because we haven't dicided how qubits connecting with each other For the simpliest situation, see :ref:`SimpleGridDevice <doxid-class_q_panda_1_1_simple_grid_device>`.

Construction
------------

.. index:: pair: function; BasicGridDevice
.. _doxid-class_q_panda_1_1_basic_grid_device_1a1e09ced2a5c390a0e129caa02d8c8419:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	BasicGridDevice(int m, int n)

constructor constructor

m, n: the grid side length

Methods
-------

.. index:: pair: function; clear
.. _doxid-class_q_panda_1_1_basic_grid_device_1a09714a4863204df35d7eb25b8cf62659:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void clear()

clear all properties except gird side length, re-initialize

.. index:: pair: function; getQubit
.. _doxid-class_q_panda_1_1_basic_grid_device_1a5a459002641fd59163c9e401432f3067:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	auto& getQubit(int i, int j)

get the qubit on (i, j)

.. index:: pair: function; canApplyGate
.. _doxid-class_q_panda_1_1_basic_grid_device_1a8503407bf9a2886c42df382a06ab8d26:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool canApplyGate(int i1, int j1, int i2, int j2, int)

Determine whether a double-qubit gate can be applied.

.. index:: pair: function; canApplyGate
.. _doxid-class_q_panda_1_1_basic_grid_device_1a1742ac2b23467a88d610d0126dc75cae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool canApplyGate(int i, int j, int)

Determine whether a single-qubit gate can be applied.

.. index:: pair: function; applySingleGate
.. _doxid-class_q_panda_1_1_basic_grid_device_1a8009420486f96cc0d115dfe8c8529a45:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void applySingleGate(int i, int j)

apply gate and comsume time

.. index:: pair: function; applyGate
.. _doxid-class_q_panda_1_1_basic_grid_device_1a80b82b2592f6c40f0aa6198b60f7a299:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void applyGate(int i1, int j1, int i2, int j2, int time)

apply a double-qubit gate

.. index:: pair: function; isNearBy
.. _doxid-class_q_panda_1_1_basic_grid_device_1ad876b3453ae76379e449267a8cfcb3f4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool isNearBy(int i1, int j1, int i2, int j2) = 0

Check if two qubits are adjacent, location of qubits are (i1, j1) and (i2, j2)

.. index:: pair: function; getDistance
.. _doxid-class_q_panda_1_1_basic_grid_device_1aae022b1fcadc203e9d3a92b9ab57afe5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int getDistance(int i1, int j1, int i2, int j2) = 0

get distance+1 of two qubits

.. index:: pair: function; map
.. _doxid-class_q_panda_1_1_basic_grid_device_1acf0aea261a0e455057e23901c170b78e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void map(int dest, int i, int j)

map one qubit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- dest: index of the logical qubit

	*
		- int

		- i: location of the physical qubit

	*
		- int

		- j: location of the physical qubit

.. index:: pair: function; resetTime
.. _doxid-class_q_panda_1_1_basic_grid_device_1a4e341e62b3a245f3a7dba6607458a2a9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void resetTime()

reset the time

.. index:: pair: function; nextCycle
.. _doxid-class_q_panda_1_1_basic_grid_device_1af9af37dfc8f684a1a42fdcef19509ede:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void nextCycle()

go on next instruction cycle

.. index:: pair: function; maxTime
.. _doxid-class_q_panda_1_1_basic_grid_device_1a809242f417ef1be38236a72963553cae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int maxTime()

time when all qubits end up being busy

.. index:: pair: function; isQubitFree
.. _doxid-class_q_panda_1_1_basic_grid_device_1ae55c1f5d2e3f711d775ad7c2ea1a2e5b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isQubitFree(int i, int j)

check if physical qubit on (i, j) free

.. index:: pair: function; isAllQubitFree
.. _doxid-class_q_panda_1_1_basic_grid_device_1a5397662e8b72e6e7d7578f4ee9bb74a7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isAllQubitFree()

check if all physical qubits free

