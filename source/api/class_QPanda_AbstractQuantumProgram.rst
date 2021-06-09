.. index:: pair: class; QPanda::AbstractQuantumProgram
.. _doxid-class_q_panda_1_1_abstract_quantum_program:

class QPanda::AbstractQuantumProgram
====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum program basic abstract class. :ref:`More...<details-class_q_panda_1_1_abstract_quantum_program>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgram.h>
	
	class AbstractQuantumProgram: public :ref:`QPanda::AbstractNodeManager<doxid-class_q_panda_1_1_abstract_node_manager>`
	{
	public:
		// methods
	
		virtual void :ref:`clear<doxid-class_q_panda_1_1_abstract_quantum_program_1a5f31f3aa64a849d6654eb8ee1f73d3ab>`() = 0;
		virtual size_t :ref:`get_max_qubit_addr<doxid-class_q_panda_1_1_abstract_quantum_program_1a8bdeebab139384217702489f01a7920a>`() = 0;
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_abstract_quantum_program_1abea5d2c41984ba3cf679325137b3067a>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual size_t :ref:`get_used_cbits<doxid-class_q_panda_1_1_abstract_quantum_program_1a8db1ec2607e05c8a11232a0c627572c9>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0;
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_abstract_quantum_program_1aa910c05e038c58904ef1a49635087622>`() = 0;
		virtual bool :ref:`is_measure_last_pos<doxid-class_q_panda_1_1_abstract_quantum_program_1a1d8232f912af4b86cf1b1770fda0360e>`() = 0;
		virtual std::map<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, bool> :ref:`get_measure_pos<doxid-class_q_panda_1_1_abstract_quantum_program_1ad25f4650c9ac5a30649f260c0ac43a8d>`() = 0;
		virtual std::vector<std::pair<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>> :ref:`get_measure_qubits_cbits<doxid-class_q_panda_1_1_abstract_quantum_program_1a76a02e81401bb45d83a365decfb584d5>`() = 0;
	};

	// direct descendants

	class :ref:`OriginProgram<doxid-class_q_panda_1_1_origin_program>`;
	class :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`;

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

.. _details-class_q_panda_1_1_abstract_quantum_program:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum program basic abstract class.

Methods
-------

.. index:: pair: function; clear
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a5f31f3aa64a849d6654eb8ee1f73d3ab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clear() = 0

Clear all node in current quantum program node.

.. index:: pair: function; get_max_qubit_addr
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a8bdeebab139384217702489f01a7920a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_max_qubit_addr() = 0

Gets the maximum physical address of used qubits.



.. rubric:: Returns:

size_t maximum physical address

.. index:: pair: function; get_used_qubits
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1abea5d2c41984ba3cf679325137b3067a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_used_qubits(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0

Get the used qubits for current quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- used qubits vector



.. rubric:: Returns:

size_t

.. index:: pair: function; get_used_cbits
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a8db1ec2607e05c8a11232a0c627572c9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_used_cbits(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0

Get the used classical bits for current quantum program.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

		- used qubits vector



.. rubric:: Returns:

size_t

.. index:: pair: function; get_qgate_num
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1aa910c05e038c58904ef1a49635087622:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_qgate_num() = 0

Get current quantum program qgate number.



.. rubric:: Returns:

size_t

.. index:: pair: function; is_measure_last_pos
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a1d8232f912af4b86cf1b1770fda0360e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_measure_last_pos() = 0

Measure operation in the last position of the program.



.. rubric:: Returns:

bool

.. index:: pair: function; get_measure_pos
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1ad25f4650c9ac5a30649f260c0ac43a8d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, bool> get_measure_pos() = 0

Get Measure operation position of the program.



.. rubric:: Returns:

std::map<Qubit\*, bool>

.. index:: pair: function; get_measure_qubits_cbits
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a76a02e81401bb45d83a365decfb584d5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::pair<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>> get_measure_qubits_cbits() = 0

Get Measure operation qubits and cbits vector.



.. rubric:: Returns:

std::vector<std::pair<Qubit\*, ClassicalCondition>>

