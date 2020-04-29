.. index:: pair: class; QPanda::QCircuitParam
.. _doxid-class_q_panda_1_1_q_circuit_param:

class QPanda::QCircuitParam
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Circuit Parameter information. :ref:`More...<details-class_q_panda_1_1_q_circuit_param>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitInfo.h>
	
	class QCircuitParam
	{
	public:
		// fields
	
		bool :ref:`m_is_dagger<doxid-class_q_panda_1_1_q_circuit_param_1a5b815041da10bbf9cd84dd9888aa486c>`;
		std::vector<:ref:`QPanda::Qubit<doxid-class_q_panda_1_1_qubit>`*> :ref:`m_control_qubits<doxid-class_q_panda_1_1_q_circuit_param_1a04fbad0c2f4083190783e263b1cafa94>`;

		// construction
	
		:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param_1a725c15808ec6e629c7b884c032feca35>`();
		:ref:`QCircuitParam<doxid-class_q_panda_1_1_q_circuit_param_1a1f8261e3c407793ad57edab243534314>`(const QCircuitParam& rhs);

		// methods
	
		std::shared_ptr<QCircuitParam> :ref:`clone<doxid-class_q_panda_1_1_q_circuit_param_1a610bc95562c27a0a5e53aeca3c4605a0>`();
		void :ref:`append_control_qubits<doxid-class_q_panda_1_1_q_circuit_param_1ae6c97a2064895b2602ad64ed05436b1d>`(const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& ctrl_qubits);
		static :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`get_real_append_qubits<doxid-class_q_panda_1_1_q_circuit_param_1a71fe32cc5e7f1342dee18f887bda4dcd>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` append_qubits, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` target_qubits);
	};
.. _details-class_q_panda_1_1_q_circuit_param:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Circuit Parameter information.

Fields
------

.. index:: pair: variable; m_is_dagger
.. _doxid-class_q_panda_1_1_q_circuit_param_1a5b815041da10bbf9cd84dd9888aa486c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool m_is_dagger

dagger information

.. index:: pair: variable; m_control_qubits
.. _doxid-class_q_panda_1_1_q_circuit_param_1a04fbad0c2f4083190783e263b1cafa94:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`QPanda::Qubit<doxid-class_q_panda_1_1_qubit>`*> m_control_qubits

control Quantum bits

Construction
------------

.. index:: pair: function; QCircuitParam
.. _doxid-class_q_panda_1_1_q_circuit_param_1a725c15808ec6e629c7b884c032feca35:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QCircuitParam()

Constructor of :ref:`QCircuitParam <doxid-class_q_panda_1_1_q_circuit_param>`.

.. index:: pair: function; QCircuitParam
.. _doxid-class_q_panda_1_1_q_circuit_param_1a1f8261e3c407793ad57edab243534314:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QCircuitParam(const QCircuitParam& rhs)

copy constructor

Methods
-------

.. index:: pair: function; clone
.. _doxid-class_q_panda_1_1_q_circuit_param_1a610bc95562c27a0a5e53aeca3c4605a0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<QCircuitParam> clone()

clone

.. index:: pair: function; append_control_qubits
.. _doxid-class_q_panda_1_1_q_circuit_param_1ae6c97a2064895b2602ad64ed05436b1d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void append_control_qubits(const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& ctrl_qubits)

append control qubits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- control qubits

.. index:: pair: function; get_real_append_qubits
.. _doxid-class_q_panda_1_1_q_circuit_param_1a71fe32cc5e7f1342dee18f887bda4dcd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` get_real_append_qubits(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` append_qubits, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>` target_qubits)

get the real increased control qubits



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- increased control qubits, maybe some repeat exist

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- already controled qubits



.. rubric:: Returns:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>` the real increased control qubits

