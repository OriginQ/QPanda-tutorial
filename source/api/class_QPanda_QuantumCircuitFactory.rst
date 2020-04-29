.. index:: pair: class; QPanda::QuantumCircuitFactory
.. _doxid-class_q_panda_1_1_quantum_circuit_factory:

class QPanda::QuantumCircuitFactory
===================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`AbstractQuantumCircuit <doxid-class_q_panda_1_1_abstract_quantum_circuit>`. :ref:`More...<details-class_q_panda_1_1_quantum_circuit_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuit.h>
	
	class QuantumCircuitFactory
	{
	public:
		// methods
	
		void :target:`registClass<doxid-class_q_panda_1_1_quantum_circuit_factory_1a3feaa239e5584d4db82e2a85251bc935>`(
			std::string name,
			:ref:`CreateQCircuit<doxid-namespace_q_panda_1ab8c010d113d8febb212ee484acb321a3>` method
			);
	
		:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`* :target:`getQuantumCircuit<doxid-class_q_panda_1_1_quantum_circuit_factory_1a38f609459e2b4ad10d18ecbe072979df>`(std::string&);
		static QuantumCircuitFactory& :ref:`getInstance<doxid-class_q_panda_1_1_quantum_circuit_factory_1a8fc6c6386b5527af0e9410890349c1d8>`();
	};
.. _details-class_q_panda_1_1_quantum_circuit_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`AbstractQuantumCircuit <doxid-class_q_panda_1_1_abstract_quantum_circuit>`.

Methods
-------

.. index:: pair: function; getInstance
.. _doxid-class_q_panda_1_1_quantum_circuit_factory_1a8fc6c6386b5527af0e9410890349c1d8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QuantumCircuitFactory& getInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QuantumCircuitFactory <doxid-class_q_panda_1_1_quantum_circuit_factory>` &

