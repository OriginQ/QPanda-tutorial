.. index:: pair: class; QPanda::OriginQGate
.. _doxid-class_q_panda_1_1_origin_q_gate:

class QPanda::OriginQGate
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QGate <doxid-class_q_panda_1_1_q_gate>`. :ref:`More...<details-class_q_panda_1_1_origin_q_gate>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QGate.h>
	
	class OriginQGate:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractQGateNode<doxid-class_q_panda_1_1_abstract_q_gate_node>`
	{
	public:
		// construction
	
		:target:`OriginQGate<doxid-class_q_panda_1_1_origin_q_gate_1a6bdd4074354f640ec28689997633e7b8>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&,
			:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*
			);

		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_q_gate_1a289a189f32d4fc2f3b39f60f43ed9ef4>`() const;
		virtual size_t :ref:`getQuBitVector<doxid-class_q_panda_1_1_origin_q_gate_1abd21f4492afe40943fd216b911658c3f>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const;
		virtual size_t :ref:`getTargetQubitNum<doxid-class_q_panda_1_1_origin_q_gate_1afb97fe04738cf235ca585a4c151c2f00>`() const;
		virtual size_t :ref:`getControlQubitNum<doxid-class_q_panda_1_1_origin_q_gate_1a8425692d5f3b68f37e3c59f0d258099a>`() const;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`popBackQuBit<doxid-class_q_panda_1_1_origin_q_gate_1a1b3a19e040e57af230b251e77fce0b2a>`();
		virtual :ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* :ref:`getQGate<doxid-class_q_panda_1_1_origin_q_gate_1a86a84d652e3bc4259db0ccbd6ab82f77>`() const;
		virtual void :ref:`setQGate<doxid-class_q_panda_1_1_origin_q_gate_1a56c6c33f9aa4f6e7117617c0569175c5>`(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*);
		virtual bool :ref:`setDagger<doxid-class_q_panda_1_1_origin_q_gate_1a92e412a3fe47a10b001dbd8cc4f15346>`(bool);
		virtual bool :ref:`setControl<doxid-class_q_panda_1_1_origin_q_gate_1a252fb142c39d234bed82332ce13b1c46>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_origin_q_gate_1ac2f8642b4fafff5c9789319673d2a1d4>`() const;
		virtual size_t :ref:`getControlVector<doxid-class_q_panda_1_1_origin_q_gate_1a3a3c35274292c34bc7fb74ac7be21aa1>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const;
		virtual void :ref:`PushBackQuBit<doxid-class_q_panda_1_1_origin_q_gate_1ab2b18fc595acbe9c64a365cf6ac957c4>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
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

.. _details-class_q_panda_1_1_origin_q_gate:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QGate <doxid-class_q_panda_1_1_q_gate>`.

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_q_gate_1a289a189f32d4fc2f3b39f60f43ed9ef4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; getQuBitVector
.. _doxid-class_q_panda_1_1_origin_q_gate_1abd21f4492afe40943fd216b911658c3f:

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
.. _doxid-class_q_panda_1_1_origin_q_gate_1afb97fe04738cf235ca585a4c151c2f00:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getTargetQubitNum() const

Get target qubit num inside this quantum gate.



.. rubric:: Returns:

size_t qubit num

.. index:: pair: function; getControlQubitNum
.. _doxid-class_q_panda_1_1_origin_q_gate_1a8425692d5f3b68f37e3c59f0d258099a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t getControlQubitNum() const

Get control qubit num inside this quantum gate.



.. rubric:: Returns:

size_t qubit num

.. index:: pair: function; popBackQuBit
.. _doxid-class_q_panda_1_1_origin_q_gate_1a1b3a19e040e57af230b251e77fce0b2a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* popBackQuBit()

erase qubit vector element at end



.. rubric:: Returns:

Qubit\*

.. index:: pair: function; getQGate
.. _doxid-class_q_panda_1_1_origin_q_gate_1a86a84d652e3bc4259db0ccbd6ab82f77:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`* getQGate() const

Get Quantum Gate.



.. rubric:: Returns:

QuantumGate \*

.. index:: pair: function; setQGate
.. _doxid-class_q_panda_1_1_origin_q_gate_1a56c6c33f9aa4f6e7117617c0569175c5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setQGate(:ref:`QuantumGate<doxid-class_q_g_a_t_e___s_p_a_c_e_1_1_quantum_gate>`*)

Set Quantum Gate.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QuantumGate\*

		- QuantumGate pointer

.. index:: pair: function; setDagger
.. _doxid-class_q_panda_1_1_origin_q_gate_1a92e412a3fe47a10b001dbd8cc4f15346:

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
.. _doxid-class_q_panda_1_1_origin_q_gate_1a252fb142c39d234bed82332ce13b1c46:

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

.. index:: pair: function; isDagger
.. _doxid-class_q_panda_1_1_origin_q_gate_1ac2f8642b4fafff5c9789319673d2a1d4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool isDagger() const

Judge current quantum gate is dagger.



.. rubric:: Returns:

bool

.. index:: pair: function; getControlVector
.. _doxid-class_q_panda_1_1_origin_q_gate_1a3a3c35274292c34bc7fb74ac7be21aa1:

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

.. index:: pair: function; PushBackQuBit
.. _doxid-class_q_panda_1_1_origin_q_gate_1ab2b18fc595acbe9c64a365cf6ac957c4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void PushBackQuBit(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*)

insert qubit vector element at end



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Qubit\*

		- :ref:`Qubit <doxid-class_q_panda_1_1_qubit>` pointer

