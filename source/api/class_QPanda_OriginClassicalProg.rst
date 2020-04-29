.. index:: pair: class; QPanda::OriginClassicalProg
.. _doxid-class_q_panda_1_1_origin_classical_prog:

class QPanda::OriginClassicalProg
=================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Origin classical program class. :ref:`More...<details-class_q_panda_1_1_origin_classical_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ClassicalProgram.h>
	
	class OriginClassicalProg:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`
	{
	public:
		// construction
	
		:ref:`OriginClassicalProg<doxid-class_q_panda_1_1_origin_classical_prog_1acd8679bd3f116369396234a279f50c59>`(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&);

		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_classical_prog_1a741b2e1666c45e61742398cffe9f29eb>`() const;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_origin_classical_prog_1af354f9c774a94a5a14b256d75c97cc79>`();
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :ref:`getExpr<doxid-class_q_panda_1_1_origin_classical_prog_1aea781941d5a9e2240128b956d795cac3>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :ref:`getExpr<doxid-class_q_panda_1_1_abstract_classical_prog_1ac60d04893715ce3900525675045392b8>`() = 0;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_abstract_classical_prog_1aeb45d67fe6f5783158b010c863d489fa>`() = 0;

.. _details-class_q_panda_1_1_origin_classical_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Origin classical program class.

Implementation class of :ref:`ClassicalProg <doxid-class_q_panda_1_1_classical_prog>` This class type can hold classical expr and insert into QNodeMap

Construction
------------

.. index:: pair: function; OriginClassicalProg
.. _doxid-class_q_panda_1_1_origin_classical_prog_1acd8679bd3f116369396234a279f50c59:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginClassicalProg(:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`&)

Construct a new Origin Classical Prog object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- classical_cond

		- Target classical condition

Methods
-------

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_classical_prog_1a741b2e1666c45e61742398cffe9f29eb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

.. index:: pair: function; eval
.. _doxid-class_q_panda_1_1_origin_classical_prog_1af354f9c774a94a5a14b256d75c97cc79:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` eval()

Get classical program value.



.. rubric:: Returns:

cbit_size_t

.. index:: pair: function; getExpr
.. _doxid-class_q_panda_1_1_origin_classical_prog_1aea781941d5a9e2240128b956d795cac3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> getExpr()

Get classical expr shared ptr.



.. rubric:: Returns:

std::shared_ptr<CExpr>

