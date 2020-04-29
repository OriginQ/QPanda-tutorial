.. index:: pair: class; QPanda::Configuration
.. _doxid-struct_q_panda_1_1_configuration:

class QPanda::Configuration
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum qubit and cbit :ref:`Configuration <doxid-struct_q_panda_1_1_configuration>`. :ref:`More...<details-struct_q_panda_1_1_configuration>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMachineInterface.h>
	
	class Configuration
	{
	public:
		// fields
	
		size_t :ref:`maxQubit<doxid-struct_q_panda_1_1_configuration_1af9956cbee0b8c74060c5bcc04145d7d1>`;
		size_t :ref:`maxCMem<doxid-struct_q_panda_1_1_configuration_1aa1b780159354441b758013bc17c7b221>`;
	};
.. _details-struct_q_panda_1_1_configuration:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum qubit and cbit :ref:`Configuration <doxid-struct_q_panda_1_1_configuration>`.

Default number is 25



.. rubric:: See also:

:ref:`QVM <doxid-class_q_panda_1_1_q_v_m>`

Fields
------

.. index:: pair: variable; maxQubit
.. _doxid-struct_q_panda_1_1_configuration_1af9956cbee0b8c74060c5bcc04145d7d1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t maxQubit

Config max qubit num

.. index:: pair: variable; maxCMem
.. _doxid-struct_q_panda_1_1_configuration_1aa1b780159354441b758013bc17c7b221:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t maxCMem

Config max cbit num

