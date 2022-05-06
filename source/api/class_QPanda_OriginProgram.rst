.. index:: pair: class; QPanda::OriginProgram
.. _doxid-class_q_panda_1_1_origin_program:

class QPanda::OriginProgram
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`. :ref:`More...<details-class_q_panda_1_1_origin_program>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgram.h>
	
	class OriginProgram:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractQuantumProgram<doxid-class_q_panda_1_1_abstract_quantum_program>`
	{
	public:
		// methods
	
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_origin_program_1abbbaf3b4f6b866bc7cdf8f72191a3305>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_origin_program_1ac76dc74aac5d82dced00905b8465e4ce>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_origin_program_1a539febf291fd142e10d00ef34fa42705>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_origin_program_1a3387d72885e4bb19f95e2cedb0f204d9>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_origin_program_1a4b099fa404b6832a2ec3cc7f4f5ce105>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_origin_program_1aeb2ae2774001036b8e77aa999193aa8e>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_origin_program_1acf553e4d734100f2f6444c9195cddfa7>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&);
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_program_1aae506f078e9dfd73c88679e323d4f4d7>`() const;
		virtual void :ref:`clear<doxid-class_q_panda_1_1_origin_program_1ae79ff7fae98c24945d49095394d26e2d>`();
		bool :target:`check_insert_node_type<doxid-class_q_panda_1_1_origin_program_1a612c7718151cb65149ed63c3dd839b4b>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node);
		virtual size_t :ref:`get_max_qubit_addr<doxid-class_q_panda_1_1_origin_program_1a53eb0f2d40f051d3ad01c09ebcdce0ee>`();
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_origin_program_1a747348ccc8edf978b319fe69c5b94135>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual size_t :ref:`get_used_cbits<doxid-class_q_panda_1_1_origin_program_1a6585d6ef5c3cc53819347fb6209b58f6>`(std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>&);
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_origin_program_1a1163cc37848d8fb0205567d4b5dd3923>`();
		virtual std::map<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, bool> :ref:`get_measure_pos<doxid-class_q_panda_1_1_origin_program_1aa36793a5104d177c5f1a2c72fe6f46e9>`();
		virtual bool :ref:`is_measure_last_pos<doxid-class_q_panda_1_1_origin_program_1a215f1b4e46a4799f898c5f52911610e6>`();
		virtual std::vector<std::pair<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>> :ref:`get_measure_qubits_cbits<doxid-class_q_panda_1_1_origin_program_1a1a2a8b67b5fcc7b4a23c096a3a7ae342>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
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

.. _details-class_q_panda_1_1_origin_program:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`.

Methods
-------

.. index:: pair: function; pushBackNode
.. _doxid-class_q_panda_1_1_origin_program_1abbbaf3b4f6b866bc7cdf8f72191a3305:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void pushBackNode(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node)

Insert new node at the end of current quantum program node.



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

.. index:: pair: function; getFirstNodeIter
.. _doxid-class_q_panda_1_1_origin_program_1ac76dc74aac5d82dced00905b8465e4ce:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getFirstNodeIter()

Get the first :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getLastNodeIter
.. _doxid-class_q_panda_1_1_origin_program_1a539febf291fd142e10d00ef34fa42705:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getLastNodeIter()

Get the last :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getEndNodeIter
.. _doxid-class_q_panda_1_1_origin_program_1a3387d72885e4bb19f95e2cedb0f204d9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getEndNodeIter()

Get the end :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getHeadNodeIter
.. _doxid-class_q_panda_1_1_origin_program_1a4b099fa404b6832a2ec3cc7f4f5ce105:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getHeadNodeIter()

Get the head :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; insertQNode
.. _doxid-class_q_panda_1_1_origin_program_1aeb2ae2774001036b8e77aa999193aa8e:

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
.. _doxid-class_q_panda_1_1_origin_program_1acf553e4d734100f2f6444c9195cddfa7:

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

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_program_1aae506f078e9dfd73c88679e323d4f4d7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; clear
.. _doxid-class_q_panda_1_1_origin_program_1ae79ff7fae98c24945d49095394d26e2d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clear()

Clear all node in current quantum program node.



.. rubric:: Returns:

void

.. index:: pair: function; get_max_qubit_addr
.. _doxid-class_q_panda_1_1_origin_program_1a53eb0f2d40f051d3ad01c09ebcdce0ee:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_max_qubit_addr()

Gets the maximum physical address of used qubits.



.. rubric:: Returns:

size_t maximum physical address

.. index:: pair: function; get_used_qubits
.. _doxid-class_q_panda_1_1_origin_program_1a747348ccc8edf978b319fe69c5b94135:

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
.. _doxid-class_q_panda_1_1_origin_program_1a6585d6ef5c3cc53819347fb6209b58f6:

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
.. _doxid-class_q_panda_1_1_origin_program_1a1163cc37848d8fb0205567d4b5dd3923:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual size_t get_qgate_num()

Get current quantum program qgate number.



.. rubric:: Returns:

size_t

.. index:: pair: function; get_measure_pos
.. _doxid-class_q_panda_1_1_origin_program_1aa36793a5104d177c5f1a2c72fe6f46e9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::map<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, bool> get_measure_pos()

Get Measure operation position of the program.



.. rubric:: Returns:

std::map<Qubit\*, bool>

.. index:: pair: function; is_measure_last_pos
.. _doxid-class_q_panda_1_1_origin_program_1a215f1b4e46a4799f898c5f52911610e6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool is_measure_last_pos()

Measure operation in the last position of the program.



.. rubric:: Returns:

bool

.. index:: pair: function; get_measure_qubits_cbits
.. _doxid-class_q_panda_1_1_origin_program_1a1a2a8b67b5fcc7b4a23c096a3a7ae342:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::vector<std::pair<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*, :ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`>> get_measure_qubits_cbits()

Get Measure operation qubits and cbits vector.



.. rubric:: Returns:

std::vector<std::pair<Qubit\*, ClassicalCondition>>

