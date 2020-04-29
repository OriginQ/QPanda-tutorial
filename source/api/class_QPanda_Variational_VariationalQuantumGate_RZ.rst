.. index:: pair: class; QPanda::Variational::VariationalQuantumGate_RZ
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z:

class QPanda::Variational::VariationalQuantumGate_RZ
====================================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	class VariationalQuantumGate_RZ: public :ref:`QPanda::Variational::VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`
	{
	public:
		// construction
	
		:target:`VariationalQuantumGate_RZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1a46646e68e1b475ad638941bca99e5ec8>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*,
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`
			);
	
		:target:`VariationalQuantumGate_RZ<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1a438d8810bfa8f6e39614803f9d99c6b7>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*,
			double angle
			);

		// methods
	
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1ac2d0e051925776fd1bd447e7bd771ad5>`() const;
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1a52e385399f78dcd97ade22b0bf9916ba>`(std::map<size_t, double> offset) const;
		virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> :ref:`copy<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1a52e995f5cf4a579ae03207776c596219>`();
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
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a965a0c45df612b9df05f6e2140a361d3>`() const = 0;
		virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` :ref:`feed<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1a6fa99388fac051437c395003cc02160d>`(std::map<size_t, double> offset) const;
		virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> :ref:`copy<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate_1aa135247611e3a0f49af4a15734f3505f>`() = 0;

.. _details-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; feed
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1ac2d0e051925776fd1bd447e7bd771ad5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` feed() const

Interface to instantialize the :ref:`QGate <doxid-class_q_panda_1_1_q_gate>` with VQG.



.. rubric:: Returns:

:ref:`QGate <doxid-class_q_panda_1_1_q_gate>` Instantiation

.. index:: pair: function; feed
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1a52e385399f78dcd97ade22b0bf9916ba:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QGate<doxid-class_q_panda_1_1_q_gate>` feed(std::map<size_t, double> offset) const

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
.. _doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate___r_z_1a52e995f5cf4a579ae03207776c596219:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`VariationalQuantumGate<doxid-class_q_panda_1_1_variational_1_1_variational_quantum_gate>`> copy()

Interface to copy the instance, and return a shared_ptr for the object.



.. rubric:: Returns:

std::shared_ptr<VariationalQuantumGate>

