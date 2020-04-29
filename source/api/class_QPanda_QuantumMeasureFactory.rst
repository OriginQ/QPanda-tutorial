.. index:: pair: class; QPanda::QuantumMeasureFactory
.. _doxid-class_q_panda_1_1_quantum_measure_factory:

class QPanda::QuantumMeasureFactory
===================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`AbstractQuantumMeasure <doxid-class_q_panda_1_1_abstract_quantum_measure>`. :ref:`More...<details-class_q_panda_1_1_quantum_measure_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMeasure.h>
	
	class QuantumMeasureFactory
	{
	public:
		// methods
	
		void :target:`registClass<doxid-class_q_panda_1_1_quantum_measure_factory_1a1ebeb3f6bccc49853edd201f5725fdc1>`(
			std::string name,
			:ref:`CreateMeasure<doxid-namespace_q_panda_1aaa3162dce15c83be0503e264ff0059dd>` method
			);
	
		:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`* :target:`getQuantumMeasure<doxid-class_q_panda_1_1_quantum_measure_factory_1a074b97180a64307257daba30270a1560>`(
			std::string&,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*,
			:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*
			);
	
		static QuantumMeasureFactory& :ref:`getInstance<doxid-class_q_panda_1_1_quantum_measure_factory_1aa1f2959fe64143b9b03060fe000d4ff9>`();
	};
.. _details-class_q_panda_1_1_quantum_measure_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`AbstractQuantumMeasure <doxid-class_q_panda_1_1_abstract_quantum_measure>`.

Methods
-------

.. index:: pair: function; getInstance
.. _doxid-class_q_panda_1_1_quantum_measure_factory_1aa1f2959fe64143b9b03060fe000d4ff9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QuantumMeasureFactory& getInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QuantumMeasureFactory <doxid-class_q_panda_1_1_quantum_measure_factory>` &

