.. index:: pair: class; QPanda::QGate
.. _doxid-class_q_panda_1_1_q_gate:

class QPanda::QGate
===================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QPanda2 quantum gate basic classs. :ref:`More...<details-class_q_panda_1_1_q_gate>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QGate.h>
	
	class QGate: public :ref:`QPanda::AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`
	{
	public:
		// construction
	
		:target:`QGate<doxid-class_q_panda_1_1_q_gate_1a17f0d4de8360c3af491ce9778ac35144>`(const QGate&);
	
		:target:`QGate<doxid-class_q_panda_1_1_q_gate_1a142b50e4f701ad89cc7b650f7e2f0fd0>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&,
			:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*
			);
	
		:target:`QGate<doxid-class_q_panda_1_1_q_gate_1aa8072130142e1598737883896bd08479>`(std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> node);

		// methods
	
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_gate_1a29ad4ab9dcadcd7f475001fd9a0556b8>`() const;
		virtual size_t :ref:`getQuBitVector<doxid-class_q_panda_1_1_q_gate_1af8b38e520fdfa4b7d7cb930a40040c18>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const;
		virtual size_t :ref:`getTargetQubitNum<doxid-class_q_panda_1_1_q_gate_1a81a7ed8b3bf6e3caf0699963589b6ad4>`() const;
		virtual size_t :ref:`getControlQubitNum<doxid-class_q_panda_1_1_q_gate_1a815b77d108038bf9ffc190c6742a21ff>`() const;
		virtual :ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* :ref:`getQGate<doxid-class_q_panda_1_1_q_gate_1a981f821f17af5aafaad2b8fe0bb7bf17>`() const;
		virtual bool :ref:`setDagger<doxid-class_q_panda_1_1_q_gate_1a352e65d95899b339f427cc79913e311d>`(bool);
		virtual bool :ref:`setControl<doxid-class_q_panda_1_1_q_gate_1aaf82a6a76dd24f00cab894b47075643e>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);
		std::shared_ptr<:ref:`AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_q_gate_1af2ffa323b23339b414f35218dd28d9bf>`();
		QGate :ref:`dagger<doxid-class_q_panda_1_1_q_gate_1a3880ada6470a3f75537075ad628c5d0b>`();
		QGate :ref:`control<doxid-class_q_panda_1_1_q_gate_1aa63bc39be9ea5afe47a8e029b23a6f9b>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_q_gate_1a4f73af1d279083a0096122377db8c3c8>`() const;
		virtual size_t :ref:`getControlVector<doxid-class_q_panda_1_1_q_gate_1a5938d3c01939b1700fd424e577bf202a>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

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

.. _details-class_q_panda_1_1_q_gate:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPanda2 quantum gate basic classs.

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_q_gate_1a29ad4ab9dcadcd7f475001fd9a0556b8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; getQuBitVector
.. _doxid-class_q_panda_1_1_q_gate_1af8b38e520fdfa4b7d7cb930a40040c18:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getQuBitVector(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const

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

.. index:: pair: function; getTargetQubitNum
.. _doxid-class_q_panda_1_1_q_gate_1a81a7ed8b3bf6e3caf0699963589b6ad4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getTargetQubitNum() const

Get qubit num inside this quantum gate.



.. rubric:: Returns:

size_t qubit num

.. index:: pair: function; getControlQubitNum
.. _doxid-class_q_panda_1_1_q_gate_1a815b77d108038bf9ffc190c6742a21ff:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getControlQubitNum() const

Get control qubit num inside this quantum gate.



.. rubric:: Returns:

size_t qubit num

.. index:: pair: function; getQGate
.. _doxid-class_q_panda_1_1_q_gate_1a981f821f17af5aafaad2b8fe0bb7bf17:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* getQGate() const

Get Quantum Gate.



.. rubric:: Returns:

QuantumGate \*

.. index:: pair: function; setDagger
.. _doxid-class_q_panda_1_1_q_gate_1a352e65d95899b339f427cc79913e311d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool setDagger(bool)

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
.. _doxid-class_q_panda_1_1_q_gate_1aaf82a6a76dd24f00cab894b47075643e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool setControl(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`)

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

.. index:: pair: function; dagger
.. _doxid-class_q_panda_1_1_q_gate_1a3880ada6470a3f75537075ad628c5d0b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QGate dagger()

Get a dagger quantumgate base on current quantum gate node.



.. rubric:: Returns:

:ref:`QPanda::QGate <doxid-class_q_panda_1_1_q_gate>` quantum gate

.. index:: pair: function; control
.. _doxid-class_q_panda_1_1_q_gate_1aa63bc39be9ea5afe47a8e029b23a6f9b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QGate control(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`)

Get a control quantumgate base on current quantum gate node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- control qubits vector



.. rubric:: Returns:

:ref:`QPanda::QGate <doxid-class_q_panda_1_1_q_gate>` quantum gate



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; isDagger
.. _doxid-class_q_panda_1_1_q_gate_1a4f73af1d279083a0096122377db8c3c8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool isDagger() const

Judge current quantum gate is dagger.



.. rubric:: Returns:

bool

.. index:: pair: function; getControlVector
.. _doxid-class_q_panda_1_1_q_gate_1a5938d3c01939b1700fd424e577bf202a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getControlVector(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const

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

