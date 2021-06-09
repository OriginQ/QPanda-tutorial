.. index:: pair: class; QPanda::DRAW_TEXT_PIC::DrawQProg
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog:

class QPanda::DRAW_TEXT_PIC::DrawQProg
======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

draw Qprog by text :ref:`More...<details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <DrawQProg.h>
	
	class DrawQProg
	{
	public:
		// construction
	
		:ref:`DrawQProg<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog_1ab68cd814402b61873a8555db992b673a>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prg,
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_start,
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_end,
			bool b_out_put_to_file = false
			);

		// methods
	
		std::string :ref:`textDraw<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog_1a2d00a58f510bdb67b953bb0b7747021d>`(:ref:`TEXT_PIC_TYPE<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1af860ad3fc4dd4a45b78c415a604e6a5b>` t, uint32_t length = 100, const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`);
	};
.. _details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

draw Qprog by text

Construction
------------

.. index:: pair: function; DrawQProg
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog_1ab68cd814402b61873a8555db992b673a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DrawQProg(
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prg,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_start,
		const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` node_itr_end,
		bool b_out_put_to_file = false
		)

Constructor of :ref:`DrawQProg <doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog>`.

Methods
-------

.. index:: pair: function; textDraw
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_q_prog_1a2d00a58f510bdb67b953bb0b7747021d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string textDraw(
		:ref:`TEXT_PIC_TYPE<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1af860ad3fc4dd4a45b78c415a604e6a5b>` t,
		uint32_t length = 100,
		const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`
		)

Draw text-picture.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- TEXT_PIC_TYPE

		- draw type

	*
		- const

		- std::string It can be configuration file or configuration data, which can be distinguished by file suffix, so the configuration file must be end with ".json", default is CONFIG_PATH



.. rubric:: Returns:

std::string the text-picture



.. rubric:: See also:

:ref:`TEXT_PIC_TYPE <doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1af860ad3fc4dd4a45b78c415a604e6a5b>`

