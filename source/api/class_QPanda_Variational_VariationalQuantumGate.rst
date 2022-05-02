.. index:: pair: class; QPanda::Variational::VariationalQuantumGate
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate:

class QPanda::Variational::VariationalQuantumGate
=================================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	class VariationalQuantumGate
	{
	public:
		// construction
	
		:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a44eadb3fe9594c0cc691c2d1b06cd658>`(const VariationalQuantumGate&);
		:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a2a29b7083325db10b62755ae610d2a35>`();

		// methods
	
		size_t :ref:`n_var<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a94e84e5572d19b6f4017e15671cc8fc1>`();
		const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& :ref:`get_vars<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a040e35879202ce657c995466e9a64e04>`();
		const std::vector<double>& :target:`get_constants<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aed2ab2281bc321a0e964473be6cfcc35>`();
		int :ref:`var_pos<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a289faed2739b91d54ea82d7a72aa4beb>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` _var);
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1ad331ff4076e3ad2e6108ebb270dc4947>`() = 0;
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1af174cd439585ec3b29f4b1360d3ecd90>`(std::map<size_t, double> offset);
		virtual std::shared_ptr<VariationalQuantumGate> :ref:`copy<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aa135247611e3a0f49af4a15734f3505f>`() = 0;
		virtual bool :target:`set_dagger<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1afed11fe49d8001f62cfe7ab4586d54de>`(bool dagger);
		virtual bool :target:`set_control<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1abb9d281d38884a750e2e0b80af4e7e20>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` control_qubit);
		virtual bool :target:`is_dagger<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a2dad50fec23fd4383e94b019e980a5cb>`();
		virtual :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`get_control_qubit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aa7d2fd40c59539a415039e876cb701b3>`();
		virtual void :target:`copy_dagger_and_control_qubit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1afb798617339f0ac98f9bd4bc5d73c34f>`(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate);
		virtual void :target:`copy_dagger_and_control_qubit<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a7bba6ce2dfc554c5f4c452007dcdfb9f>`(std::shared_ptr<VariationalQuantumGate> gate);
	};

	// direct descendants

	class :ref:`VariationalQuantumGate_CNOT<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_n_o_t>`;
	class :ref:`VariationalQuantumGate_CR<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r>`;
	class :ref:`VariationalQuantumGate_CRX<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_x>`;
	class :ref:`VariationalQuantumGate_CRY<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_y>`;
	class :ref:`VariationalQuantumGate_CRZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_r_z>`;
	class :ref:`VariationalQuantumGate_CU<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_u>`;
	class :ref:`VariationalQuantumGate_CZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___c_z>`;
	class :ref:`VariationalQuantumGate_H<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___h>`;
	class :ref:`VariationalQuantumGate_iSWAP<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate__i_s_w_a_p>`;
	class :ref:`VariationalQuantumGate_RPhi<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_phi>`;
	class :ref:`VariationalQuantumGate_RX<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_x>`;
	class :ref:`VariationalQuantumGate_RY<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_y>`;
	class :ref:`VariationalQuantumGate_RZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z>`;
	class :ref:`VariationalQuantumGate_S<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___s>`;
	class :ref:`VariationalQuantumGate_SqiSWAP<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___sqi_s_w_a_p>`;
	class :ref:`VariationalQuantumGate_SWAP<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___s_w_a_p>`;
	class :ref:`VariationalQuantumGate_T<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___t>`;
	class :ref:`VariationalQuantumGate_U1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u1>`;
	class :ref:`VariationalQuantumGate_U2<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u2>`;
	class :ref:`VariationalQuantumGate_U3<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u3>`;
	class :ref:`VariationalQuantumGate_U4<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___u4>`;
	class :ref:`VariationalQuantumGate_X<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___x>`;
	class :ref:`VariationalQuantumGate_X1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___x1>`;
	class :ref:`VariationalQuantumGate_Y<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___y>`;
	class :ref:`VariationalQuantumGate_Y1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___y1>`;
	class :ref:`VariationalQuantumGate_Z<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z>`;
	class :ref:`VariationalQuantumGate_Z1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1>`;
.. _details-class_q_panda_1_1_variational_1_1_variational_quantum_gate:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Construction
------------

.. index:: pair: function; VariationalQuantumGate
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a44eadb3fe9594c0cc691c2d1b06cd658:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariationalQuantumGate(const VariationalQuantumGate&)

Copy Constructor for a new :ref:`Variational <doxid-namespace_q_panda_1_1_variational>` Quantum Gate object.

.. index:: pair: function; VariationalQuantumGate
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a2a29b7083325db10b62755ae610d2a35:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	VariationalQuantumGate()

Default Constructor for a new :ref:`Variational <doxid-namespace_q_panda_1_1_variational>` Quantum Gate object.

Methods
-------

.. index:: pair: function; n_var
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a94e84e5572d19b6f4017e15671cc8fc1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t n_var()



.. rubric:: Returns:

size_t the number of vars.

.. index:: pair: function; get_vars
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a040e35879202ce657c995466e9a64e04:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& get_vars()

Get all variables for the VQG.



.. rubric:: Returns:

std::vector<Variable>

.. index:: pair: function; var_pos
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a289faed2739b91d54ea82d7a72aa4beb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int var_pos(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` _var)

Get the position for var in the m_vars. If not existed, return -1. Otherwise, return the position n, which is var == m_vars[n].



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- var

		- The corresponding variable.



.. rubric:: Returns:

int -1 if not existed, or position.

.. index:: pair: function; feed
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1ad331ff4076e3ad2e6108ebb270dc4947:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` feed() = 0

Interface to instantialize the :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` with VQG.



.. rubric:: Returns:

:ref:`QGate <doxid-class_q_panda_1_1_q_gate>` Instantiation

.. index:: pair: function; feed
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1af174cd439585ec3b29f4b1360d3ecd90:

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
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aa135247611e3a0f49af4a15734f3505f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<VariationalQuantumGate> copy() = 0

Interface to copy the instance, and return a shared_ptr for the object.



.. rubric:: Returns:

std::shared_ptr<VariationalQuantumGate>

