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
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_abstract_quantum_program_1a8a7dbbd920bb4c2eff9871f3236e39a8>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_abstract_quantum_program_1acc4046b581ce325ab55d1491eb3cb9a9>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_abstract_quantum_program_1aca6ac4bf3cf1a0c158daf19c42e13a6b>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_abstract_quantum_program_1ac443054fc81e539e26a8b28dcc0c33b3>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_abstract_quantum_program_1a75619b19712397a7584c4838a28c5318>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_abstract_quantum_program_1afe70cb8d924c9f2285a3445ef5867e97>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&) = 0;
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_abstract_quantum_program_1a8581223f39a24f0a69e5b58c62c82892>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual void :ref:`clear<doxid-class_q_panda_1_1_abstract_quantum_program_1a5f31f3aa64a849d6654eb8ee1f73d3ab>`() = 0;

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

Insert a new node at the end of current quantum program node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::shared_ptr<QNode>

		- quantum node shared pointer



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
.. _doxid-class_q_panda_1_1_q_prog_1a7e13f7b5bc298632c64bdf04c9e3b90f:

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

.. index:: pair: function; clear
.. _doxid-class_q_panda_1_1_q_prog_1a4539154daf7588ef19dce47f1838454b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clear()

Clear all node in current quantum program node.

