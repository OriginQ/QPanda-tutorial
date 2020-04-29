.. index:: pair: class; QPanda::QuantumProgramFactory
.. _doxid-class_q_panda_1_1_quantum_program_factory:

class QPanda::QuantumProgramFactory
===================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`AbstractQuantumProgram <doxid-class_q_panda_1_1_abstract_quantum_program>`. :ref:`More...<details-class_q_panda_1_1_quantum_program_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgram.h>
	
	class QuantumProgramFactory
	{
	public:
		// methods
	
		void :target:`registClass<doxid-class_q_panda_1_1_quantum_program_factory_1ac11ad7e6ec7827e9cf4edb5ff7cef00f>`(
			std::string name,
			:ref:`CreateQProgram<doxid-namespace_q_panda_1a56c39ff2ef01b4b9bc43db917c14936f>` method
			);
	
		:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`* :target:`getQuantumQProg<doxid-class_q_panda_1_1_quantum_program_factory_1a5fe431da6f3b6036306df862b22476d2>`(std::string&);
		static QuantumProgramFactory& :ref:`getInstance<doxid-class_q_panda_1_1_quantum_program_factory_1a6da1210b8c9c8684849f2a52ac9f4869>`();
	};
.. _details-class_q_panda_1_1_quantum_program_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`AbstractQuantumProgram <doxid-class_q_panda_1_1_abstract_quantum_program>`.

Methods
-------

.. index:: pair: function; getInstance
.. _doxid-class_q_panda_1_1_quantum_program_factory_1a6da1210b8c9c8684849f2a52ac9f4869:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QuantumProgramFactory& getInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QuantumProgramFactory <doxid-class_q_panda_1_1_quantum_program_factory>` &

