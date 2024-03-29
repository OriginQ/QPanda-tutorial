.. index:: pair: class; QPanda::Variational::expression
.. _doxid-class_q_panda_1_1_variational_1_1expression:

class QPanda::Variational::expression
=====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

A proxy class for the :ref:`Variational::var <doxid-class_q_panda_1_1_variational_1_1var>`. :ref:`More...<details-class_q_panda_1_1_variational_1_1expression>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <expression.h>
	
	class expression
	{
	public:
		// construction
	
		:ref:`expression<doxid-class_q_panda_1_1_variational_1_1expression_1a15a5fd5ca50b4afd2c767dc9c824e67a>`(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` root);

		// methods
	
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :ref:`getRoot<doxid-class_q_panda_1_1_variational_1_1expression_1a77b062979855dbd6e0d5cea92e6d6e91>`() const;
		std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :ref:`findLeaves<doxid-class_q_panda_1_1_variational_1_1expression_1a7934f625ad6b5873f8dfd8a18a77ff3f>`();
		MatrixXd :ref:`propagate<doxid-class_q_panda_1_1_variational_1_1expression_1acd67086821d6c6ae6b995e77c136ed69>`();
		MatrixXd :ref:`propagate<doxid-class_q_panda_1_1_variational_1_1expression_1a268ed58d996f7745cdb86567347274cc>`(const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves);
		std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :ref:`findNonConsts<doxid-class_q_panda_1_1_variational_1_1expression_1a134d5be16f4aae3734105693fc25eaff>`(const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&);
		std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`findNonConsts<doxid-class_q_panda_1_1_variational_1_1expression_1a8eafcd6d5802826b2c2c02753a64c56b>`(const std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&);
		void :ref:`backpropagate<doxid-class_q_panda_1_1_variational_1_1expression_1ad48564e60cabeec8423a639a53047942>`(std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>& leaves);
	
		void :ref:`backpropagate<doxid-class_q_panda_1_1_variational_1_1expression_1a63e11664908cf2a982ec04d0cf972e67>`(
			std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>& leaves,
			const std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& nonconsts
			);
	
		std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`findVariables<doxid-class_q_panda_1_1_variational_1_1expression_1a9575963379e8e2a64c0305eddf17330b>`();
	};
.. _details-class_q_panda_1_1_variational_1_1expression:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

A proxy class for the :ref:`Variational::var <doxid-class_q_panda_1_1_variational_1_1var>`.

Construction
------------

.. index:: pair: function; expression
.. _doxid-class_q_panda_1_1_variational_1_1expression_1a15a5fd5ca50b4afd2c767dc9c824e67a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	expression(:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` root)

Construct a new expression object.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- root

		- the root variable, denoting the y in dy/dx.

Methods
-------

.. index:: pair: function; getRoot
.. _doxid-class_q_panda_1_1_variational_1_1expression_1a77b062979855dbd6e0d5cea92e6d6e91:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` getRoot() const

Get the root.



.. rubric:: Returns:

var the root, denoting the y in dy/dx.

.. index:: pair: function; findLeaves
.. _doxid-class_q_panda_1_1_variational_1_1expression_1a7934f625ad6b5873f8dfd8a18a77ff3f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> findLeaves()

recursively finding the leaves for the root



.. rubric:: Returns:

std::vector<var> the vector of the leaves

.. index:: pair: function; propagate
.. _doxid-class_q_panda_1_1_variational_1_1expression_1acd67086821d6c6ae6b995e77c136ed69:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MatrixXd propagate()

feed forward the expression, return the value



.. rubric:: Returns:

MatrixXd The result

.. index:: pair: function; propagate
.. _doxid-class_q_panda_1_1_variational_1_1expression_1a268ed58d996f7745cdb86567347274cc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MatrixXd propagate(const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves)

feed forward the expression with given leaves



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- leaves

		- leaves either generated by :ref:`expression::findLeaves <doxid-class_q_panda_1_1_variational_1_1expression_1a7934f625ad6b5873f8dfd8a18a77ff3f>` or assigned by user (usually not including the training data placeholders).



.. rubric:: Returns:

MatrixXd The reuslts.

.. index:: pair: function; findNonConsts
.. _doxid-class_q_panda_1_1_variational_1_1expression_1a134d5be16f4aae3734105693fc25eaff:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> findNonConsts(const std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>&)

find all non-constants variable for the given leaves. if there is some variable not related in the path from the root to the leaves, it will not be added into the set



.. rubric:: Returns:

std::unordered_set<var> All non-constants variables.

.. index:: pair: function; backpropagate
.. _doxid-class_q_panda_1_1_variational_1_1expression_1ad48564e60cabeec8423a639a53047942:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void backpropagate(std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>& leaves)

backpropagation and evalute all gradients.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- leaves

		- The var-grad map. This function will update the gradients.

.. index:: pair: function; backpropagate
.. _doxid-class_q_panda_1_1_variational_1_1expression_1a63e11664908cf2a982ec04d0cf972e67:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void backpropagate(
		std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd>& leaves,
		const std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& nonconsts
		)

backpropagation and evalute all gradients.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- leaves

		- The var-grad map. This function will update the gradients.

	*
		- nonconsts

		- all non-constants. using this to remove unnecessary nodes from the gradient-evaluation.

