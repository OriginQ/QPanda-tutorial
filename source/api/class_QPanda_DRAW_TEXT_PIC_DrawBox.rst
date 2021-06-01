.. index:: pair: class; QPanda::DRAW_TEXT_PIC::DrawBox
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box:

class QPanda::DRAW_TEXT_PIC::DrawBox
====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Draw text-picture box. :ref:`More...<details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class DrawBox
	{
	public:
		// construction
	
		:ref:`DrawBox<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1ae4aae07a87097cf2067b25f33e0ef807>`(
			const std::string& top_format_str,
			const std::string& mid_format_str,
			const std::string& bot_format_str
			);

		// methods
	
		virtual const std::string& :ref:`getTopStr<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a5b8b7bf5182df88b809183725a9a7617>`() const;
		virtual const std::string& :ref:`getMidStr<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a86abdc9ad3b3b9523d321024c124b445>`() const;
		virtual const std::string& :ref:`getBotStr<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1ae229a00d8f0b4e06513f2da98fcbf560>`() const;
		virtual void :ref:`set_top_connected<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a17b16501c47c715881a2616868185835>`();
		virtual void :ref:`set_bot_connected<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a78814ca9ee4afa30b1b0f375c7222f42>`();
		virtual int :ref:`getLen<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1ae14a340431dc3128a9bb48ffba3c0265>`() const = 0;
	};
.. _details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Draw text-picture box.

Construction
------------

.. index:: pair: function; DrawBox
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1ae4aae07a87097cf2067b25f33e0ef807:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DrawBox(
		const std::string& top_format_str,
		const std::string& mid_format_str,
		const std::string& bot_format_str
		)

Constructor of :ref:`DrawBox <doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box>`.

Methods
-------

.. index:: pair: function; getTopStr
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a5b8b7bf5182df88b809183725a9a7617:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getTopStr() const

get top string of box

.. index:: pair: function; getMidStr
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a86abdc9ad3b3b9523d321024c124b445:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getMidStr() const

get middle string of box

.. index:: pair: function; getBotStr
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1ae229a00d8f0b4e06513f2da98fcbf560:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getBotStr() const

get bottom string of box

.. index:: pair: function; set_top_connected
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a17b16501c47c715881a2616868185835:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_top_connected()

set connected str on the top of box

.. index:: pair: function; set_bot_connected
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1a78814ca9ee4afa30b1b0f375c7222f42:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_bot_connected()

set connected str on the bottom of box

.. index:: pair: function; getLen
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box_1ae14a340431dc3128a9bb48ffba3c0265:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int getLen() const = 0

get box len



.. rubric:: Returns:

int the length of box

