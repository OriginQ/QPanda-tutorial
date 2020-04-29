.. index:: pair: class; QPanda::QNode
.. _doxid-class_q_panda_1_1_q_node:

class QPanda::QNode
===================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum node basic abstract class. :ref:`More...<details-class_q_panda_1_1_q_node>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QNode.h>
	
	class QNode: public :ref:`QPanda::QObject<doxid-class_q_panda_1_1_q_object>`
	{
	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
	};

	// direct descendants

	class :ref:`OriginCircuit<doxid-class_q_panda_1_1_origin_circuit>`;
	class :ref:`OriginClassicalProg<doxid-class_q_panda_1_1_origin_classical_prog>`;
	class :ref:`OriginMeasure<doxid-class_q_panda_1_1_origin_measure>`;
	class :ref:`OriginProgram<doxid-class_q_panda_1_1_origin_program>`;
	class :ref:`OriginQGate<doxid-class_q_panda_1_1_origin_q_gate>`;
	class :ref:`OriginQIf<doxid-class_q_panda_1_1_origin_q_if>`;
	class :ref:`OriginQWhile<doxid-class_q_panda_1_1_origin_q_while>`;
	class :ref:`OriginReset<doxid-class_q_panda_1_1_origin_reset>`;
.. _details-class_q_panda_1_1_q_node:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum node basic abstract class.

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const = 0

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

