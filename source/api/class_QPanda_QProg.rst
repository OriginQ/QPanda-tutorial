.. index:: pair: class; QPanda::QProg
.. _doxid-class_q_panda_1_1_q_prog:

class QPanda::QProg
===================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum program,can construct quantum circuit,data struct is linked list. :ref:`More...<details-class_q_panda_1_1_q_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgram.h>
	
	class QProg: public :ref:`QPanda::AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`
	{
	public:
		// construction
	
		:target:`QProg<doxid-class_q_panda_1_1_q_prog_1a5aeb2a42cc4d629fa9d41016c8f49a63>`();
		:target:`QProg<doxid-class_q_panda_1_1_q_prog_1ad3d10865c1cc81e85b3b33b087a7e5d7>`(const QProg&);
	
		template <typename Ty>
		:target:`QProg<doxid-class_q_panda_1_1_q_prog_1a234deed8ac5a1055ad7cd1da32c0e9dc>`(Ty& node);
	
		:target:`QProg<doxid-class_q_panda_1_1_q_prog_1adc6cf1d0ff22aab8ad11b8f1be6c600f>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		:target:`QProg<doxid-class_q_panda_1_1_q_prog_1a438fbae8a19e8537fb7d9da1529254ad>`(std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`>);
		:target:`QProg<doxid-class_q_panda_1_1_q_prog_1a03b0dff1bdc2d31d22b456263a667fb1>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& node);
		:target:`QProg<doxid-class_q_panda_1_1_q_prog_1aa00fc95ddd653d44d40aaf59a0070b14>`(QProg& other);

		// methods
	
		std::shared_ptr<:ref:`AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_q_prog_1a9a50f38e2a8b28f4f483cea65e20c22f>`();
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_q_prog_1a52f04bef1c8f76e5d24e107ce15292a1>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
	
		template <typename T>
		QProg& :ref:`operator <<<doxid-class_q_panda_1_1_q_prog_1a5e8afc385e3e7b19e5c43a5535d37e6f>` (:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` node);
	
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_q_prog_1adda1747aa1c60d93d26fe395dd2d3c6d>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_q_prog_1a5009bfd3c6ae07e239ad41590069b076>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_q_prog_1a4fef9766cd8bfeb5a27e7bd6db5e8601>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_q_prog_1a6c602df4ad87db532fd40bb8b83de726>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_q_prog_1a0367d361d37e06aae2ce2e7cc2a272fa>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_q_prog_1a7e13f7b5bc298632c64bdf04c9e3b90f>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&);
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :target:`getNodeType<doxid-class_q_panda_1_1_q_prog_1a48aa62d22a7048ee8c55488fa1bcc1cb>`() const;
		virtual void :ref:`clear<doxid-class_q_panda_1_1_q_prog_1a4539154daf7588ef19dce47f1838454b>`();
		bool :target:`is_empty<doxid-class_q_panda_1_1_q_prog_1ab4b894d5b2465058ea8eb128eb077e48>`();
		virtual size_t :ref:`get_max_qubit_addr<doxid-class_q_panda_1_1_q_prog_1a580e83b888c69247b2d00cf3bf15a78d>`();
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_q_prog_1acf9d0368e058874908b2e7ac44d07b08>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual size_t :ref:`get_used_cbits<doxid-class_q_panda_1_1_q_prog_1ad66c6274b3775ddc40fc656ff57b4623>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&);
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_q_prog_1a1ae4a68e8c4105edc68b6902ec271487>`();
		virtual bool :ref:`is_measure_last_pos<doxid-class_q_panda_1_1_q_prog_1abceefb7494911603bc8a26f8f9ef033e>`();
		virtual std::map<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, bool> :ref:`get_measure_pos<doxid-class_q_panda_1_1_q_prog_1ac19d9f00f216057c4d63b61379fe2585>`();
		virtual std::vector<std::pair<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>> :ref:`get_measure_qubits_cbits<doxid-class_q_panda_1_1_q_prog_1ad8648f6fc7eea1db2f1d76905055fbc7>`();
	};

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
		virtual void :ref:`clear<doxid-class_q_panda_1_1_abstract_quantum_program_1a5f31f3aa64a849d6654eb8ee1f73d3ab>`() = 0;
		virtual size_t :ref:`get_max_qubit_addr<doxid-class_q_panda_1_1_abstract_quantum_program_1a8bdeebab139384217702489f01a7920a>`() = 0;
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_abstract_quantum_program_1abea5d2c41984ba3cf679325137b3067a>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual size_t :ref:`get_used_cbits<doxid-class_q_panda_1_1_abstract_quantum_program_1a8db1ec2607e05c8a11232a0c627572c9>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&) = 0;
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_abstract_quantum_program_1aa910c05e038c58904ef1a49635087622>`() = 0;
		virtual bool :ref:`is_measure_last_pos<doxid-class_q_panda_1_1_abstract_quantum_program_1a1d8232f912af4b86cf1b1770fda0360e>`() = 0;
		virtual std::map<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, bool> :ref:`get_measure_pos<doxid-class_q_panda_1_1_abstract_quantum_program_1ad25f4650c9ac5a30649f260c0ac43a8d>`() = 0;
		virtual std::vector<std::pair<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>> :ref:`get_measure_qubits_cbits<doxid-class_q_panda_1_1_abstract_quantum_program_1a76a02e81401bb45d83a365decfb584d5>`() = 0;

.. _details-class_q_panda_1_1_q_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum program,can construct quantum circuit,data struct is linked list.

Methods
-------

.. index:: pair: function; pushBackNode
.. _doxid-class_q_panda_1_1_q_prog_1a52f04bef1c8f76e5d24e107ce15292a1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void pushBackNode(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>)

Insert a new Node at the end of current quantum circuit.



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
.. _doxid-class_q_panda_1_1_q_prog_1a5e8afc385e3e7b19e5c43a5535d37e6f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	QProg& operator << (:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` node)

