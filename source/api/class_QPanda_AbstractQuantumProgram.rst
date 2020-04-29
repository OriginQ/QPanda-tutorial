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
	
	class AbstractQuantumProgram
	{
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
	};

	// direct descendants

	class :ref:`OriginProgram<doxid-class_q_panda_1_1_origin_program>`;
	class :ref:`QProg<doxid-class_q_panda_1_1_q_prog>`;
.. _details-class_q_panda_1_1_abstract_quantum_program:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum program basic abstract class.

Methods
-------

.. index:: pair: function; getFirstNodeIter
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a8a7dbbd920bb4c2eff9871f3236e39a8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getFirstNodeIter() = 0

Get the first :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getLastNodeIter
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1acc4046b581ce325ab55d1491eb3cb9a9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getLastNodeIter() = 0

Get the last :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getEndNodeIter
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1aca6ac4bf3cf1a0c158daf19c42e13a6b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getEndNodeIter() = 0

Get the end :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; getHeadNodeIter
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1ac443054fc81e539e26a8b28dcc0c33b3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` getHeadNodeIter() = 0

Get the head :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`.



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; insertQNode
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a75619b19712397a7584c4838a28c5318:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` insertQNode(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0

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
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1afe70cb8d924c9f2285a3445ef5867e97:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` deleteQNode(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&) = 0

Delete a :ref:`QNode <doxid-class_q_panda_1_1_q_node>` at the location specified by :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- NodeIter&

		- specified location



.. rubric:: Returns:

:ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>` Deleted :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>`

.. index:: pair: function; pushBackNode
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a8581223f39a24f0a69e5b58c62c82892:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void pushBackNode(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0

Insert a new node at the end of current quantum program node.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::shared_ptr<QNode>

		- quantum node shared pointer



.. rubric:: See also:

:ref:`QNode <doxid-class_q_panda_1_1_q_node>`

.. index:: pair: function; clear
.. _doxid-class_q_panda_1_1_abstract_quantum_program_1a5f31f3aa64a849d6654eb8ee1f73d3ab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void clear() = 0

Clear all node in current quantum program node.

