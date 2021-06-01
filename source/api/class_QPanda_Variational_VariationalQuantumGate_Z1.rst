.. index:: pair: class; QPanda::Variational::VariationalQuantumGate_Z1
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1:

class QPanda::Variational::VariationalQuantumGate_Z1
====================================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	class VariationalQuantumGate_Z1: public :ref:`QPanda::Variational::VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`
	{
	public:
		// construction
	
		:target:`VariationalQuantumGate_Z1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1a7d4165dbb01bdf498cabbba46a473172>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* q);
		:target:`VariationalQuantumGate_Z1<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1aea9f4d529b7e9b6a82b0dd6bce6cd099>`(const VariationalQuantumGate_Z1& gate);

		// methods
	
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1ad586c2043e0adfc277c915907095a43c>`();
		virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> :ref:`copy<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1a480b978b9fa1276106ae6d6327daedc6>`();
		VariationalQuantumGate_Z1 :target:`dagger<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1a83545998f05917a96f101db3f451728e>`();
		VariationalQuantumGate_Z1 :target:`control<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1afc4cfaaa2a88521d3469964e5390cd6e>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` qv);
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

.. _details-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; feed
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1ad586c2043e0adfc277c915907095a43c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` feed()

Interface to instantialize the :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` with VQG.



.. rubric:: Returns:

:ref:`QGate <doxid-class_q_panda_1_1_q_gate>` Instantiation

.. index:: pair: function; copy
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___z1_1a480b978b9fa1276106ae6d6327daedc6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> copy()

Interface to copy the instance, and return a shared_ptr for the object.



.. rubric:: Returns:

std::shared_ptr<VariationalQuantumGate>

