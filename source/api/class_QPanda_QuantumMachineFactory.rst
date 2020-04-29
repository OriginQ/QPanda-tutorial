.. index:: pair: class; QPanda::QuantumMachineFactory
.. _doxid-class_q_panda_1_1_quantum_machine_factory:

class QPanda::QuantumMachineFactory
===================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`QuantumMachine <doxid-class_q_panda_1_1_quantum_machine>`. :ref:`More...<details-class_q_panda_1_1_quantum_machine_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMachineFactory.h>
	
	class QuantumMachineFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*()> :target:`constructor_t<doxid-class_q_panda_1_1_quantum_machine_factory_1acbc73d632b02f72136a5a5eaf29276ad>`;
		typedef std::map<std::string, :ref:`constructor_t<doxid-class_q_panda_1_1_quantum_machine_factory_1acbc73d632b02f72136a5a5eaf29276ad>`> :target:`constructor_map_t<doxid-class_q_panda_1_1_quantum_machine_factory_1af8c0dfb6bf8854e042351779c242a8aa>`;

		// fields
	
		:ref:`constructor_map_t<doxid-class_q_panda_1_1_quantum_machine_factory_1af8c0dfb6bf8854e042351779c242a8aa>` :target:`_Quantum_Machine_Constructor<doxid-class_q_panda_1_1_quantum_machine_factory_1ae6ecba2fb5cca702c1792ee6d0f91c1d>`;

		// methods
	
		static QuantumMachineFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_quantum_machine_factory_1a1378d539ddfa3f9c4ef8c85a6bb5861c>`();
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* :target:`CreateByName<doxid-class_q_panda_1_1_quantum_machine_factory_1a0d7c100856f51a8106d5c66d1d686eff>`(std::string);
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* :target:`CreateByType<doxid-class_q_panda_1_1_quantum_machine_factory_1aae9a49ecd490041a9294756d9a569c95>`(:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` class_type);
	
		void :target:`registerclass<doxid-class_q_panda_1_1_quantum_machine_factory_1a446caf20fe2721ebe9cc0156ec516ed5>`(
			std::string,
			:ref:`constructor_t<doxid-class_q_panda_1_1_quantum_machine_factory_1acbc73d632b02f72136a5a5eaf29276ad>` constructor
			);
	};
.. _details-class_q_panda_1_1_quantum_machine_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`QuantumMachine <doxid-class_q_panda_1_1_quantum_machine>`.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_quantum_machine_factory_1a1378d539ddfa3f9c4ef8c85a6bb5861c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QuantumMachineFactory& GetFactoryInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QuantumMachineFactory <doxid-class_q_panda_1_1_quantum_machine_factory>` &

