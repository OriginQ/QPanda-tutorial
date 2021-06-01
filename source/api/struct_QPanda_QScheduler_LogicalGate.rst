.. index:: pair: struct; QPanda::QScheduler::LogicalGate
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate:

struct QPanda::QScheduler::LogicalGate
======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

logical gate :ref:`More...<details-struct_q_panda_1_1_q_scheduler_1_1_logical_gate>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QScheduler.h>
	
	struct LogicalGate
	{
		// fields
	
		int :ref:`t<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1a944c20a5975deef8ac2b52f95becbaa8>`;
		int :ref:`c<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1aa20140a3fe4cadb09f4eb2f1ebdeb7aa>`;
		std::string :ref:`gate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1afe8cfb0b223a262490027cb6b2893513>`;
		int :ref:`gate_type<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1af8d83dcc88845d1312daba612b1ce7f6>`;
		bool :target:`is_dagger<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1a27a7c9f5878f9cac7811d1ec4f56faf8>`;
		std::vector<double> :target:`param<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1a3d91eac0f008477d33b0369f9ff6e4e3>`;
		int :target:`barrier_id<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1a6f3a6eed7b32520c9349e3ca19ab5e30>`;

		// construction
	
		:ref:`LogicalGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1aa0bb52912685b6a3d0d63e88753e6c09>`(
			std::string gate,
			int gate_type,
			int c,
			int t,
			std::vector<double> param,
			int barrier_id,
			bool is_dagger
			);

		// methods
	
		bool :target:`isSingleQubitGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1aa550acff038d570f11d8090e6667bab3>`() const;
	};
.. _details-struct_q_panda_1_1_q_scheduler_1_1_logical_gate:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

logical gate

Fields
------

.. index:: pair: variable; t
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1a944c20a5975deef8ac2b52f95becbaa8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int t

index of the target qubit

.. index:: pair: variable; c
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1aa20140a3fe4cadb09f4eb2f1ebdeb7aa:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int c

index of the control qubit, c = -1 for single qubit gate

.. index:: pair: variable; gate
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1afe8cfb0b223a262490027cb6b2893513:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string gate

type of the gate

.. index:: pair: variable; gate_type
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1af8d83dcc88845d1312daba612b1ce7f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int gate_type

these parameters can be encapsulated

Construction
------------

.. index:: pair: function; LogicalGate
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate_1aa0bb52912685b6a3d0d63e88753e6c09:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	LogicalGate(
		std::string gate,
		int gate_type,
		int c,
		int t,
		std::vector<double> param,
		int barrier_id,
		bool is_dagger
		)

create a gate

