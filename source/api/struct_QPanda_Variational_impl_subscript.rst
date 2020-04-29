.. index:: pair: struct; QPanda::Variational::impl_subscript
.. _doxid-struct_q_panda_1_1_variational_1_1impl__subscript:

struct QPanda::Variational::impl_subscript
==========================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

implementation for the subscript operation. :ref:`More...<details-struct_q_panda_1_1_variational_1_1impl__subscript>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	struct impl_subscript: public :ref:`QPanda::Variational::impl<doxid-struct_q_panda_1_1_variational_1_1impl>`
	{
		// fields
	
		int :ref:`m_subscript<doxid-struct_q_panda_1_1_variational_1_1impl__subscript_1ad6e8858835041f0531becd251d49e08f>`;

		// construction
	
		:ref:`impl_subscript<doxid-struct_q_panda_1_1_variational_1_1impl__subscript_1a8e826963dd1b6f31d8154f90e7fa34b2>`(int subscript, const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&);
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

.. _details-struct_q_panda_1_1_variational_1_1impl__subscript:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

implementation for the subscript operation.

Fields
------

.. index:: pair: variable; m_subscript
.. _doxid-struct_q_panda_1_1_variational_1_1impl__subscript_1ad6e8858835041f0531becd251d49e08f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int m_subscript

the subscript

Construction
------------

.. index:: pair: function; impl_subscript
.. _doxid-struct_q_panda_1_1_variational_1_1impl__subscript_1a8e826963dd1b6f31d8154f90e7fa34b2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	impl_subscript(int subscript, const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&)

Construct a new impl subscript object by child and the subscript. c = a[i], subscript=i, a=children and c=parent.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- subscript

		- the subscript.

