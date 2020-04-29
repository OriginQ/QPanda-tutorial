.. index:: pair: class; QPanda::OriginQMachineStatus
.. _doxid-class_q_panda_1_1_origin_q_machine_status:

class QPanda::OriginQMachineStatus
==================================

.. toctree::
	:hidden:

Implementation class of :ref:`QMachineStatus <doxid-class_q_panda_1_1_q_machine_status>`.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginQMachineStatus: public :ref:`QPanda::QMachineStatus<doxid-class_q_panda_1_1_q_machine_status>`
	{
	public:
		// methods
	
		virtual int :target:`getStatusCode<doxid-class_q_panda_1_1_origin_q_machine_status_1ae7d0f20fcbb073ad190b28cef6c56f96>`() const;
		virtual void :target:`setStatusCode<doxid-class_q_panda_1_1_origin_q_machine_status_1a3f930c6dc481ec376f16021be835790e>`(int miStatus);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual int :ref:`getStatusCode<doxid-class_q_panda_1_1_q_machine_status_1a4bbdd6c20d191dcf612a98db20926429>`() const = 0;
		virtual void :ref:`setStatusCode<doxid-class_q_panda_1_1_q_machine_status_1af8bf1610a52c92188705b1155c3d1d50>`(int) = 0;