Insert new Node at the end of current node.

if T_GATE is QSingleGateNode/QDoubleGateNode/QIfEndNode, deep copy T_GATE and insert it into left :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`; if T_GATE is QIfProg/QWhileProg/QProg,deepcopy IF/WHILE/QProg circuit and insert it into left :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- Node

		- QGate/QCircuit/QProg/QIf/QWhile



.. rubric:: Returns:

:ref:`QPanda::QProg <doxid-class_q_panda_1_1_q_prog>` & quantum program



.. rubric:: See also:

:ref:`QNode <doxid-class_q_panda_1_1_q_node>`

.. index:: pair: function; getFirstNodeIter
.. _doxid-class_q_panda_1_1_q_prog_1adda1747aa1c60d93d26fe395dd2d3c6d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getFirstNodeIter()

Get the first :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getLastNodeIter
.. _doxid-class_q_panda_1_1_q_prog_1a5009bfd3c6ae07e239ad41590069b076:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getLastNodeIter()

Get the last :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getEndNodeIter
.. _doxid-class_q_panda_1_1_q_prog_1a4fef9766cd8bfeb5a27e7bd6db5e8601:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getEndNodeIter()

Get the end :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getHeadNodeIter
.. _doxid-class_q_panda_1_1_q_prog_1a6c602df4ad87db532fd40bb8b83de726:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getHeadNodeIter()

Get the head :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; insertQNode
.. _doxid-class_q_panda_1_1_q_prog_1a0367d361d37e06aae2ce2e7cc2a272fa:

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
.. _doxid-class_q_panda_1_1_q_prog_1a7e13f7b5bc298632c64bdf04c9e3b90f:

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

.. index:: pair: function; clear
.. _doxid-class_q_panda_1_1_q_prog_1a4539154daf7588ef19dce47f1838454b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clear()

Clear all node in current quantum program node.

.. index:: pair: function; get_max_qubit_addr
.. _doxid-class_q_panda_1_1_q_prog_1a580e83b888c69247b2d00cf3bf15a78d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_max_qubit_addr()

Gets the maximum physical address of used qubits.



.. rubric:: Returns:

size_t maximum physical address

.. index:: pair: function; get_used_qubits
.. _doxid-class_q_panda_1_1_q_prog_1acf9d0368e058874908b2e7ac44d07b08:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_used_qubits(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&)

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
.. _doxid-class_q_panda_1_1_q_prog_1ad66c6274b3775ddc40fc656ff57b4623:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_used_cbits(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&)

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
.. _doxid-class_q_panda_1_1_q_prog_1a1ae4a68e8c4105edc68b6902ec271487:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_qgate_num()

Get current quantum program qgate number.



.. rubric:: Returns:

size_t

.. index:: pair: function; is_measure_last_pos
.. _doxid-class_q_panda_1_1_q_prog_1abceefb7494911603bc8a26f8f9ef033e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_measure_last_pos()

Measure operation in the last position of the program.



.. rubric:: Returns:

bool

.. index:: pair: function; get_measure_pos
.. _doxid-class_q_panda_1_1_q_prog_1ac19d9f00f216057c4d63b61379fe2585:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, bool> get_measure_pos()

Get Measure operation position of the program.



.. rubric:: Returns:

std::map<Qubit\*, bool>

.. index:: pair: function; get_measure_qubits_cbits
.. _doxid-class_q_panda_1_1_q_prog_1ad8648f6fc7eea1db2f1d76905055fbc7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::pair<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>> get_measure_qubits_cbits()

Get Measure operation qubits and cbits vector.



.. rubric:: Returns:

std::vector<std::pair<Qubit\*, ClassicalCondition>>

