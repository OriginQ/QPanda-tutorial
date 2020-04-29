.. index:: pair: class; QPanda::DrawBox
.. _doxid-class_q_panda_1_1_draw_box:

class QPanda::DrawBox
=====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Draw text-picture box. :ref:`More...<details-class_q_panda_1_1_draw_box>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class DrawBox
	{
	public:
		// construction
	
		:ref:`DrawBox<doxid-class_q_panda_1_1_draw_box_1a8475d5865295e1cd8195bd42916e607a>`(
			const std::string& top_format_str,
			const std::string& mid_format_str,
			const std::string& bot_format_str
			);

		// methods
	
		virtual const std::string& :ref:`getTopStr<doxid-class_q_panda_1_1_draw_box_1ac3bc3ed1cfa1c380ead737a99b61c99d>`() const;
		virtual const std::string& :ref:`getMidStr<doxid-class_q_panda_1_1_draw_box_1ab7a783202664ad21d5c87bc9ff3d6e20>`() const;
		virtual const std::string& :ref:`getBotStr<doxid-class_q_panda_1_1_draw_box_1a49ba43467de70888886b63fe69da27c8>`() const;
		virtual void :ref:`set_top_connected<doxid-class_q_panda_1_1_draw_box_1ad320944b1f8a6fbcf38c8af0c994678b>`();
		virtual void :ref:`set_bot_connected<doxid-class_q_panda_1_1_draw_box_1a2efeff02b250dcddd49575871bd27141>`();
		virtual int :ref:`getLen<doxid-class_q_panda_1_1_draw_box_1afec8ad14d82b3b3a4911fd4922dad41f>`() const = 0;
	};
.. _details-class_q_panda_1_1_draw_box:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Draw text-picture box.

Construction
------------

.. index:: pair: function; DrawBox
.. _doxid-class_q_panda_1_1_draw_box_1a8475d5865295e1cd8195bd42916e607a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DrawBox(
		const std::string& top_format_str,
		const std::string& mid_format_str,
		const std::string& bot_format_str
		)

Constructor of :ref:`DrawBox <doxid-class_q_panda_1_1_draw_box>`.

Methods
-------

.. index:: pair: function; getTopStr
.. _doxid-class_q_panda_1_1_draw_box_1ac3bc3ed1cfa1c380ead737a99b61c99d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getTopStr() const

get top string of box

.. index:: pair: function; getMidStr
.. _doxid-class_q_panda_1_1_draw_box_1ab7a783202664ad21d5c87bc9ff3d6e20:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getMidStr() const

get middle string of box

.. index:: pair: function; getBotStr
.. _doxid-class_q_panda_1_1_draw_box_1a49ba43467de70888886b63fe69da27c8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual const std::string& getBotStr() const

get bottom string of box

.. index:: pair: function; set_top_connected
.. _doxid-class_q_panda_1_1_draw_box_1ad320944b1f8a6fbcf38c8af0c994678b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_top_connected()

set connected str on the top of box

.. index:: pair: function; set_bot_connected
.. _doxid-class_q_panda_1_1_draw_box_1a2efeff02b250dcddd49575871bd27141:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void set_bot_connected()

set connected str on the bottom of box

.. index:: pair: function; getLen
.. _doxid-class_q_panda_1_1_draw_box_1afec8ad14d82b3b3a4911fd4922dad41f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual int getLen() const = 0

get box len



.. rubric:: Returns:

int the length of box

