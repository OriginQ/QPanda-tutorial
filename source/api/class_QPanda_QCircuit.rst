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
		virtual QCircuit :ref:`control<doxid-class_q_panda_1_1_q_circuit_1a895b9bbb1b6c9bf825436dd8b3d69aa5>`(const QVec);
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_circuit_1ab3a37b3d981285ad7127eedbb9e0c6b5>`() const;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_q_circuit_1aa09cf54785a8c09befeddf5eff6bc4cc>`() const;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_q_circuit_1a56414aa73904b6ec9433297a62187101>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_q_circuit_1aa469d1cffaf63059e04c3e1dde9d5c1b>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_q_circuit_1ad69ffc60fb639ac326e68a72ae26aed9>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_q_circuit_1aaa07e04eb4206ec2f22288263ff4e868>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_q_circuit_1a57f22108948500db0b56032ceb39a720>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_q_circuit_1a3bca05ba8250155feacfa03d01b56e8b>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_q_circuit_1abaca2f9009304097977ab01e5f935009>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&);
		bool :target:`is_empty<doxid-class_q_panda_1_1_q_circuit_1a2d4ece37b1a27194521d80d569704c65>`();
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_q_circuit_1a40036d789e82cbf24f711674a825e7c6>`(bool isDagger);
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_q_circuit_1a0217be0bb49add047fdc6f43e40909bb>`(const QVec);
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_q_circuit_1adba3dfe84e87dbbd3303cc545cb96219>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const;
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_q_circuit_1a5d63e1573c3f5d55064a0f9714a8b545>`();
	};

	// direct descendants

	class :ref:`HadamardQCircuit<doxid-class_q_panda_1_1_hadamard_q_circuit>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1aab8aacb324825696cf2c7735b8ce17bc>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1af035a5d190751faeea05132aefe1d6c6>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1ad2f723e4ab1bfbb499226d0a6939bd18>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1abffeb4cc2327ec65520da3b127999393>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_abstract_node_manager_1a9b5dc4a55201cd684f010f60835dd40d>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_abstract_node_manager_1a1aab80e3d5b0a1dab7f0804458c6628e>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&) = 0;
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_abstract_node_manager_1ae4b5be219a36fc04e671f00dfe3b6b11>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a9901ebf6ad22292cba7f9911ec3b600f>`() const = 0;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ac4e834af252b8cefb1a9de6ae8781a7d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad25e733d7f1a6bb837ca764135db1c8b>`(bool isDagger) = 0;
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0d810051304b282991d6fd1b87bb437d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0;
		virtual void :ref:`clearControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a3e61c68f5be51f3716506b42e6cf2359>`() = 0;
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a5b7386321461dff5dcee0ae6dcd4812a>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0;
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad054a6feb7cca5f960df1420f0b9a629>`() = 0;

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
.. _doxid-class_q_panda_1_1_q_circuit_1a895b9bbb1b6c9bf825436dd8b3d69aa5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual QCircuit control(const QVec)

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
.. _doxid-class_q_panda_1_1_q_circuit_1a3bca05ba8250155feacfa03d01b56e8b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` insertQNode(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>)

Insert a new :ref:`QNode <doxid-class_q_panda_1_1_q_node>` at the location specified by :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



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

Delete a :ref:`QNode <doxid-class_q_panda_1_1_q_node>` at the location specified by :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



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
.. _doxid-class_q_panda_1_1_q_circuit_1a0217be0bb49add047fdc6f43e40909bb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setControl(const QVec)

Set control qubits to current quantum circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- control qubits vector



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; get_used_qubits
.. _doxid-class_q_panda_1_1_q_circuit_1adba3dfe84e87dbbd3303cc545cb96219:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_used_qubits(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const

Get the used qubits for current quantum circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- used qubits vector



.. rubric:: Returns:

size_t

.. index:: pair: function; get_qgate_num
.. _doxid-class_q_panda_1_1_q_circuit_1a5d63e1573c3f5d55064a0f9714a8b545:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_qgate_num()

Get current quantum circuit qgate number.



.. rubric:: Returns:

size_t

