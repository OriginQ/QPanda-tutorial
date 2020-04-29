.. index:: pair: class; QPanda::QMeasure
.. _doxid-class_q_panda_1_1_q_measure:

class QPanda::QMeasure
======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum Measure basic class. :ref:`More...<details-class_q_panda_1_1_q_measure>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMeasure.h>
	
	class QMeasure: public :ref:`QPanda::AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`
	{
	public:
		// construction
	
		:target:`QMeasure<doxid-class_q_panda_1_1_q_measure_1ac37cd436e2e77af1df160a27df86cb56>`(const QMeasure&);
	
		:target:`QMeasure<doxid-class_q_panda_1_1_q_measure_1a4ec7b4279512df4c333805055caca75f>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*,
			:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*
			);
	
		:target:`QMeasure<doxid-class_q_panda_1_1_q_measure_1abc9fce64dfa78faeff136ec5a32875f3>`(std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> node);

		// methods
	
		std::shared_ptr<:ref:`AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_q_measure_1a6f2237a49dda5be403e392b62105b39d>`();
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_q_measure_1ada87818e060192810cfcefd907ea6764>`() const;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_q_measure_1a325c38fc46e243d082b6341f52e86728>`() const;
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :target:`getNodeType<doxid-class_q_panda_1_1_q_measure_1a51b981ad7da7d9899473430abba888e0>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_abstract_quantum_measure_1ae377dd6d809e3c4c97fa6ec1fab23513>`() const = 0;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_abstract_quantum_measure_1ab08d02223fc2440ff809ff277857f74b>`() const = 0;

.. _details-class_q_panda_1_1_q_measure:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum Measure basic class.

Methods
-------

.. index:: pair: function; getQuBit
.. _doxid-class_q_panda_1_1_q_measure_1ada87818e060192810cfcefd907ea6764:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* getQuBit() const

Get measure node qubit address.



.. rubric:: Returns:

:ref:`Qubit <doxid-class_q_panda_1_1_qubit>` \*

.. index:: pair: function; getCBit
.. _doxid-class_q_panda_1_1_q_measure_1a325c38fc46e243d082b6341f52e86728:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* getCBit() const

Get measure node cbit address.



.. rubric:: Returns:

:ref:`CBit <doxid-class_q_panda_1_1_c_bit>` \*

