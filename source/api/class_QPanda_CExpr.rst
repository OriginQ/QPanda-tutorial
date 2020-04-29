.. index:: pair: class; QPanda::CExpr
.. _doxid-class_q_panda_1_1_c_expr:

class QPanda::CExpr
===================

.. toctree::
	:hidden:

Overview
~~~~~~~~

classical expression base class :ref:`More...<details-class_q_panda_1_1_c_expr>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CExprFactory.h>
	
	class CExpr
	{
	public:
		// methods
	
		virtual CExpr* :ref:`getLeftExpr<doxid-class_q_panda_1_1_c_expr_1a5e8a364369e85a5479f33a2a3eb799f1>`() const = 0;
		virtual CExpr* :ref:`getRightExpr<doxid-class_q_panda_1_1_c_expr_1a2cf5895fd37574f8aa1eccc6dbd54cdc>`() const = 0;
		virtual void :ref:`setLeftExpr<doxid-class_q_panda_1_1_c_expr_1a330d8433fa601ac347cec888682df916>`(CExpr* left_expr) = 0;
		virtual void :ref:`setRightExpr<doxid-class_q_panda_1_1_c_expr_1a2bea6675832789ae30a886e3df9c6815>`(CExpr* right_expr) = 0;
		virtual std::string :ref:`getName<doxid-class_q_panda_1_1_c_expr_1a74c9764bd9a65db33aaf5aad6a20a0df>`() const = 0;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_c_expr_1ae27aed1a4e15fd2867d6293201c7a7ea>`() const = 0;
		virtual bool :ref:`checkValidity<doxid-class_q_panda_1_1_c_expr_1a098c3db0d4deefb86e0fd87af3d919b5>`() const = 0;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_c_expr_1abb5146bfaf8c28b68b9f68e8f4f28f8b>`() const = 0;
		virtual int :ref:`getContentSpecifier<doxid-class_q_panda_1_1_c_expr_1a0c47e5f9d4c8754136c412bab83ebaf9>`() const = 0;
		virtual CExpr* :ref:`deepcopy<doxid-class_q_panda_1_1_c_expr_1aab82ac71c15e94928f7f260554d05473>`() const = 0;
		virtual void :ref:`getCBitsName<doxid-class_q_panda_1_1_c_expr_1ab37db29d84b5f36d76877c2a58e60318>`(std::vector<std::string>&) = 0;
	};

	// direct descendants

	class :ref:`OriginCExpr<doxid-class_q_panda_1_1_origin_c_expr>`;
.. _details-class_q_panda_1_1_c_expr:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

classical expression base class

Methods
-------

.. index:: pair: function; getLeftExpr
.. _doxid-class_q_panda_1_1_c_expr_1a5e8a364369e85a5479f33a2a3eb799f1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual CExpr* getLeftExpr() const = 0

Get the Left Expr pointer.



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; getRightExpr
.. _doxid-class_q_panda_1_1_c_expr_1a2cf5895fd37574f8aa1eccc6dbd54cdc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual CExpr* getRightExpr() const = 0

Get the Right Expr pointer.



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; setLeftExpr
.. _doxid-class_q_panda_1_1_c_expr_1a330d8433fa601ac347cec888682df916:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setLeftExpr(CExpr* left_expr) = 0

Set the Left Expr pointer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- CExpr\*

		- left expr

.. index:: pair: function; setRightExpr
.. _doxid-class_q_panda_1_1_c_expr_1a2bea6675832789ae30a886e3df9c6815:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setRightExpr(CExpr* right_expr) = 0

Set the Right Expr pointer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- CExpr\*

		- right expr

.. index:: pair: function; getName
.. _doxid-class_q_panda_1_1_c_expr_1a74c9764bd9a65db33aaf5aad6a20a0df:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getName() const = 0

Get the Name object.



.. rubric:: Returns:

std::string

.. index:: pair: function; getCBit
.. _doxid-class_q_panda_1_1_c_expr_1ae27aed1a4e15fd2867d6293201c7a7ea:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* getCBit() const = 0

get classical bit pointer



.. rubric:: Returns:

CBit\*

.. index:: pair: function; checkValidity
.. _doxid-class_q_panda_1_1_c_expr_1a098c3db0d4deefb86e0fd87af3d919b5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool checkValidity() const = 0

check validity



.. rubric:: Returns:

true check validity ture

false check validity false

.. index:: pair: function; eval
.. _doxid-class_q_panda_1_1_c_expr_1abb5146bfaf8c28b68b9f68e8f4f28f8b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` eval() const = 0

get value



.. rubric:: Returns:

cbit_size_t

.. index:: pair: function; getContentSpecifier
.. _doxid-class_q_panda_1_1_c_expr_1a0c47e5f9d4c8754136c412bab83ebaf9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int getContentSpecifier() const = 0

get specifier of this cexpr



.. rubric:: Returns:

int

.. index:: pair: function; deepcopy
.. _doxid-class_q_panda_1_1_c_expr_1aab82ac71c15e94928f7f260554d05473:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual CExpr* deepcopy() const = 0

deep copy this cexpr



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; getCBitsName
.. _doxid-class_q_panda_1_1_c_expr_1ab37db29d84b5f36d76877c2a58e60318:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void getCBitsName(std::vector<std::string>&) = 0

get all cbits name



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<std::string>

		- cibts name vector

