.. index:: pair: class; QPanda::QProgClockCycle
.. _doxid-class_q_panda_1_1_q_prog_clock_cycle:

class QPanda::QProgClockCycle
=============================

.. toctree::
	:hidden:

Count Quantum Program clock cycle.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgClockCycle.h>
	
	class QProgClockCycle
	{
	public:
		// construction
	
		:target:`QProgClockCycle<doxid-class_q_panda_1_1_q_prog_clock_cycle_1a5ef1225d2eaf3fe97cf79e974c426123>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);

		// methods
	
		size_t :target:`count<doxid-class_q_panda_1_1_q_prog_clock_cycle_1a33d20fb6fdb2610dc2cf16d0b1631754>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			bool optimize = false
			);
	};
