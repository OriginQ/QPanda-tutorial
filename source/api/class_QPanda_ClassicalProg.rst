.. index:: pair: class; QPanda::ClassicalProg
.. _doxid-class_q_panda_1_1_classical_prog:

class QPanda::ClassicalProg
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Classical program class. :ref:`More...<details-class_q_panda_1_1_classical_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ClassicalProgram.h>
	
	class ClassicalProg: public :ref:`QPanda::AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`
	{
	public:
		// construction
	
		:ref:`ClassicalProg<doxid-class_q_panda_1_1_classical_prog_1ab359b2cd641837f51dbf04fbcec77158>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& classical_cond);
		:ref:`ClassicalProg<doxid-class_q_panda_1_1_classical_prog_1a66791d3d4a898244940573837f407ad7>`(const ClassicalProg& old);
		:target:`ClassicalProg<doxid-class_q_panda_1_1_classical_prog_1a5991d2bc8a6cb313bc79731e4746b187>`(std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> node);

		// methods
	
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_classical_prog_1a4bd939b333efeddf051b0ab69a153f4a>`() const;
		std::shared_ptr<:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_classical_prog_1a3d8e970b6e5441a5a11b4f38d5bf2047>`();
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_classical_prog_1a4b9c6fdc2bfda5c1fe2a166cf9f61c94>`();
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :ref:`getExpr<doxid-class_q_panda_1_1_classical_prog_1a12d166515b8d6cd1c6d9371226211e1c>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :ref:`getExpr<doxid-class_q_panda_1_1_abstract_classical_prog_1ac60d04893715ce3900525675045392b8>`() = 0;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_abstract_classical_prog_1aeb45d67fe6f5783158b010c863d489fa>`() = 0;

.. _details-class_q_panda_1_1_classical_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Classical program class.

The proxy class of the :ref:`AbstractClassicalProg <doxid-class_q_panda_1_1_abstract_classical_prog>` implementation class

Construction
------------

.. index:: pair: function; ClassicalProg
.. _doxid-class_q_panda_1_1_classical_prog_1ab359b2cd641837f51dbf04fbcec77158:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalProg(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& classical_cond)

Construct a new Classical Prog object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- classical_cond

		- Target classical condition

.. index:: pair: function; ClassicalProg
.. _doxid-class_q_panda_1_1_classical_prog_1a66791d3d4a898244940573837f407ad7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalProg(const ClassicalProg& old)

Construct a new Classical Prog object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- old

		- Target classical program

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_classical_prog_1a4bd939b333efeddf051b0ab69a153f4a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; eval
.. _doxid-class_q_panda_1_1_classical_prog_1a4b9c6fdc2bfda5c1fe2a166cf9f61c94:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` eval()

Get classical program value.



.. rubric:: Returns:

cbit_size_t

.. index:: pair: function; getExpr
.. _doxid-class_q_panda_1_1_classical_prog_1a12d166515b8d6cd1c6d9371226211e1c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> getExpr()

Get classical expr shared ptr.



.. rubric:: Returns:

std::shared_ptr<CExpr>

