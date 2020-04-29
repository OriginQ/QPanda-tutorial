.. index:: pair: class; QPanda::AbstractQGateNode
.. _doxid-class_q_panda_1_1_abstract_q_gate_node:

class QPanda::AbstractQGateNode
===============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum gate basic abstract class. :ref:`More...<details-class_q_panda_1_1_abstract_q_gate_node>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QGate.h>
	
	class AbstractQGateNode
	{
	public:
		// methods
	
		virtual size_t :ref:`getQuBitVector<doxid-class_q_panda_1_1_abstract_q_gate_node_1a0e536c808361e0243bffcdb949f5cc46>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`popBackQuBit<doxid-class_q_panda_1_1_abstract_q_gate_node_1a16a32117dd9d453c5219bac6a4223aee>`() = 0;
		virtual void :ref:`PushBackQuBit<doxid-class_q_panda_1_1_abstract_q_gate_node_1a6eff60e20adc05b09f142506716b11a4>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0;
		virtual size_t :ref:`getTargetQubitNum<doxid-class_q_panda_1_1_abstract_q_gate_node_1aba498aceb9db852cf5f52febf01c67c1>`() const = 0;
		virtual size_t :ref:`getControlQubitNum<doxid-class_q_panda_1_1_abstract_q_gate_node_1a5f01c3abe784f28ab97f1bf7c9846be0>`() const = 0;
		virtual :ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* :ref:`getQGate<doxid-class_q_panda_1_1_abstract_q_gate_node_1afdc702d1ca93eb404b532fac032bd61d>`() const = 0;
		virtual void :ref:`setQGate<doxid-class_q_panda_1_1_abstract_q_gate_node_1af754b29a705224c2b8569594bb59c35d>`(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*) = 0;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_abstract_q_gate_node_1a741d55580cfb5d2597bd25f3236819a8>`() const = 0;
		virtual size_t :ref:`getControlVector<doxid-class_q_panda_1_1_abstract_q_gate_node_1ac82c51d31b345c36c0ce5edf2a8411b7>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0;
		virtual bool :ref:`setDagger<doxid-class_q_panda_1_1_abstract_q_gate_node_1ae930a57233bd67928e5c8abfcd6b1835>`(bool) = 0;
		virtual bool :ref:`setControl<doxid-class_q_panda_1_1_abstract_q_gate_node_1aff311eda65e1ce1105cf54aa10cf8650>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0;
	};

	// direct descendants

	class :ref:`OriginQGate<doxid-class_q_panda_1_1_origin_q_gate>`;
	class :ref:`QGate<doxid-class_q_panda_1_1_q_gate>`;
.. _details-class_q_panda_1_1_abstract_q_gate_node:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum gate basic abstract class.

Methods
-------

.. index:: pair: function; getQuBitVector
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1a0e536c808361e0243bffcdb949f5cc46:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getQuBitVector(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0

Get qubit vector inside this quantum gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubit vector



.. rubric:: Returns:

size_t



.. rubric:: See also:

:ref:`GateType <doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`

.. index:: pair: function; popBackQuBit
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1a16a32117dd9d453c5219bac6a4223aee:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* popBackQuBit() = 0

erase qubit vector element at end



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; PushBackQuBit
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1a6eff60e20adc05b09f142506716b11a4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void PushBackQuBit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*) = 0

insert qubit vector element at end



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` pointer

.. index:: pair: function; getTargetQubitNum
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1aba498aceb9db852cf5f52febf01c67c1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getTargetQubitNum() const = 0

Get target qubit num inside this quantum gate.



.. rubric:: Returns:

size_t qubit num

.. index:: pair: function; getControlQubitNum
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1a5f01c3abe784f28ab97f1bf7c9846be0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getControlQubitNum() const = 0

Get control qubit num inside this quantum gate.



.. rubric:: Returns:

size_t qubit num

.. index:: pair: function; getQGate
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1afdc702d1ca93eb404b532fac032bd61d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* getQGate() const = 0

Get Quantum Gate.



.. rubric:: Returns:

QuantumGate \*

.. index:: pair: function; setQGate
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1af754b29a705224c2b8569594bb59c35d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setQGate(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*) = 0

Set Quantum Gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QuantumGate\*

		- QuantumGate pointer

.. index:: pair: function; isDagger
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1a741d55580cfb5d2597bd25f3236819a8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool isDagger() const = 0

Judge current quantum gate is dagger.



.. rubric:: Returns:

bool

.. index:: pair: function; getControlVector
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1ac82c51d31b345c36c0ce5edf2a8411b7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getControlVector(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0

Get control vector fron current quantum gate node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubits vector



.. rubric:: Returns:

size_t



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; setDagger
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1ae930a57233bd67928e5c8abfcd6b1835:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool setDagger(bool) = 0

Set dagger to current quantum gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- is dagger



.. rubric:: Returns:

bool

.. index:: pair: function; setControl
.. _doxid-class_q_panda_1_1_abstract_q_gate_node_1aff311eda65e1ce1105cf54aa10cf8650:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool setControl(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0

Set control qubits to current quantum gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- control qubits vector



.. rubric:: Returns:

bool



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

