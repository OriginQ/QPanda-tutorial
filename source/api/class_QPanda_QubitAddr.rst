.. index:: pair: class; QPanda::QubitAddr
.. _doxid-class_q_panda_1_1_qubit_addr:

class QPanda::QubitAddr
=======================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMachineInterface.h>
	
	class QubitAddr
	{
	public:
		// construction
	
		:target:`QubitAddr<doxid-class_q_panda_1_1_qubit_addr_1a88751ce51cd1ab924d5c6fad4ef31547>`(
			int ix,
			int iy
			);
	
		:target:`QubitAddr<doxid-class_q_panda_1_1_qubit_addr_1a936b9eb93a70f022d02e5f379be4de1d>`();

		// methods
	
		virtual int :target:`getX<doxid-class_q_panda_1_1_qubit_addr_1a99c4f99f24645fb919f29ac2f1a82643>`() const;
		virtual int :target:`getY<doxid-class_q_panda_1_1_qubit_addr_1a4489171f1635720ad0b49c66f9a3359c>`() const;
		virtual void :target:`setX<doxid-class_q_panda_1_1_qubit_addr_1ae1d5e4b53a8f0e2b09c2f079cafd2da1>`(int x);
		virtual void :target:`setY<doxid-class_q_panda_1_1_qubit_addr_1a39ef499ea32cd1fea1c2e8900882c75d>`(int y);
	};
