.. index:: pair: class; QPanda::Exp
.. _doxid-class_q_panda_1_1_exp:

class QPanda::Exp
=================

.. toctree::
	:hidden:

	enum_QPanda_Exp_ContentType.rst
	struct_QPanda_Exp_Content.rst

Overview
~~~~~~~~

Saves the expression containing the variable. :ref:`More...<details-class_q_panda_1_1_exp>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QASMToQProg.h>
	
	class Exp
	{
	public:
		// enums
	
		enum :ref:`ContentType<doxid-class_q_panda_1_1_exp_1a81af5e3c83ca9c23d03436dbd3c66c3f>`;

		// structs
	
		struct :ref:`Content<doxid-struct_q_panda_1_1_exp_1_1_content>`;

		// construction
	
		:target:`Exp<doxid-class_q_panda_1_1_exp_1a37e07af58e990abfb411e8313b8fa3b0>`(std::string name);
	
		:target:`Exp<doxid-class_q_panda_1_1_exp_1a35a47c26b6d9872598c93236378b8b85>`(
			std::shared_ptr<Exp> left_exp_ptr,
			std::shared_ptr<Exp> right_exp_ptr,
			std::string op
			);
	
		:target:`Exp<doxid-class_q_panda_1_1_exp_1a5431d94ff261106e64335992dcdecd73>`(double val);

		// methods
	
		std::shared_ptr<Exp> :ref:`clone<doxid-class_q_panda_1_1_exp_1ab1523308d9cc8e39de0d7ea7450c8660>`();
		void :target:`set_formal_actual_var_map<doxid-class_q_panda_1_1_exp_1a1942564c13c2215356699cd0a42e1d46>`(std::map<std::string, double> name_val_map);
		double :ref:`eval<doxid-class_q_panda_1_1_exp_1a557f54032493ad2672a83fa19e0efe8c>`();
	};
.. _details-class_q_panda_1_1_exp:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Saves the expression containing the variable.

Methods
-------

.. index:: pair: function; clone
.. _doxid-class_q_panda_1_1_exp_1ab1523308d9cc8e39de0d7ea7450c8660:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::shared_ptr<Exp> clone()

clone :ref:`Exp <doxid-class_q_panda_1_1_exp>` class



.. rubric:: Returns:

std::shared_ptr<Exp> :ref:`Exp <doxid-class_q_panda_1_1_exp>` class shared ptr

.. index:: pair: function; eval
.. _doxid-class_q_panda_1_1_exp_1a557f54032493ad2672a83fa19e0efe8c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	double eval()

evaluation



.. rubric:: Returns:

double operation rusult

