.. index:: pair: class; QPanda::OriginCExpr
.. _doxid-class_q_panda_1_1_origin_c_expr:

class QPanda::OriginCExpr
=========================

.. toctree::
	:hidden:

	union_QPanda_OriginCExpr_content_u.rst

Overview
~~~~~~~~

Implementation class of :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>`. :ref:`More...<details-class_q_panda_1_1_origin_c_expr>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginClassicalExpression.h>
	
	class OriginCExpr: public :ref:`QPanda::CExpr<doxid-class_q_panda_1_1_c_expr>`
	{
	public:
		// unions
	
		union :ref:`content_u<doxid-union_q_panda_1_1_origin_c_expr_1_1content__u>`;

		// fields
	
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`m_node_type<doxid-class_q_panda_1_1_origin_c_expr_1a06200078575d1b414cae238707e6f170>`;
		:ref:`qmap_size_t<doxid-namespace_q_panda_1a0fa97ce1598fc0399345a33fde3d9509>` :target:`m_postion<doxid-class_q_panda_1_1_origin_c_expr_1ad38e6bcff5af3e84db2ac767b7914349>`;

		// construction
	
		:target:`OriginCExpr<doxid-class_q_panda_1_1_origin_c_expr_1a147893f0d8b77d72aa0ae1895e8111b3>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* cbit);
	
		:target:`OriginCExpr<doxid-class_q_panda_1_1_origin_c_expr_1a4c41a59ab8de18325e0764836540ea3d>`(
			:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* leftExpr,
			:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* rightExpr,
			int
			);
	
		:target:`OriginCExpr<doxid-class_q_panda_1_1_origin_c_expr_1a91f10db4c5d72555ae12ed307a5fdf9d>`(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`);

		// methods
	
		virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`getLeftExpr<doxid-class_q_panda_1_1_origin_c_expr_1a7cdd3b99a9cc5836109c2a102b8ac4bf>`() const;
		virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`getRightExpr<doxid-class_q_panda_1_1_origin_c_expr_1acfbecdb4f0747c118d0e42f9899975a4>`() const;
		virtual std::string :ref:`getName<doxid-class_q_panda_1_1_origin_c_expr_1a6f71687ee92e44e2ae7e9a177778b3f0>`() const;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_origin_c_expr_1a955ef3a560e3b95332a3fc633376a48b>`() const;
		virtual void :ref:`setLeftExpr<doxid-class_q_panda_1_1_origin_c_expr_1ac9567da5ed0db8ba7b2024cad13c405b>`(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* left_expr);
		virtual void :ref:`setRightExpr<doxid-class_q_panda_1_1_origin_c_expr_1a90ec1812eef078d0fdc70c53ccaca287>`(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* right_expr);
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_origin_c_expr_1ac6bb8c1efaffbd4a76752153246b6684>`() const;
		virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`deepcopy<doxid-class_q_panda_1_1_origin_c_expr_1ab2c89a552b2830db23cdfd6efa9990cb>`() const;
		virtual bool :ref:`checkValidity<doxid-class_q_panda_1_1_origin_c_expr_1a09531b6ba2bd0449978267422348b0c6>`() const;
		virtual void :ref:`getCBitsName<doxid-class_q_panda_1_1_origin_c_expr_1a3463aa26b78398d705968dd2c19c4ca3>`(std::vector<std::string>&);
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_c_expr_1a29bb0f6ae0d7abab4bc5d7205fbbf30c>`() const;
		:ref:`qmap_size_t<doxid-namespace_q_panda_1a0fa97ce1598fc0399345a33fde3d9509>` :target:`getPosition<doxid-class_q_panda_1_1_origin_c_expr_1a727e44155ade4a19d04676ef6cecd03a>`() const;
		void :target:`setPosition<doxid-class_q_panda_1_1_origin_c_expr_1a53edcd58a6cf2d8d5b946a600151562c>`(:ref:`qmap_size_t<doxid-namespace_q_panda_1a0fa97ce1598fc0399345a33fde3d9509>`);
		virtual int :ref:`getContentSpecifier<doxid-class_q_panda_1_1_origin_c_expr_1ae2b73d2194ec1a594154304890259dd3>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`getLeftExpr<doxid-class_q_panda_1_1_c_expr_1a5e8a364369e85a5479f33a2a3eb799f1>`() const = 0;
		virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`getRightExpr<doxid-class_q_panda_1_1_c_expr_1a2cf5895fd37574f8aa1eccc6dbd54cdc>`() const = 0;
		virtual void :ref:`setLeftExpr<doxid-class_q_panda_1_1_c_expr_1a330d8433fa601ac347cec888682df916>`(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* left_expr) = 0;
		virtual void :ref:`setRightExpr<doxid-class_q_panda_1_1_c_expr_1a2bea6675832789ae30a886e3df9c6815>`(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* right_expr) = 0;
		virtual std::string :ref:`getName<doxid-class_q_panda_1_1_c_expr_1a74c9764bd9a65db33aaf5aad6a20a0df>`() const = 0;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_c_expr_1ae27aed1a4e15fd2867d6293201c7a7ea>`() const = 0;
		virtual bool :ref:`checkValidity<doxid-class_q_panda_1_1_c_expr_1a098c3db0d4deefb86e0fd87af3d919b5>`() const = 0;
		virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` :ref:`eval<doxid-class_q_panda_1_1_c_expr_1abb5146bfaf8c28b68b9f68e8f4f28f8b>`() const = 0;
		virtual int :ref:`getContentSpecifier<doxid-class_q_panda_1_1_c_expr_1a0c47e5f9d4c8754136c412bab83ebaf9>`() const = 0;
		virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`deepcopy<doxid-class_q_panda_1_1_c_expr_1aab82ac71c15e94928f7f260554d05473>`() const = 0;
		virtual void :ref:`getCBitsName<doxid-class_q_panda_1_1_c_expr_1ab37db29d84b5f36d76877c2a58e60318>`(std::vector<std::string>&) = 0;

