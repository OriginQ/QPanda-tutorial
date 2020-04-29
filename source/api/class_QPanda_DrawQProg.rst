.. index:: pair: class; QPanda::DrawQProg
.. _doxid-class_q_panda_1_1_draw_q_prog:

class QPanda::DrawQProg
=======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

draw Qprog by text :ref:`More...<details-class_q_panda_1_1_draw_q_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <DrawQProg.h>
	
	class DrawQProg
	{
	public:
		// construction
	
		:ref:`DrawQProg<doxid-class_q_panda_1_1_draw_q_prog_1aad262761b3fd61b53bbd73134d378f66>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prg, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_start, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_end);

		// methods
	
		std::string :ref:`textDraw<doxid-class_q_panda_1_1_draw_q_prog_1a3e5faf8720eeeef91d1b2d5e9e797fbe>`(:ref:`TEXT_PIC_TYPE<doxid-namespace_q_panda_1afc58110f73ad7ce75b10a2030ff338b8>` t);
	};
.. _details-class_q_panda_1_1_draw_q_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

draw Qprog by text

Construction
------------

.. index:: pair: function; DrawQProg
.. _doxid-class_q_panda_1_1_draw_q_prog_1aad262761b3fd61b53bbd73134d378f66:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DrawQProg(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prg, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_start, const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_end)

Constructor of :ref:`DrawQProg <doxid-class_q_panda_1_1_draw_q_prog>`.

Methods
-------

.. index:: pair: function; textDraw
.. _doxid-class_q_panda_1_1_draw_q_prog_1a3e5faf8720eeeef91d1b2d5e9e797fbe:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string textDraw(:ref:`TEXT_PIC_TYPE<doxid-namespace_q_panda_1afc58110f73ad7ce75b10a2030ff338b8>` t)

Draw text-picture.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- TEXT_PIC_TYPE

		- draw type



.. rubric:: Returns:

std::string the text-picture



.. rubric:: See also:

:ref:`TEXT_PIC_TYPE <doxid-namespace_q_panda_1afc58110f73ad7ce75b10a2030ff338b8>`

