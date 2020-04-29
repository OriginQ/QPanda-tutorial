.. index:: pair: struct; QPanda::Variational::impl
.. _doxid-struct_q_panda_1_1_variational_1_1impl:

struct QPanda::Variational::impl
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

implementation class for the var. Impl only includes classical operator with fixed number of arguments. :ref:`More...<details-struct_q_panda_1_1_variational_1_1impl>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	struct impl
	{
		// fields
	
		MatrixXd :ref:`val<doxid-struct_q_panda_1_1_variational_1_1impl_1a192110dfe5013d1fd808aab4f262e241>`;
		bool :ref:`m_is_differentiable<doxid-struct_q_panda_1_1_variational_1_1impl_1ad7bb7cb00dd81ad05e29767d35ae2c4a>`;
		:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` :ref:`op<doxid-struct_q_panda_1_1_variational_1_1impl_1a48c4c2d47ded74e71bf3615945943e3b>`;
		std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :ref:`children<doxid-struct_q_panda_1_1_variational_1_1impl_1ab9026462afdd43c59bfe64fff032691f>`;
		std::vector<std::weak_ptr<impl>> :ref:`parents<doxid-struct_q_panda_1_1_variational_1_1impl_1a9cd6c23efd4e542bb77b9ad85f1e9529>`;
		MatrixXd :ref:`m_prob<doxid-struct_q_panda_1_1_variational_1_1impl_1af9668071cafbb85c671d03ef55065c87>`;

		// construction
	
		:ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl_1ae616bd11074f0d644e25f20b55153de7>`(const MatrixXd&);
	
		:target:`impl<doxid-struct_q_panda_1_1_variational_1_1impl_1ad7ccd00d8500101df6fd7be1ba315a60>`(
			const MatrixXd&,
			bool isDifferentiable
			);
	
		:ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl_1a760c425eded6d5a3e8e8e53601abc914>`(:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>`, const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&);
	};

	// direct descendants

	struct :ref:`impl_qop_pmeasure<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure>`;
	struct :ref:`impl_qop_pmeasure_real_chip<doxid-struct_q_panda_1_1_variational_1_1impl__qop__pmeasure__real__chip>`;
	struct :ref:`impl_stack<doxid-struct_q_panda_1_1_variational_1_1impl__stack>`;
	struct :ref:`impl_subscript<doxid-struct_q_panda_1_1_variational_1_1impl__subscript>`;
	struct :ref:`impl_vqp<doxid-struct_q_panda_1_1_variational_1_1impl__vqp>`;
	struct :ref:`impl_vqp_real_chip<doxid-struct_q_panda_1_1_variational_1_1impl__vqp__real__chip>`;
.. _details-struct_q_panda_1_1_variational_1_1impl:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

implementation class for the var. Impl only includes classical operator with fixed number of arguments.

Fields
------

.. index:: pair: variable; val
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1a192110dfe5013d1fd808aab4f262e241:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MatrixXd val

Internal value.

.. index:: pair: variable; m_is_differentiable
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1ad7bb7cb00dd81ad05e29767d35ae2c4a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool m_is_differentiable

Placeholder/Variable.

.. index:: pair: variable; op
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1a48c4c2d47ded74e71bf3615945943e3b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` op

Operator type.

.. index:: pair: variable; children
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1ab9026462afdd43c59bfe64fff032691f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> children

Childrens. For example, c = a + b. c is a and b's parent, a and b are c's children.

.. index:: pair: variable; parents
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1a9cd6c23efd4e542bb77b9ad85f1e9529:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::weak_ptr<impl>> parents

Parents. For example, c = a + b. c is a and b's parent, a and b are c's children.

.. index:: pair: variable; m_prob
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1af9668071cafbb85c671d03ef55065c87:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MatrixXd m_prob

Internal value.

Construction
------------

.. index:: pair: function; impl
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1ae616bd11074f0d644e25f20b55153de7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	impl(const MatrixXd&)

Construct from a Eigen matrix.

.. index:: pair: function; impl
.. _doxid-struct_q_panda_1_1_variational_1_1impl_1a760c425eded6d5a3e8e8e53601abc914:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	impl(:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>`, const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&)

Construct from a operator.

