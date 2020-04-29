.. index:: pair: class; QPanda::AbstractQuantumMeasure
.. _doxid-class_q_panda_1_1_abstract_quantum_measure:

class QPanda::AbstractQuantumMeasure
====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum Measure basic abstract class. :ref:`More...<details-class_q_panda_1_1_abstract_quantum_measure>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMeasure.h>
	
	class AbstractQuantumMeasure
	{
	public:
		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_abstract_quantum_measure_1ae377dd6d809e3c4c97fa6ec1fab23513>`() const = 0;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_abstract_quantum_measure_1ab08d02223fc2440ff809ff277857f74b>`() const = 0;
	};

	// direct descendants

	class :ref:`OriginMeasure<doxid-class_q_panda_1_1_origin_measure>`;
	class :ref:`QMeasure<doxid-class_q_panda_1_1_q_measure>`;
.. _details-class_q_panda_1_1_abstract_quantum_measure:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum Measure basic abstract class.

Methods
-------

.. index:: pair: function; getQuBit
.. _doxid-class_q_panda_1_1_abstract_quantum_measure_1ae377dd6d809e3c4c97fa6ec1fab23513:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* getQuBit() const = 0

Get measure node qubit address.



.. rubric:: Returns:

:ref:`Qubit <doxid-class_q_panda_1_1_qubit>` \*

.. index:: pair: function; getCBit
.. _doxid-class_q_panda_1_1_abstract_quantum_measure_1ab08d02223fc2440ff809ff277857f74b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* getCBit() const = 0

Get measure node cbit address.



.. rubric:: Returns:

:ref:`CBit <doxid-class_q_panda_1_1_c_bit>` \*

