.. index:: pair: class; QPanda::CExprFactoryHelper
.. _doxid-class_q_panda_1_1_c_expr_factory_helper:

class QPanda::CExprFactoryHelper
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

:ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` factory helper Provide :ref:`CExprFactory <doxid-class_q_panda_1_1_c_expr_factory>` class registration interface for the outside. :ref:`More...<details-class_q_panda_1_1_c_expr_factory_helper>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CExprFactory.h>
	
	class CExprFactoryHelper
	{
	public:
		// construction
	
		:ref:`CExprFactoryHelper<doxid-class_q_panda_1_1_c_expr_factory_helper_1afb3598bc6de86bcf542c4d627bf89eeb>`(std::string name, cbit_constructor_t _Constructor);
		:ref:`CExprFactoryHelper<doxid-class_q_panda_1_1_c_expr_factory_helper_1ac3d05d271b1ae0668b1eedd7123404df>`(std::string, value_constructor_t _Constructor);
		:ref:`CExprFactoryHelper<doxid-class_q_panda_1_1_c_expr_factory_helper_1a1f0f66f6997be1b236a70c0820afa30b>`(std::string, operator_constructor_t _Constructor);
	};
.. _details-class_q_panda_1_1_c_expr_factory_helper:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

:ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` factory helper Provide :ref:`CExprFactory <doxid-class_q_panda_1_1_c_expr_factory>` class registration interface for the outside.

Construction
------------

.. index:: pair: function; CExprFactoryHelper
.. _doxid-class_q_panda_1_1_c_expr_factory_helper_1afb3598bc6de86bcf542c4d627bf89eeb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CExprFactoryHelper(std::string name, cbit_constructor_t _Constructor)

Construct a new :ref:`CExprFactoryHelper <doxid-class_q_panda_1_1_c_expr_factory_helper>` object Call the :ref:`CExprFactory <doxid-class_q_panda_1_1_c_expr_factory>` class registration interface for register the :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` subclass.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- subclass name

	*
		- cbit_constructor_t

		- function

.. index:: pair: function; CExprFactoryHelper
.. _doxid-class_q_panda_1_1_c_expr_factory_helper_1ac3d05d271b1ae0668b1eedd7123404df:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CExprFactoryHelper(std::string, value_constructor_t _Constructor)

Construct a new :ref:`CExprFactoryHelper <doxid-class_q_panda_1_1_c_expr_factory_helper>` object Call the :ref:`CExprFactory <doxid-class_q_panda_1_1_c_expr_factory>` class registration interface for register the :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` subclass.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- subclass name

	*
		- value_constructor_t

		- function

.. index:: pair: function; CExprFactoryHelper
.. _doxid-class_q_panda_1_1_c_expr_factory_helper_1a1f0f66f6997be1b236a70c0820afa30b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CExprFactoryHelper(std::string, operator_constructor_t _Constructor)

Construct a new :ref:`CExprFactoryHelper <doxid-class_q_panda_1_1_c_expr_factory_helper>` object Call the :ref:`CExprFactory <doxid-class_q_panda_1_1_c_expr_factory>` class registration interface for register the :ref:`CExpr <doxid-class_q_panda_1_1_c_expr>` subclass.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- subclass name

	*
		- operator_constructor_t

		- function

