.. index:: pair: struct; QPanda::QScheduler::PhysicsGate
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate:

struct QPanda::QScheduler::PhysicsGate
======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

physical gate :ref:`More...<details-struct_q_panda_1_1_q_scheduler_1_1_physics_gate>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QScheduler.h>
	
	struct PhysicsGate
	{
		// fields
	
		std::string :target:`type<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a1607a42a4ca028b4a4e2938ad4f717d5>`;
		int :target:`gate_type<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1aa575e9d2e5d913556148b6a3fa001c99>`;
		bool :target:`is_dagger<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a86a48362a90b86e73f2fa03448e9d28d>`;
		std::vector<double> :target:`param<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1ac267517f28e389896a686b7c1ec0c381>`;
		bool :target:`is_apply_swap<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1ae3af1b9f832b281df236eeffbedad94d>`;
		int :target:`i1<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a381acafeeab418b49d0dba601ec1e038>`;
		int :ref:`j1<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a2f50314b34577f38b319ea4a68337473>`;
		int :target:`i2<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1ad92284b8ac8648918560d6431c74e387>`;
		int :ref:`j2<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a0274f7ceeeceba69f52d93e108d7e7b1>`;
		int :target:`barrier_id<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a7f7044ba40b5730bfb9b9177c3ae7c56>`;

		// methods
	
		bool :target:`isSwapGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1ab4973dbf1341a0ff9f7f61162549bd09>`();
		bool :target:`isControlGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a7d8f364ff33bd3774dd1f9bf9ba2ebac>`();
	};
.. _details-struct_q_panda_1_1_q_scheduler_1_1_physics_gate:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

physical gate

Fields
------

.. index:: pair: variable; j1
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a2f50314b34577f38b319ea4a68337473:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int j1

(i1, j1) is the position for the first qubit parament of the gate

.. index:: pair: variable; j2
.. _doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate_1a0274f7ceeeceba69f52d93e108d7e7b1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int j2

(i2, j2) is the position for the first qubit parament of the two-qubit gate

