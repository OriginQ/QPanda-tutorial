.. index:: pair: class; QPanda::DRAW_TEXT_PIC::Wire
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire:

class QPanda::DRAW_TEXT_PIC::Wire
=================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

the wire of text-picture :ref:`More...<details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class Wire
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<Wire> :target:`sRef<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aa0c18d4de553840230509b7b49569936>`;

		// construction
	
		:ref:`Wire<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a0a56cc95c580d7f9cd938b62f4f83e3c>`(const std::string& connect_str);

		// methods
	
		virtual void :ref:`setName<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a8b1cc51df94b4ebe5a5e4692854a54d3>`(const std::string& name, size_t nameLen);
		virtual int :ref:`append<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aea4e6f0775daa49c22ba7168644c9435>`(const :ref:`DrawBox<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box>`& box, const int box_pos);
		virtual int :ref:`getWireLength<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a1344cc405f0c6cc38ef080feb130c738>`();
		virtual std::string :ref:`draw<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a5c20aa509fa55b6e110d146599466ee9>`();
		virtual void :ref:`updateWireLen<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a7b92a77ef5826e20a5d8b7f86de63ef7>`(const int len);
		virtual void :ref:`setMergedFlag<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a10f260b03f96d010e1496b1f35a99e65>`(bool b);
		virtual const std::string& :ref:`getTopLine<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aa0eaa05daa27d39edd52954d130982da>`() const;
		virtual const std::string& :ref:`getMidLine<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aeae435602b2cfbd339f09b36c8e810d4>`() const;
		virtual const std::string& :ref:`getBotLine<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1ab9955e1aff28776c91a1805d2177f80d>`() const;
		int :ref:`update_time_sequence<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a0e9e978227649b35a70a3d42ec90e77b>`(unsigned int increase_time_sequence);
		int :ref:`get_time_sequence<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1ac2d7b639cee1ecf7cfccf3355e501204>`();
	};
.. _details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

the wire of text-picture

Construction
------------

.. index:: pair: function; Wire
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a0a56cc95c580d7f9cd938b62f4f83e3c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Wire(const std::string& connect_str)

Constructor of :ref:`DrawBox <doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box>`.

Methods
-------

.. index:: pair: function; setName
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a8b1cc51df94b4ebe5a5e4692854a54d3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setName(const std::string& name, size_t nameLen)

set the name of wire



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- name

	*
		- size_t

		- name length

.. index:: pair: function; append
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aea4e6f0775daa49c22ba7168644c9435:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int append(const :ref:`DrawBox<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_box>`& box, const int box_pos)

append a box to current wire



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- DrawBox&

		- box

	*
		- int

		- append postion



.. rubric:: Returns:

int the length of current wire

.. index:: pair: function; getWireLength
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a1344cc405f0c6cc38ef080feb130c738:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int getWireLength()

get the length of current wire



.. rubric:: Returns:

int the length of current wire

.. index:: pair: function; draw
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a5c20aa509fa55b6e110d146599466ee9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string draw()

conver current wire to string and save to file



.. rubric:: Returns:

std::string

.. index:: pair: function; updateWireLen
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a7b92a77ef5826e20a5d8b7f86de63ef7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void updateWireLen(const int len)

update current wire length



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- the new length

.. index:: pair: function; setMergedFlag
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a10f260b03f96d010e1496b1f35a99e65:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void setMergedFlag(bool b)

set whether to merge wire



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool

		-

.. index:: pair: function; getTopLine
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aa0eaa05daa27d39edd52954d130982da:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getTopLine() const

get top line string



.. rubric:: Returns:

std::string

.. index:: pair: function; getMidLine
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aeae435602b2cfbd339f09b36c8e810d4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getMidLine() const

get middle line string



.. rubric:: Returns:

std::string

.. index:: pair: function; getBotLine
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1ab9955e1aff28776c91a1805d2177f80d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getBotLine() const

get bottom line string



.. rubric:: Returns:

std::string

.. index:: pair: function; update_time_sequence
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1a0e9e978227649b35a70a3d42ec90e77b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int update_time_sequence(unsigned int increase_time_sequence)

update current wire time sequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- the increased time sequence

.. index:: pair: function; get_time_sequence
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1ac2d7b639cee1ecf7cfccf3355e501204:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int get_time_sequence()

get current wire time sequence



.. rubric:: Returns:

int

