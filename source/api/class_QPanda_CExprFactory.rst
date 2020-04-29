.. index:: pair: class; QPanda::CExprFactory
.. _doxid-class_q_panda_1_1_c_expr_factory:

class QPanda::CExprFactory
==========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

classical expr class factory :ref:`More...<details-class_q_panda_1_1_c_expr_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CExprFactory.h>
	
	class CExprFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*)> :ref:`cbit_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a33da1fb910b15ca1dd1c38b794779bb6>`;
		typedef std::map<std::string, :ref:`cbit_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a33da1fb910b15ca1dd1c38b794779bb6>`> :ref:`cbit_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1ad3835068ce3fbcc9d5cfa2a54073cfd4>`;
		typedef std::function<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)> :ref:`value_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1ac0693c72cc0d94855797b822b8ed2a89>`;
		typedef std::map<std::string, :ref:`value_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1ac0693c72cc0d94855797b822b8ed2a89>`> :ref:`value_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1afe3a2089f64b8e59cd1c5bab04c66c66>`;
		typedef std::function<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*, :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*, int)> :ref:`operator_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a77fe0f058a199ccb167c91a3a555fcff>`;
		typedef std::map<std::string, :ref:`operator_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a77fe0f058a199ccb167c91a3a555fcff>`> :ref:`operator_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1adc8443b051d6ad4837da3e25a76cdf16>`;

		// fields
	
		:ref:`cbit_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1ad3835068ce3fbcc9d5cfa2a54073cfd4>` :ref:`_CExpr_CBit_Constructor<doxid-class_q_panda_1_1_c_expr_factory_1ab5a41323ff62c85fc37b20a5c3ac31e2>`;
		:ref:`value_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1afe3a2089f64b8e59cd1c5bab04c66c66>` :ref:`_CExpr_Value_Constructor<doxid-class_q_panda_1_1_c_expr_factory_1afab6043dcfc4ac40a54976eb606c6647>`;
		:ref:`operator_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1adc8443b051d6ad4837da3e25a76cdf16>` :ref:`_CExpr_Operator_Constructor<doxid-class_q_panda_1_1_c_expr_factory_1ade5108e8aadc5c5fd171e06f46b0513f>`;

		// methods
	
		static CExprFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_c_expr_factory_1a77132239f228f6c77ec467637aacf1b9>`();
		:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`GetCExprByCBit<doxid-class_q_panda_1_1_c_expr_factory_1a656255b4e70ae84db3876173ed1c7f89>`(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* cbit);
		void :ref:`registerclass_CBit_<doxid-class_q_panda_1_1_c_expr_factory_1a3d8e91b630323d599c9857df989cdf9c>`(std::string& name, :ref:`cbit_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a33da1fb910b15ca1dd1c38b794779bb6>` constructor);
		:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`GetCExprByValue<doxid-class_q_panda_1_1_c_expr_factory_1af35e4339f12121a288ab71d894ad6ed8>`(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value);
		void :ref:`registerclass_Value_<doxid-class_q_panda_1_1_c_expr_factory_1ab51fa228e8f92544ab408231e170a187>`(std::string&, :ref:`value_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1ac0693c72cc0d94855797b822b8ed2a89>`);
		:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* :ref:`GetCExprByOperation<doxid-class_q_panda_1_1_c_expr_factory_1aecbc3ad256b7423a91ad8bbf4408a2aa>`(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* left_cexpr, :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* right_cexpr, int operat);
		void :ref:`registerclass_operator_<doxid-class_q_panda_1_1_c_expr_factory_1a20ef3f0cb0c8defb7f77c66862a05c29>` (std::string&, :ref:`operator_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a77fe0f058a199ccb167c91a3a555fcff>`);
	};
.. _details-class_q_panda_1_1_c_expr_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

classical expr class factory

Typedefs
--------

.. index:: pair: typedef; cbit_constructor_t
.. _doxid-class_q_panda_1_1_c_expr_factory_1a33da1fb910b15ca1dd1c38b794779bb6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*)> cbit_constructor_t

We typedef the cbit_constructor_t is a constructor that use cbit create cexpr.

.. index:: pair: typedef; cbit_constructor_map_t
.. _doxid-class_q_panda_1_1_c_expr_factory_1ad3835068ce3fbcc9d5cfa2a54073cfd4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::map<std::string, :ref:`cbit_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a33da1fb910b15ca1dd1c38b794779bb6>`> cbit_constructor_map_t

We typedef the cbit_constructor_map_t is a collection of constructors that use cbit create cexpr.