.. _details-class_q_panda_1_1_origin_c_expr:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class of :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>`.

Fields
------

.. index:: pair: variable; m_node_type
.. _doxid-class_q_panda_1_1_origin_c_expr_1a06200078575d1b414cae238707e6f170:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` m_node_type

quantum node type

Methods
-------

.. index:: pair: function; getLeftExpr
.. _doxid-class_q_panda_1_1_origin_c_expr_1a7cdd3b99a9cc5836109c2a102b8ac4bf:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* getLeftExpr() const

Get the Left Expr pointer.



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; getRightExpr
.. _doxid-class_q_panda_1_1_origin_c_expr_1acfbecdb4f0747c118d0e42f9899975a4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* getRightExpr() const

Get the Right Expr pointer.



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; getName
.. _doxid-class_q_panda_1_1_origin_c_expr_1a6f71687ee92e44e2ae7e9a177778b3f0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string getName() const

Get the Name object.



.. rubric:: Returns:

std::string

.. index:: pair: function; getCBit
.. _doxid-class_q_panda_1_1_origin_c_expr_1a955ef3a560e3b95332a3fc633376a48b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* getCBit() const

get classical bit pointer



.. rubric:: Returns:

CBit\*

.. index:: pair: function; setLeftExpr
.. _doxid-class_q_panda_1_1_origin_c_expr_1ac9567da5ed0db8ba7b2024cad13c405b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setLeftExpr(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* left_expr)

Set the Left Expr pointer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- CExpr\*

		- left expr

.. index:: pair: function; setRightExpr
.. _doxid-class_q_panda_1_1_origin_c_expr_1a90ec1812eef078d0fdc70c53ccaca287:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setRightExpr(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* right_expr)

Set the Right Expr pointer.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- CExpr\*

		- right expr

.. index:: pair: function; eval
.. _doxid-class_q_panda_1_1_origin_c_expr_1ac6bb8c1efaffbd4a76752153246b6684:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` eval() const

get value



.. rubric:: Returns:

cbit_size_t

.. index:: pair: function; deepcopy
.. _doxid-class_q_panda_1_1_origin_c_expr_1ab2c89a552b2830db23cdfd6efa9990cb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* deepcopy() const

deep copy this cexpr



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; checkValidity
.. _doxid-class_q_panda_1_1_origin_c_expr_1a09531b6ba2bd0449978267422348b0c6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool checkValidity() const

check validity



.. rubric:: Returns:

true check validity ture

false check validity false

.. index:: pair: function; getCBitsName
.. _doxid-class_q_panda_1_1_origin_c_expr_1a3463aa26b78398d705968dd2c19c4ca3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void getCBitsName(std::vector<std::string>&)

get all cbits name



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<std::string>

		- cibts name vector

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_c_expr_1a29bb0f6ae0d7abab4bc5d7205fbbf30c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

get quantum node type



.. rubric:: Returns:

NodeType

.. index:: pair: function; getContentSpecifier
.. _doxid-class_q_panda_1_1_origin_c_expr_1ae2b73d2194ec1a594154304890259dd3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int getContentSpecifier() const

get content specifier



.. rubric:: Returns:

NodeType

