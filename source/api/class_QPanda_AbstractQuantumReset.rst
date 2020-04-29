.. index:: pair: class; QPanda::AbstractQuantumReset
.. _doxid-class_q_panda_1_1_abstract_quantum_reset:

class QPanda::AbstractQuantumReset
==================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum Reset basic abstract class. :ref:`More...<details-class_q_panda_1_1_abstract_quantum_reset>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QReset.h>
	
	class AbstractQuantumReset
	{
	public:
		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_abstract_quantum_reset_1a60c3a60eff08e2cfeba20c3662cdb4cb>`() const = 0;
	};

	// direct descendants

	class :ref:`OriginReset<doxid-class_q_panda_1_1_origin_reset>`;
	class :ref:`QReset<doxid-class_q_panda_1_1_q_reset>`;
.. _details-class_q_panda_1_1_abstract_quantum_reset:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum Reset basic abstract class.

Methods
-------

.. index:: pair: function; getQuBit
.. _doxid-class_q_panda_1_1_abstract_quantum_reset_1a60c3a60eff08e2cfeba20c3662cdb4cb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* getQuBit() const = 0

Get the reset qubit.



.. rubric:: Returns:

:ref:`Qubit <doxid-class_q_panda_1_1_qubit>` \*

