.. index:: pair: struct; QPanda::BasicGridDevice::PhysicalQubit
.. _doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit:

struct QPanda::BasicGridDevice::PhysicalQubit
=============================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <GridDevice.h>
	
	struct PhysicalQubit
	{
		// fields
	
		int :ref:`map_to<doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit_1ac31f8600a0e672b885734c7f439fddee>` = -1;
		int :ref:`time<doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit_1ad7187696f699dd9acfc1db54e3ae0346>`;
		std::vector<std::pair<int, int>> :target:`nearbyQubits<doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit_1ae1e345ca3f94384519236e32f1527dfb>`;
	};
.. _details-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Fields
------

.. index:: pair: variable; map_to
.. _doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit_1ac31f8600a0e672b885734c7f439fddee:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int map_to = -1

which logical qubit maps to it, -1 if no

.. index:: pair: variable; time
.. _doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit_1ad7187696f699dd9acfc1db54e3ae0346:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int time

time when it become free again, the qubit lock

