.. index:: pair: class; QPanda::DRAW_TEXT_PIC::DrawPicture
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture:

class QPanda::DRAW_TEXT_PIC::DrawPicture
========================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

draw text-picture :ref:`More...<details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Draw.h>
	
	class DrawPicture
	{
	public:
		// construction
	
		:ref:`DrawPicture<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1af21c84c92e54188799d2211094907629>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& layer_info, uint32_t length);

		// methods
	
		void :ref:`init<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a0a89097378af40dcd7ace988a04dae69>`(std::vector<int>& quBits, std::vector<int>& clBits);
		std::string :ref:`present<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a0fe68cb5e4305330fdb8740682f25646>`(bool b_out_put_to_file = false);
		void :ref:`mergeLine<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1af872b849c0703a9c07c93bf9f4257ad3>`();
		int :ref:`getMaxQuWireLength<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a71777dc9fc8632d641cc9d11aef40e9a>`(WireIter start_quBit_wire, WireIter end_quBit_wire);
		void :ref:`updateTextPicLen<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a04d36b99f2830ca880df8f48b71eeea2>`();
		unsigned long :ref:`getWideCharVal<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a2e64d6acaf8cc30ec089d1f992088d9f>`(const unsigned char* wide_char);
		void :ref:`check_time_sequence<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a48d5f0eee00668f5829d859432b7b2c2>`(:ref:`TopoSeqIter<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1ab5bad57f33815f2553766b34d9417028>` cur_layer_iter);
		void :ref:`update_time_sequence<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1ace00d8e6a8632601086789d6bfbb59b5>`(:ref:`Wire::sRef<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aa0c18d4de553840230509b7b49569936>`& p_wire, int increased_time_sequence);
		void :ref:`append_time_sequence_line<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a8003d35d8d8cd09337e2170ca938de7a>`();
		void :ref:`append_layer_line<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1ad169e72f0ce2aafac0630fa490576547>`();
		void :ref:`draw_by_layer<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a3b5fecaeb451504ed0411d35742244c4>`();
		void :ref:`draw_by_time_sequence<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1aec38d5e547c04386ea8316df39d1e282>`(const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`);
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`get_qvec_difference<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1ac79e3b13ce0b56e30fa7489f97f62889>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec1, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec2);
	};
.. _details-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

draw text-picture

Construction
------------

.. index:: pair: function; DrawPicture
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1af21c84c92e54188799d2211094907629:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	DrawPicture(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` prog, :ref:`LayeredTopoSeq<doxid-namespace_q_panda_1a3e8842707fdef1b305507d101f359626>`& layer_info, uint32_t length)

Constructor of :ref:`DrawPicture <doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture>`.

Methods
-------

.. index:: pair: function; init
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a0a89097378af40dcd7ace988a04dae69:

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
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a0fe68cb5e4305330fdb8740682f25646:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string present(bool b_out_put_to_file = false)

display and return the target string



.. rubric:: Returns:

std::string

.. index:: pair: function; mergeLine
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1af872b849c0703a9c07c93bf9f4257ad3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void mergeLine()

merge wire line

.. index:: pair: function; getMaxQuWireLength
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a71777dc9fc8632d641cc9d11aef40e9a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int getMaxQuWireLength(WireIter start_quBit_wire, WireIter end_quBit_wire)

get the max length of quantum wire between start_quBit_wire and end_quBit_wire



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- WireIter

		- start quBit wire

	*
		- WireIter

		- end quBit wire



.. rubric:: Returns:

int the max length

.. index:: pair: function; updateTextPicLen
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a04d36b99f2830ca880df8f48b71eeea2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void updateTextPicLen()

update TextPic length

.. index:: pair: function; getWideCharVal
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a2e64d6acaf8cc30ec089d1f992088d9f:

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
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a48d5f0eee00668f5829d859432b7b2c2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void check_time_sequence(:ref:`TopoSeqIter<doxid-namespace_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1ab5bad57f33815f2553766b34d9417028>` cur_layer_iter)

check the target wire time sequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- TopoSeqIter

		- the target layer

.. index:: pair: function; update_time_sequence
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1ace00d8e6a8632601086789d6bfbb59b5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void update_time_sequence(:ref:`Wire::sRef<doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_wire_1aa0c18d4de553840230509b7b49569936>`& p_wire, int increased_time_sequence)

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
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a8003d35d8d8cd09337e2170ca938de7a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void append_time_sequence_line()

append time sequence line to text-picture

.. index:: pair: function; append_layer_line
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1ad169e72f0ce2aafac0630fa490576547:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void append_layer_line()

append layer line to text-picture

.. index:: pair: function; draw_by_layer
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1a3b5fecaeb451504ed0411d35742244c4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void draw_by_layer()

draw text-picture by layer

.. index:: pair: function; draw_by_time_sequence
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1aec38d5e547c04386ea8316df39d1e282:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void draw_by_time_sequence(const std::string config_data = :ref:`CONFIG_PATH<doxid-_json_config_param_8h_1a863ab5d791c86f9dfff4c6e90624130c>`)

draw text-picture by time sequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- std::string It can be configuration file or configuration data, which can be distinguished by file suffix, so the configuration file must be end with ".json", default is CONFIG_PATH

.. index:: pair: function; get_qvec_difference
.. _doxid-class_q_panda_1_1_d_r_a_w___t_e_x_t___p_i_c_1_1_draw_picture_1ac79e3b13ce0b56e30fa7489f97f62889:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` get_qvec_difference(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec1, :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& vec2)

get the difference of two QVecs



.. rubric:: Returns:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>` vec1 - vec2

