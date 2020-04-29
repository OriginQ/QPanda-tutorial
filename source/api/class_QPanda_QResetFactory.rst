.. index:: pair: class; QPanda::QResetFactory
.. _doxid-class_q_panda_1_1_q_reset_factory:

class QPanda::QResetFactory
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`AbstractQuantumReset <doxid-class_q_panda_1_1_abstract_quantum_reset>`. :ref:`More...<details-class_q_panda_1_1_q_reset_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QReset.h>
	
	class QResetFactory
	{
	public:
		// methods
	
		void :target:`registClass<doxid-class_q_panda_1_1_q_reset_factory_1a5985ad01dd23d2dba9c724c5e73201e5>`(
			std::string name,
			:ref:`CreateReset<doxid-namespace_q_panda_1a1baefdbe7a211e28b9f569e7a097352a>` method
			);
	
		:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`* :target:`getQuantumReset<doxid-class_q_panda_1_1_q_reset_factory_1a284972ee65725f67a5dd3c29504a3afd>`(
			std::string&,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*
			);
	
		static QResetFactory& :ref:`getInstance<doxid-class_q_panda_1_1_q_reset_factory_1a5dea64486138cfc7860460d7a5dec1d8>`();
	};
.. _details-class_q_panda_1_1_q_reset_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`AbstractQuantumReset <doxid-class_q_panda_1_1_abstract_quantum_reset>`.

Methods
-------

.. index:: pair: function; getInstance
.. _doxid-class_q_panda_1_1_q_reset_factory_1a5dea64486138cfc7860460d7a5dec1d8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QResetFactory& getInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QResetFactory <doxid-class_q_panda_1_1_q_reset_factory>` &

