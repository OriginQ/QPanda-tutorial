.. index:: pair: class; QPanda::ClassicalCondition
.. _doxid-class_q_panda_1_1_classical_condition:

class QPanda::ClassicalCondition
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Classical condition class Proxy class of cexpr class. :ref:`More...<details-class_q_panda_1_1_classical_condition>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ClassicalConditionInterface.h>
	
	class ClassicalCondition
	{
	public:
		// construction
	
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition_1a475166baebe6cb84c40b7a9346477da5>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* cbit);
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition_1a9aa1e7de30c856bb2ad0f4bd52fb611f>`(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value);
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition_1aa2553bb0339b0cb10aa1a77c04abf9cf>`(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* cexpr);
		:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition_1a5e9cdf35a531ff95c076e43bf750900b>`(const ClassicalCondition& old);

		// methods
	
		std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :ref:`getExprPtr<doxid-class_q_panda_1_1_classical_condition_1a1d391947e9e439f9a64083fbe9b1d95f>`() const;
		:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_classical_condition_1aa9d33bdab8c1b9838a5753f9675ed541>`();
		void :ref:`setValue<doxid-class_q_panda_1_1_classical_condition_1abc871295162c891aca793f14417338b3>`(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);
		bool :ref:`checkValidity<doxid-class_q_panda_1_1_classical_condition_1a0ebbad048cafc03169be45d482a2c38e>`() const;
		ClassicalCondition :ref:`operator =<doxid-class_q_panda_1_1_classical_condition_1ae94c43b3e9fc438b0a587ada57a066e2>` (ClassicalCondition old);
		ClassicalCondition :ref:`operator =<doxid-class_q_panda_1_1_classical_condition_1af37ae5798411986ed9995709f850008d>` (const :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value);
	};
.. _details-class_q_panda_1_1_classical_condition:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Classical condition class Proxy class of cexpr class.

Construction
------------

.. index:: pair: function; ClassicalCondition
.. _doxid-class_q_panda_1_1_classical_condition_1a475166baebe6cb84c40b7a9346477da5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalCondition(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* cbit)

Construct a new Classical Condition object by cbit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cbit

		- target cbit ptr

.. index:: pair: function; ClassicalCondition
.. _doxid-class_q_panda_1_1_classical_condition_1a9aa1e7de30c856bb2ad0f4bd52fb611f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalCondition(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value)

Construct a new Classical Condition object by valie.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cbit

		- target cbit ptr

.. index:: pair: function; ClassicalCondition
.. _doxid-class_q_panda_1_1_classical_condition_1aa2553bb0339b0cb10aa1a77c04abf9cf:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalCondition(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* cexpr)

Construct a new Classical Condition object by :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cexpr

		- target cexpr ptr

.. index:: pair: function; ClassicalCondition
.. _doxid-class_q_panda_1_1_classical_condition_1a5e9cdf35a531ff95c076e43bf750900b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalCondition(const ClassicalCondition& old)

Construct a new Classical Condition object by :ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- old

		- target :ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` object

Methods
-------

.. index:: pair: function; getExprPtr
.. _doxid-class_q_panda_1_1_classical_condition_1a1d391947e9e439f9a64083fbe9b1d95f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> getExprPtr() const

Get the Expr Ptr.



.. rubric:: Returns:

std::shared_ptr<CExpr>

.. index:: pair: function; eval
.. _doxid-class_q_panda_1_1_classical_condition_1aa9d33bdab8c1b9838a5753f9675ed541:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` eval()

Get the value of the current object.



.. rubric:: Returns:

cbit_size_t

.. index:: pair: function; setValue
.. _doxid-class_q_panda_1_1_classical_condition_1abc871295162c891aca793f14417338b3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setValue(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)

Set the Value of the current object.

.. index:: pair: function; checkValidity
.. _doxid-class_q_panda_1_1_classical_condition_1a0ebbad048cafc03169be45d482a2c38e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool checkValidity() const

Check validity.



.. rubric:: Returns:

true check validity ture

false check validity false

.. index:: pair: function; operator=
.. _doxid-class_q_panda_1_1_classical_condition_1ae94c43b3e9fc438b0a587ada57a066e2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalCondition operator = (ClassicalCondition old)

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` assgen function by :ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- old

		- target :ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` object



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

.. index:: pair: function; operator=
.. _doxid-class_q_panda_1_1_classical_condition_1af37ae5798411986ed9995709f850008d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ClassicalCondition operator = (const :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value)

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>` assgen function by value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value

		- target value



.. rubric:: Returns:

:ref:`ClassicalCondition <doxid-class_q_panda_1_1_classical_condition>`

