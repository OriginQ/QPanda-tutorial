.. index:: pair: class; QPanda::Wire
.. _doxid-class_q_panda_1_1_wire:

class QPanda::Wire
==================

.. toctree::
	:hidden:

Overview
~~~~~~~~

the wire of text-picture :ref:`More...<details-class_q_panda_1_1_wire>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class Wire
	{
	public:
		// construction
	
		:ref:`Wire<doxid-class_q_panda_1_1_wire_1aaa4c6a6fcb11dd68386bfae0823765a0>`(const std::string& connect_str);

		// methods
	
		virtual void :ref:`setName<doxid-class_q_panda_1_1_wire_1a13f3a84b84a2fb8c639731272afb0a34>`(const std::string& name, size_t nameLen);
		virtual int :ref:`append<doxid-class_q_panda_1_1_wire_1a6b515ce93f4bc05ed72d58594244fb27>`(const :ref:`DrawBox<doxid-class_q_panda_1_1_draw_box>`& box, const int box_pos);
		virtual int :ref:`getWireLength<doxid-class_q_panda_1_1_wire_1ac0a7c0e687df4d77b89cfedf9d6ced75>`();
		virtual std::string :ref:`draw<doxid-class_q_panda_1_1_wire_1a3f9b585ecf8031c39158cf198c62ba34>`(std::ofstream& fd, int srartRow);
		virtual void :ref:`updateWireLen<doxid-class_q_panda_1_1_wire_1a8a0fa829144b1cc4667db3ecb42a03c2>`(const int len);
		virtual void :ref:`setMergedFlag<doxid-class_q_panda_1_1_wire_1aaf7c076dc8ebef0cae1da52b66091066>`(bool b);
		virtual const std::string& :ref:`getTopLine<doxid-class_q_panda_1_1_wire_1a6abfdfff4fe9277c1f54de72dcffce88>`() const;
		virtual const std::string& :ref:`getMidLine<doxid-class_q_panda_1_1_wire_1a4c25f04fa77b7cd52bf3ab36605b0939>`() const;
		virtual const std::string& :ref:`getBotLine<doxid-class_q_panda_1_1_wire_1a02f5828993ff953416924828b4298bec>`() const;
		int :ref:`update_time_sequence<doxid-class_q_panda_1_1_wire_1a22409c3f235ad233f68a22341a3b2810>`(unsigned int increase_time_sequence);
		int :ref:`get_time_sequence<doxid-class_q_panda_1_1_wire_1a3943547330f2c7d9c4aabd128728824a>`();
	};
.. _details-class_q_panda_1_1_wire:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

the wire of text-picture

Construction
------------

.. index:: pair: function; Wire
.. _doxid-class_q_panda_1_1_wire_1aaa4c6a6fcb11dd68386bfae0823765a0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Wire(const std::string& connect_str)

Constructor of :ref:`DrawBox <doxid-class_q_panda_1_1_draw_box>`.

Methods
-------

.. index:: pair: function; setName
.. _doxid-class_q_panda_1_1_wire_1a13f3a84b84a2fb8c639731272afb0a34:

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
.. _doxid-class_q_panda_1_1_wire_1a6b515ce93f4bc05ed72d58594244fb27:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int append(const :ref:`DrawBox<doxid-class_q_panda_1_1_draw_box>`& box, const int box_pos)

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
.. _doxid-class_q_panda_1_1_wire_1ac0a7c0e687df4d77b89cfedf9d6ced75:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int getWireLength()

get the length of current wire



.. rubric:: Returns:

int the length of current wire

.. index:: pair: function; draw
.. _doxid-class_q_panda_1_1_wire_1a3f9b585ecf8031c39158cf198c62ba34:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual std::string draw(std::ofstream& fd, int srartRow)

conver current wire to string and save to file



.. rubric:: Returns:

std::string

.. index:: pair: function; updateWireLen
.. _doxid-class_q_panda_1_1_wire_1a8a0fa829144b1cc4667db3ecb42a03c2:

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
.. _doxid-class_q_panda_1_1_wire_1aaf7c076dc8ebef0cae1da52b66091066:

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
.. _doxid-class_q_panda_1_1_wire_1a6abfdfff4fe9277c1f54de72dcffce88:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getTopLine() const

get top line string



.. rubric:: Returns:

std::string

.. index:: pair: function; getMidLine
.. _doxid-class_q_panda_1_1_wire_1a4c25f04fa77b7cd52bf3ab36605b0939:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getMidLine() const

get middle line string



.. rubric:: Returns:

std::string

.. index:: pair: function; getBotLine
.. _doxid-class_q_panda_1_1_wire_1a02f5828993ff953416924828b4298bec:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getBotLine() const

get bottom line string



.. rubric:: Returns:

std::string

.. index:: pair: function; update_time_sequence
.. _doxid-class_q_panda_1_1_wire_1a22409c3f235ad233f68a22341a3b2810:

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
.. _doxid-class_q_panda_1_1_wire_1a3943547330f2c7d9c4aabd128728824a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int get_time_sequence()

get current wire time sequence



.. rubric:: Returns:

int

