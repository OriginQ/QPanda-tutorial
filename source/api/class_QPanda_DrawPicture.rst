.. index:: pair: class; QPanda::DrawPicture
.. _doxid-class_q_panda_1_1_draw_picture:

class QPanda::DrawPicture
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

draw text-picture :ref:`More...<details-class_q_panda_1_1_draw_picture>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class DrawPicture
	{
	public:
		// construction
	
		:ref:`DrawPicture<doxid-class_q_panda_1_1_draw_picture_1a46f097741d596fec61b7db223a958644>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);

		// methods
	
		void :ref:`init<doxid-class_q_panda_1_1_draw_picture_1ab7b9a8952bbb75b801b8e92823c7d8fc>`(std::vector<int>& quBits, std::vector<int>& clBits);
		std::string :ref:`present<doxid-class_q_panda_1_1_draw_picture_1a5cf9614735cdfec4754de4faf71bb94f>`();
		void :ref:`mergeLine<doxid-class_q_panda_1_1_draw_picture_1af086e0d7e7bac8ea8de2366d3fe5b66c>`();
		int :ref:`getMaxQuWireLength<doxid-class_q_panda_1_1_draw_picture_1acba1930240c8d3d44a2f78953e58e1db>`(wireIter start_quBit_wire, wireIter end_quBit_wire);
		void :ref:`updateTextPicLen<doxid-class_q_panda_1_1_draw_picture_1ac0d5aca7342ea7bdeb043406195ba1c6>`();
		unsigned long :ref:`getWideCharVal<doxid-class_q_panda_1_1_draw_picture_1a87d22079efba4a6acb755680ce5c57f0>`(const unsigned char* wide_char);
		void :ref:`check_time_sequence<doxid-class_q_panda_1_1_draw_picture_1a60b15ff804f8382050d8ab5971758f37>`(std::vector<:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`>::iterator cur_layer_iter);
		void :ref:`update_time_sequence<doxid-class_q_panda_1_1_draw_picture_1a9d5b8a9a23c4347f6251e836f8bb12bd>`(std::shared_ptr<:ref:`Wire<doxid-class_q_panda_1_1_wire>`> p_wire, int increased_time_sequence);
		void :ref:`append_time_sequence_line<doxid-class_q_panda_1_1_draw_picture_1a62e7c8effe11c3b53d65852f0c793576>`();
		void :ref:`append_layer_line<doxid-class_q_panda_1_1_draw_picture_1a9c2d9c105981939ad5ffa5c1014a2793>`();
		void :ref:`draw_by_layer<doxid-class_q_panda_1_1_draw_picture_1a5f6f51f09dbdba6acdafbcc9e07c07bc>`();
		void :ref:`draw_by_time_sequence<doxid-class_q_panda_1_1_draw_picture_1a8f47af5a20ab208210551cc4d0326498>`();
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`get_qvec_difference<doxid-class_q_panda_1_1_draw_picture_1a06f85ab11f40cc876f31359652d153ae>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec1, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec2);
	};
.. _details-class_q_panda_1_1_draw_picture:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

draw text-picture

Construction
------------

.. index:: pair: function; DrawPicture
.. _doxid-class_q_panda_1_1_draw_picture_1a46f097741d596fec61b7db223a958644:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DrawPicture(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

Constructor of :ref:`DrawPicture <doxid-class_q_panda_1_1_draw_picture>`.

Methods
-------

.. index:: pair: function; init
.. _doxid-class_q_panda_1_1_draw_picture_1ab7b9a8952bbb75b801b8e92823c7d8fc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void init(std::vector<int>& quBits, std::vector<int>& clBits)

initialize



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<int>&

		- used qubits

	*
		- std::vector<int>&

		- used class bits

.. index:: pair: function; present
.. _doxid-class_q_panda_1_1_draw_picture_1a5cf9614735cdfec4754de4faf71bb94f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string present()

display and return the target string



.. rubric:: Returns:

std::string

.. index:: pair: function; mergeLine
.. _doxid-class_q_panda_1_1_draw_picture_1af086e0d7e7bac8ea8de2366d3fe5b66c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void mergeLine()

merge wire line

.. index:: pair: function; getMaxQuWireLength
.. _doxid-class_q_panda_1_1_draw_picture_1acba1930240c8d3d44a2f78953e58e1db:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int getMaxQuWireLength(wireIter start_quBit_wire, wireIter end_quBit_wire)

get the max length of quantum wire between start_quBit_wire and end_quBit_wire



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- wireIter

		- start quBit wire

	*
		- wireIter

		- end quBit wire



.. rubric:: Returns:

int the max length

.. index:: pair: function; updateTextPicLen
.. _doxid-class_q_panda_1_1_draw_picture_1ac0d5aca7342ea7bdeb043406195ba1c6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void updateTextPicLen()

update TextPic length

.. index:: pair: function; getWideCharVal
.. _doxid-class_q_panda_1_1_draw_picture_1a87d22079efba4a6acb755680ce5c57f0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	unsigned long getWideCharVal(const unsigned char* wide_char)

get val of wide char



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- unsigned char\*

		- the target wide char



.. rubric:: Returns:

the val of the wide char

.. index:: pair: function; check_time_sequence
.. _doxid-class_q_panda_1_1_draw_picture_1a60b15ff804f8382050d8ab5971758f37:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void check_time_sequence(std::vector<:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`>::iterator cur_layer_iter)

check the target wire time sequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<SequenceLayer>::iterator

		- the target wire

.. index:: pair: function; update_time_sequence
.. _doxid-class_q_panda_1_1_draw_picture_1a9d5b8a9a23c4347f6251e836f8bb12bd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void update_time_sequence(std::shared_ptr<:ref:`Wire<doxid-class_q_panda_1_1_wire>`> p_wire, int increased_time_sequence)

update the target wire time sequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::shared_ptr<Wire>

		- the target wire

	*
		- int

		- increased time sequence

.. index:: pair: function; append_time_sequence_line
.. _doxid-class_q_panda_1_1_draw_picture_1a62e7c8effe11c3b53d65852f0c793576:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void append_time_sequence_line()

append time sequence line to text-picture

.. index:: pair: function; append_layer_line
.. _doxid-class_q_panda_1_1_draw_picture_1a9c2d9c105981939ad5ffa5c1014a2793:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void append_layer_line()

append layer line to text-picture

.. index:: pair: function; draw_by_layer
.. _doxid-class_q_panda_1_1_draw_picture_1a5f6f51f09dbdba6acdafbcc9e07c07bc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void draw_by_layer()

draw text-picture by layer

.. index:: pair: function; draw_by_time_sequence
.. _doxid-class_q_panda_1_1_draw_picture_1a8f47af5a20ab208210551cc4d0326498:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void draw_by_time_sequence()

draw text-picture by time sequence

.. index:: pair: function; get_qvec_difference
.. _doxid-class_q_panda_1_1_draw_picture_1a06f85ab11f40cc876f31359652d153ae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` get_qvec_difference(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec1, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec2)

get the difference of two QVecs



.. rubric:: Returns:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>` vec1 - vec2

