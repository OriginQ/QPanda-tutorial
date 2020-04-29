.. index:: pair: class; QPanda::OriginCircuit
.. _doxid-class_q_panda_1_1_origin_circuit:

class QPanda::OriginCircuit
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`. :ref:`More...<details-class_q_panda_1_1_origin_circuit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuit.h>
	
	class OriginCircuit:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`
	{
	public:
		// methods
	
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_origin_circuit_1accb08ac60b039b7cd73701f3f487ea08>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_origin_circuit_1ab829ebc2f3231193710d100dae2f966e>`(bool isDagger);
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_origin_circuit_1a8ef52cb45260e28e86ac94261313d664>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_circuit_1ab1a3d0a35640d9e78736ff4ff5140be8>`() const;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_origin_circuit_1a76c8eea1a291bffbfa2c168e31cfe880>`() const;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_origin_circuit_1af49cd90d7105b7477ed8a35227af20b2>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_origin_circuit_1a2cdc2ed7434e40aa8423dda374bdf202>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_origin_circuit_1abe8561fc4a56d2bd288f7ef34272dcd3>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_origin_circuit_1a635c3ddf31519b53956ba549a6c7097e>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_origin_circuit_1aa0411fe9a8b8afb35ef042b57437d895>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_origin_circuit_1a935809b0630e6f52e9c4b26c15630b2d>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_origin_circuit_1a2d78dc21b81592daa1a51ade2c0cc6b0>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&);
		virtual void :ref:`clearControl<doxid-class_q_panda_1_1_origin_circuit_1ae11603555437c0f54cf62113cbb9b5b6>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad13a60e0771b9bf6a984aff13967c15e>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0c958083867fb03f0606ccc74ed13800>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a4732224c13dc949d2ed26388138dd0d3>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1af6f1864ea355c13eaa4e14bddf64934c>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_abstract_quantum_circuit_1aeabd63772ee53de4c41141b7afef6d5f>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_abstract_quantum_circuit_1aded25dd1af1558f04d6ad72736ab2ce9>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&) = 0;
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a99f9d60e21e0e4d49c64e3253ff03001>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a9901ebf6ad22292cba7f9911ec3b600f>`() const = 0;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ac4e834af252b8cefb1a9de6ae8781a7d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad25e733d7f1a6bb837ca764135db1c8b>`(bool isDagger) = 0;
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0d810051304b282991d6fd1b87bb437d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0;
		virtual void :ref:`clearControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a3e61c68f5be51f3716506b42e6cf2359>`() = 0;

.. _details-class_q_panda_1_1_origin_circuit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`.

Methods
-------

.. index:: pair: function; pushBackNode
.. _doxid-class_q_panda_1_1_origin_circuit_1accb08ac60b039b7cd73701f3f487ea08:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void pushBackNode(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>)

Insert a new Node at the end of current quantum circuit node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QNode\*

		- quantum node



.. rubric:: Returns:

void



.. rubric:: See also:

:ref:`QNode <doxid-class_q_panda_1_1_q_node>`

.. index:: pair: function; setDagger
.. _doxid-class_q_panda_1_1_origin_circuit_1ab829ebc2f3231193710d100dae2f966e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setDagger(bool isDagger)

Set dagger to current quantum circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- is dagger

.. index:: pair: function; setControl
.. _doxid-class_q_panda_1_1_origin_circuit_1a8ef52cb45260e28e86ac94261313d664:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setControl(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`)

Set control qubits to current quantum circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- control qubits vector



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_circuit_1ab1a3d0a35640d9e78736ff4ff5140be8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; isDagger
.. _doxid-class_q_panda_1_1_origin_circuit_1a76c8eea1a291bffbfa2c168e31cfe880:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool isDagger() const

Judge current quantum circuit is dagger.



.. rubric:: Returns:

bool

.. index:: pair: function; getControlVector
.. _doxid-class_q_panda_1_1_origin_circuit_1af49cd90d7105b7477ed8a35227af20b2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getControlVector(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&)

Get control vector fron current quantum circuit node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- qubits vector



.. rubric:: Returns:

bool



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; getFirstNodeIter
.. _doxid-class_q_panda_1_1_origin_circuit_1a2cdc2ed7434e40aa8423dda374bdf202:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getFirstNodeIter()

Get the first :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getLastNodeIter
.. _doxid-class_q_panda_1_1_origin_circuit_1abe8561fc4a56d2bd288f7ef34272dcd3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getLastNodeIter()

Get the last :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getEndNodeIter
.. _doxid-class_q_panda_1_1_origin_circuit_1a635c3ddf31519b53956ba549a6c7097e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getEndNodeIter()

Get the end :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getHeadNodeIter
.. _doxid-class_q_panda_1_1_origin_circuit_1aa0411fe9a8b8afb35ef042b57437d895:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getHeadNodeIter()

Get the head :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; insertQNode
.. _doxid-class_q_panda_1_1_origin_circuit_1a935809b0630e6f52e9c4b26c15630b2d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` insertQNode(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>)

Insert a new :ref:`QNode <doxid-class_q_panda_1_1_q_node>` at the location specified by :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- NodeIter&

		- specified location

	*
		- std::shared_ptr<QNode>

		- Inserted :ref:`QNode <doxid-class_q_panda_1_1_q_node>`



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; deleteQNode
.. _doxid-class_q_panda_1_1_origin_circuit_1a2d78dc21b81592daa1a51ade2c0cc6b0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` deleteQNode(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&)

Delete a :ref:`QNode <doxid-class_q_panda_1_1_q_node>` at the location specified by :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- NodeIter&

		- specified location



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>` Deleted :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; clearControl
.. _doxid-class_q_panda_1_1_origin_circuit_1ae11603555437c0f54cf62113cbb9b5b6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearControl()

Clear the control qubits for current quantum circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- control qubits vector



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

