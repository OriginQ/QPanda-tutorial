.. index:: pair: class; QPanda::OriginReset
.. _doxid-class_q_panda_1_1_origin_reset:

class QPanda::OriginReset
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class of :ref:`QReset <doxid-class_q_panda_1_1_q_reset>`. :ref:`More...<details-class_q_panda_1_1_origin_reset>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QReset.h>
	
	class OriginReset:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`
	{
	public:
		// construction
	
		:target:`OriginReset<doxid-class_q_panda_1_1_origin_reset_1a84ec071cdf2609ff03da22cac05721b7>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);

		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_origin_reset_1a7b311757b50f10f54be3c2ac9a876a1e>`() const;
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_reset_1a9bec2e757219c7613cac75552d66f1e3>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_abstract_quantum_reset_1a60c3a60eff08e2cfeba20c3662cdb4cb>`() const = 0;

.. _details-class_q_panda_1_1_origin_reset:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`QReset <doxid-class_q_panda_1_1_q_reset>`.

Methods
-------

.. index:: pair: function; getQuBit
.. _doxid-class_q_panda_1_1_origin_reset_1a7b311757b50f10f54be3c2ac9a876a1e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* getQuBit() const

Get reset node qubit address.



.. rubric:: Returns:

:ref:`QPanda::Qubit <doxid-class_q_panda_1_1_qubit>` \* QuBit address

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_reset_1a9bec2e757219c7613cac75552d66f1e3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

