.. index:: pair: struct; QPanda::Variational::impl_stack
.. _doxid-struct_q_panda_1_1_variational_1_1impl__stack:

struct QPanda::Variational::impl_stack
======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Implementation class for the stack operation. :ref:`More...<details-struct_q_panda_1_1_variational_1_1impl__stack>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	struct impl_stack: public :ref:`QPanda::Variational::impl<doxid-struct_q_panda_1_1_variational_1_1impl>`
	{
		// fields
	
		int :ref:`m_axis<doxid-struct_q_panda_1_1_variational_1_1impl__stack_1a30d5ad3a3e715c86a837360e08fd17fd>`;

		// construction
	
		:ref:`impl_stack<doxid-struct_q_panda_1_1_variational_1_1impl__stack_1a05fc539027139a7de59db97ec1092530>`(int axis, const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// fields
	
		MatrixXd :ref:`val<doxid-struct_q_panda_1_1_variational_1_1impl_1a192110dfe5013d1fd808aab4f262e241>`;
		bool :ref:`m_is_differentiable<doxid-struct_q_panda_1_1_variational_1_1impl_1ad7bb7cb00dd81ad05e29767d35ae2c4a>`;
		:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` :ref:`op<doxid-struct_q_panda_1_1_variational_1_1impl_1a48c4c2d47ded74e71bf3615945943e3b>`;
		std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :ref:`children<doxid-struct_q_panda_1_1_variational_1_1impl_1ab9026462afdd43c59bfe64fff032691f>`;
		std::vector<std::weak_ptr<:ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl>`>> :ref:`parents<doxid-struct_q_panda_1_1_variational_1_1impl_1a9cd6c23efd4e542bb77b9ad85f1e9529>`;
		MatrixXd :ref:`m_prob<doxid-struct_q_panda_1_1_variational_1_1impl_1af9668071cafbb85c671d03ef55065c87>`;

.. _details-struct_q_panda_1_1_variational_1_1impl__stack:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Implementation class for the stack operation.

Fields
------

.. index:: pair: variable; m_axis
.. _doxid-struct_q_panda_1_1_variational_1_1impl__stack_1a30d5ad3a3e715c86a837360e08fd17fd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int m_axis

stack axis, should be either 0 or 1.

Construction
------------

.. index:: pair: function; impl_stack
.. _doxid-struct_q_panda_1_1_variational_1_1impl__stack_1a05fc539027139a7de59db97ec1092530:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	impl_stack(int axis, const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&)

Construct a new impl stack object by the axis and children. y = stack(axis=0, [a,b,c,d]). It will try to place a,b,c,d into one matrix with the same columns, if axis==1, the same rows.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- axis

		- the stack axis.

