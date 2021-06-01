.. index:: pair: class; QPanda::AbstractQuantumCircuit
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit:

class QPanda::AbstractQuantumCircuit
====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum circuit basic abstract class. :ref:`More...<details-class_q_panda_1_1_abstract_quantum_circuit>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuit.h>
	
	class AbstractQuantumCircuit: public :ref:`QPanda::AbstractNodeManager<doxid-class_q_panda_1_1_abstract_node_manager>`
	{
	public:
		// methods
	
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a9901ebf6ad22292cba7f9911ec3b600f>`() const = 0;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ac4e834af252b8cefb1a9de6ae8781a7d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad25e733d7f1a6bb837ca764135db1c8b>`(bool isDagger) = 0;
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0d810051304b282991d6fd1b87bb437d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0;
		virtual void :ref:`clearControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a3e61c68f5be51f3716506b42e6cf2359>`() = 0;
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a5b7386321461dff5dcee0ae6dcd4812a>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0;
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad054a6feb7cca5f960df1420f0b9a629>`() = 0;
	};

	// direct descendants

	class :ref:`OriginCircuit<doxid-class_q_panda_1_1_origin_circuit>`;
	class :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`;

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

.. _details-class_q_panda_1_1_abstract_quantum_circuit:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum circuit basic abstract class.

Methods
-------

.. index:: pair: function; isDagger
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit_1a9901ebf6ad22292cba7f9911ec3b600f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool isDagger() const = 0

Judge current quantum circuit is dagger.



.. rubric:: Returns:

bool

.. index:: pair: function; getControlVector
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit_1ac4e834af252b8cefb1a9de6ae8781a7d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getControlVector(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0

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

.. index:: pair: function; setDagger
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad25e733d7f1a6bb837ca764135db1c8b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setDagger(bool isDagger) = 0

Set dagger to current quantum circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		- is dagger

.. index:: pair: function; setControl
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0d810051304b282991d6fd1b87bb437d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setControl(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0

Set control qubits to current quantum circuit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- control qubits vector



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; clearControl
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit_1a3e61c68f5be51f3716506b42e6cf2359:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clearControl() = 0

Clear the control qubits for current quantum circuit.



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

.. index:: pair: function; get_used_qubits
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit_1a5b7386321461dff5dcee0ae6dcd4812a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_used_qubits(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0

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
.. _doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad054a6feb7cca5f960df1420f0b9a629:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_qgate_num() = 0

Get current quantum circuit qgate number.



.. rubric:: Returns:

size_t

