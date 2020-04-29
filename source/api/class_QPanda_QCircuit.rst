.. index:: pair: class; QPanda::QCircuit
.. _doxid-class_q_panda_1_1_q_circuit:

class QPanda::QCircuit
======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum circuit basic abstract class. :ref:`More...<details-class_q_panda_1_1_q_circuit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuit.h>
	
	class QCircuit: public :ref:`QPanda::AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`
	{
	public:
		// construction
	
		:target:`QCircuit<doxid-class_q_panda_1_1_q_circuit_1a3b396acd9c516c706fad43a3e57f8795>`();
		:target:`QCircuit<doxid-class_q_panda_1_1_q_circuit_1a6b280c83cae60ce3686a949d2dff5417>`(const QCircuit&);
		:target:`QCircuit<doxid-class_q_panda_1_1_q_circuit_1adf1690671874764771e294382e10c1fd>`(:ref:`QGate<doxid-class_q_panda_1_1_q_gate>`& gate);
		:target:`QCircuit<doxid-class_q_panda_1_1_q_circuit_1aaae1551d994bdb0a7004c2df542ec5f9>`(std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> node);

		// methods
	
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_q_circuit_1a305f41c1b523203e43b01fe42df5c7c1>`();
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_q_circuit_1afee8bb25ac24c51e4c37c5d957139713>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
	
		template <typename T>
		QCircuit& :ref:`operator <<<doxid-class_q_panda_1_1_q_circuit_1a0bfc0cbf8c6e7d8364c7b1c286ff2952>` (:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` node);
	
		virtual QCircuit :ref:`dagger<doxid-class_q_panda_1_1_q_circuit_1ab3c4c560b2b45b89469a00b38ddbebe9>`();
		virtual QCircuit :ref:`control<doxid-class_q_panda_1_1_q_circuit_1a686e7f335e37faa5da17005856a6356b>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_circuit_1ab3a37b3d981285ad7127eedbb9e0c6b5>`() const;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_q_circuit_1aa09cf54785a8c09befeddf5eff6bc4cc>`() const;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_q_circuit_1a56414aa73904b6ec9433297a62187101>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_q_circuit_1aa469d1cffaf63059e04c3e1dde9d5c1b>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_q_circuit_1ad69ffc60fb639ac326e68a72ae26aed9>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_q_circuit_1aaa07e04eb4206ec2f22288263ff4e868>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_q_circuit_1a57f22108948500db0b56032ceb39a720>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_q_circuit_1a101b00b026129a0de08542dff60c305a>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_q_circuit_1abaca2f9009304097977ab01e5f935009>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&);
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_q_circuit_1a40036d789e82cbf24f711674a825e7c6>`(bool isDagger);
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_q_circuit_1afa5b3b8c7aa6ed8d424521df3a02b3b7>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);
	};

	// direct descendants

	class :ref:`HadamardQCircuit<doxid-class_q_panda_1_1_hadamard_q_circuit>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
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

.. _details-class_q_panda_1_1_q_circuit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum circuit basic abstract class.

Methods
-------

.. index:: pair: function; pushBackNode
.. _doxid-class_q_panda_1_1_q_circuit_1afee8bb25ac24c51e4c37c5d957139713:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void pushBackNode(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>)

Insert new Node at the end of current quantum circuit node.



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

.. index:: pair: function; operator<<
.. _doxid-class_q_panda_1_1_q_circuit_1a0bfc0cbf8c6e7d8364c7b1c286ff2952:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	QCircuit& operator << (:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` node)

Insert new Node at the end of current node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- node

		- QGate/QCircuit



.. rubric:: Returns:

:ref:`QPanda::QCircuit <doxid-class_q_panda_1_1_q_circuit>` & quantum circuit



.. rubric:: See also:

:ref:`QNode <doxid-class_q_panda_1_1_q_node>`

.. index:: pair: function; dagger
.. _doxid-class_q_panda_1_1_q_circuit_1ab3c4c560b2b45b89469a00b38ddbebe9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual QCircuit dagger()

Get a dagger circuit base on current quantum circuit node.



.. rubric:: Returns:

:ref:`QPanda::QCircuit <doxid-class_q_panda_1_1_q_circuit>` quantum circuit

.. index:: pair: function; control
.. _doxid-class_q_panda_1_1_q_circuit_1a686e7f335e37faa5da17005856a6356b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual QCircuit control(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`)

Get a control quantumgate base on current quantum circuit node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- control qubits vector



.. rubric:: Returns:

:ref:`QPanda::QCircuit <doxid-class_q_panda_1_1_q_circuit>` quantum circuit



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_q_circuit_1ab3a37b3d981285ad7127eedbb9e0c6b5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; isDagger
.. _doxid-class_q_panda_1_1_q_circuit_1aa09cf54785a8c09befeddf5eff6bc4cc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool isDagger() const

Judge current quantum circuit is dagger.



.. rubric:: Returns:

bool

.. index:: pair: function; getControlVector
.. _doxid-class_q_panda_1_1_q_circuit_1a56414aa73904b6ec9433297a62187101:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getControlVector(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&)

Get control vector from current quantum circuit node.



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
.. _doxid-class_q_panda_1_1_q_circuit_1aa469d1cffaf63059e04c3e1dde9d5c1b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getFirstNodeIter()

Get the first :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getLastNodeIter
.. _doxid-class_q_panda_1_1_q_circuit_1ad69ffc60fb639ac326e68a72ae26aed9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getLastNodeIter()

Get the last :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getEndNodeIter
.. _doxid-class_q_panda_1_1_q_circuit_1aaa07e04eb4206ec2f22288263ff4e868:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getEndNodeIter()

Get the end :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getHeadNodeIter
.. _doxid-class_q_panda_1_1_q_circuit_1a57f22108948500db0b56032ceb39a720:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getHeadNodeIter()

Get the head :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; insertQNode
.. _doxid-class_q_panda_1_1_q_circuit_1a101b00b026129a0de08542dff60c305a:

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
.. _doxid-class_q_panda_1_1_q_circuit_1abaca2f9009304097977ab01e5f935009:

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

.. index:: pair: function; setDagger
.. _doxid-class_q_panda_1_1_q_circuit_1a40036d789e82cbf24f711674a825e7c6:

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
.. _doxid-class_q_panda_1_1_q_circuit_1afa5b3b8c7aa6ed8d424521df3a02b3b7:

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