.. index:: pair: typedef; value_constructor_t
.. _doxid-class_q_panda_1_1_c_expr_factory_1ac0693c72cc0d94855797b822b8ed2a89:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>`)> value_constructor_t

We typedef the value_constructor_t is a constructor that use value create cexpr.

.. index:: pair: typedef; value_constructor_map_t
.. _doxid-class_q_panda_1_1_c_expr_factory_1afe3a2089f64b8e59cd1c5bab04c66c66:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::map<std::string, :ref:`value_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1ac0693c72cc0d94855797b822b8ed2a89>`> value_constructor_map_t

We typedef the value_constructor_map_t is a collection of constructors that use value create cexpr.

.. index:: pair: typedef; operator_constructor_t
.. _doxid-class_q_panda_1_1_c_expr_factory_1a77fe0f058a199ccb167c91a3a555fcff:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::function<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*, :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`*, int)> operator_constructor_t

We typedef the operator_constructor_t is a constructor that use operator create cexpr.

.. index:: pair: typedef; operator_constructor_map_t
.. _doxid-class_q_panda_1_1_c_expr_factory_1adc8443b051d6ad4837da3e25a76cdf16:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::map<std::string, :ref:`operator_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a77fe0f058a199ccb167c91a3a555fcff>`> operator_constructor_map_t

We typedef the operator_constructor_map_t is a collection of constructors that use operator create cexpr.

Fields
------

.. index:: pair: variable; _CExpr_CBit_Constructor
.. _doxid-class_q_panda_1_1_c_expr_factory_1ab5a41323ff62c85fc37b20a5c3ac31e2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`cbit_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1ad3835068ce3fbcc9d5cfa2a54073cfd4>` _CExpr_CBit_Constructor

A collection of constructors that use cbit create cexpr.

.. index:: pair: variable; _CExpr_Value_Constructor
.. _doxid-class_q_panda_1_1_c_expr_factory_1afab6043dcfc4ac40a54976eb606c6647:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`value_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1afe3a2089f64b8e59cd1c5bab04c66c66>` _CExpr_Value_Constructor

A collection of constructors that use value create cexpr.

.. index:: pair: variable; _CExpr_Operator_Constructor
.. _doxid-class_q_panda_1_1_c_expr_factory_1ade5108e8aadc5c5fd171e06f46b0513f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`operator_constructor_map_t<doxid-class_q_panda_1_1_c_expr_factory_1adc8443b051d6ad4837da3e25a76cdf16>` _CExpr_Operator_Constructor

A collection of constructors that use operator create cexpr.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_c_expr_factory_1a77132239f228f6c77ec467637aacf1b9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static CExprFactory& GetFactoryInstance()

Get the Factory Instance object.



.. rubric:: Returns:

:ref:`CExprFactory <doxid-class_q_panda_1_1_c_expr_factory>` &

.. index:: pair: function; GetCExprByCBit
.. _doxid-class_q_panda_1_1_c_expr_factory_1a656255b4e70ae84db3876173ed1c7f89:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* GetCExprByCBit(:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* cbit)

Get cexpr by cbit.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cbit

		- target cbit



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; registerclass_CBit_
.. _doxid-class_q_panda_1_1_c_expr_factory_1a3d8e91b630323d599c9857df989cdf9c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void registerclass_CBit_(std::string& name, :ref:`cbit_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a33da1fb910b15ca1dd1c38b794779bb6>` constructor)

Registration function This function can be used to register constructors that inherit subclasses of the :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` class.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- name subclass name

	*
		- cbit_constructor_t

		- constructor subclass constructor

.. index:: pair: function; GetCExprByValue
.. _doxid-class_q_panda_1_1_c_expr_factory_1af35e4339f12121a288ab71d894ad6ed8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* GetCExprByValue(:ref:`cbit_size_t<doxid-namespace_q_panda_1a389dd5cda589523f080c1f8671f5ae5a>` value)

Get cexpr by value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- cbit_size_t

		- target value



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; registerclass_Value_
.. _doxid-class_q_panda_1_1_c_expr_factory_1ab51fa228e8f92544ab408231e170a187:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void registerclass_Value_(std::string&, :ref:`value_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1ac0693c72cc0d94855797b822b8ed2a89>`)

Registration function This function can be used to register constructors that inherit subclasses of the :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` class.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- subclass name

	*
		- value_constructor_t

		- subclass constructor

.. index:: pair: function; GetCExprByOperation
.. _doxid-class_q_panda_1_1_c_expr_factory_1aecbc3ad256b7423a91ad8bbf4408a2aa:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* GetCExprByOperation(:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* left_cexpr, :ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`* right_cexpr, int operat)

Get cexpr by Operation.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- CExpr\*

		- left :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>`

	*
		- CExpr\*

		- right :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>`

	*
		- int

		- target operator



.. rubric:: Returns:

CExpr\*

.. index:: pair: function; registerclass_operator_
.. _doxid-class_q_panda_1_1_c_expr_factory_1a20ef3f0cb0c8defb7f77c66862a05c29:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void registerclass_operator_ (std::string&, :ref:`operator_constructor_t<doxid-class_q_panda_1_1_c_expr_factory_1a77fe0f058a199ccb167c91a3a555fcff>`)

Registration function This function can be used to register constructors that inherit subclasses of the :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` class.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- subclass name

	*
		- operator_constructor_t

		- subclass constructor

