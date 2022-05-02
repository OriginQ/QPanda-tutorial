.. index:: pair: class; QPanda::Variational::VariationalQuantumGate_U1
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1:

class QPanda::Variational::VariationalQuantumGate_U1
====================================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	class VariationalQuantumGate_U1: public :ref:`QPanda::Variational::VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`
	{
	public:
		// construction
	
		:target:`VariationalQuantumGate_U1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1ac194d030ff4bc983984b359fd00040e1>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*,
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`
			);
	
		:target:`VariationalQuantumGate_U1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1a2aa4aedb12bded60b59c73f37889a097>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*,
			double angle
			);
	
		:target:`VariationalQuantumGate_U1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1aac0df3f4e4de6dd7b37ca34645ed1e72>`(const VariationalQuantumGate_U1& gate);

		// methods
	
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1a067438675b4c204ef321708e8c904f32>`();
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1a1f972e633ec57ce39dcce3acddbdd864>`(std::map<size_t, double> offset);
		virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> :ref:`copy<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1ad94b645b6aa68a0e33de42957b5505c0>`();
		VariationalQuantumGate_U1 :target:`dagger<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1a2287be661bb7dcfb25c1ed987dfdf6be>`();
		VariationalQuantumGate_U1 :target:`control<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1afd62866bafc30bc62eb07a68723c7077>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qv);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		size_t :ref:`n_var<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a94e84e5572d19b6f4017e15671cc8fc1>`();
		const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& :ref:`get_vars<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a040e35879202ce657c995466e9a64e04>`();
		const std::vector<double>& :ref:`get_constants<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aed2ab2281bc321a0e964473be6cfcc35>`();
		int :ref:`var_pos<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a289faed2739b91d54ea82d7a72aa4beb>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` _var);
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1ad331ff4076e3ad2e6108ebb270dc4947>`() = 0;
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1af174cd439585ec3b29f4b1360d3ecd90>`(std::map<size_t, double> offset);
		virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> :ref:`copy<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aa135247611e3a0f49af4a15734f3505f>`() = 0;
		virtual bool :ref:`set_dagger<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1afed11fe49d8001f62cfe7ab4586d54de>`(bool dagger);
		virtual bool :ref:`set_control<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1abb9d281d38884a750e2e0b80af4e7e20>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` control_qubit);
		virtual bool :ref:`is_dagger<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a2dad50fec23fd4383e94b019e980a5cb>`();
		virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`get_control_qubit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aa7d2fd40c59539a415039e876cb701b3>`();
		virtual void :ref:`copy_dagger_and_control_qubit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1afb798617339f0ac98f9bd4bc5d73c34f>`(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate);
		virtual void :ref:`copy_dagger_and_control_qubit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a7bba6ce2dfc554c5f4c452007dcdfb9f>`(std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> gate);

.. _details-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; feed
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1a067438675b4c204ef321708e8c904f32:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` feed()

Interface to instantialize the :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` with VQG.



.. rubric:: Returns:

:ref:`QGate <doxid-class_q_panda_1_1_q_gate>` Instantiation

.. index:: pair: function; feed
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1a1f972e633ec57ce39dcce3acddbdd864:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` feed(std::map<size_t, double> offset)

Interface to instantialize the :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` with the "offset".



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- offset

		- <number of variable, offset>



.. rubric:: Returns:

:ref:`QGate <doxid-class_q_panda_1_1_q_gate>`

.. index:: pair: function; copy
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1_1ad94b645b6aa68a0e33de42957b5505c0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> copy()

Interface to copy the instance, and return a shared_ptr for the object.



.. rubric:: Returns:

std::shared_ptr<VariationalQuantumGate>

