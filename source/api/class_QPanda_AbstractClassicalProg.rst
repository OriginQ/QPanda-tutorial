.. index:: pair: class; QPanda::AbstractClassicalProg
.. _doxid-class_q_panda_1_1_abstract_classical_prog:

class QPanda::AbstractClassicalProg
===================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Classical program abstract class. :ref:`More...<details-class_q_panda_1_1_abstract_classical_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ClassicalProgram.h>
	
	class AbstractClassicalProg
	{
	public:
		// methods
	
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :ref:`getExpr<doxid-class_q_panda_1_1_abstract_classical_prog_1ac60d04893715ce3900525675045392b8>`() = 0;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`get_val<doxid-class_q_panda_1_1_abstract_classical_prog_1a74e02336eb2b7234678747a83b38180f>`() = 0;
	};

	// direct descendants

	class :ref:`ClassicalProg<doxid-class_q_panda_1_1_classical_prog>`;
	class :ref:`OriginClassicalProg<doxid-class_q_panda_1_1_origin_classical_prog>`;
.. _details-class_q_panda_1_1_abstract_classical_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Classical program abstract class.

Methods
-------

.. index:: pair: function; getExpr
.. _doxid-class_q_panda_1_1_abstract_classical_prog_1ac60d04893715ce3900525675045392b8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> getExpr() = 0

Get classical expr shared ptr.



.. rubric:: Returns:

std::shared_ptr<CExpr>

.. index:: pair: function; get_val
.. _doxid-class_q_panda_1_1_abstract_classical_prog_1a74e02336eb2b7234678747a83b38180f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` get_val() = 0

Get classical program value.



.. rubric:: Returns:

cbit_size_t

