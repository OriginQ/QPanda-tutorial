.. index:: pair: struct; QPanda::StitchesInfo
.. _doxid-struct_q_panda_1_1_stitches_info:

struct QPanda::StitchesInfo
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Cutting point information Note: Each cut point corresponds to a measurement-qubit and a preparation-qubit of two sub-circuit respectively. :ref:`More...<details-struct_q_panda_1_1_stitches_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <CutQC.h>
	
	struct StitchesInfo
	{
		// typedefs
	
		typedef std::pair<uint32_t, uint32_t> :ref:`sub_cir_op_qubit_index<doxid-struct_q_panda_1_1_stitches_info_1a5b0d27762ea53e1c086a705603d88395>`;

		// fields
	
		:ref:`sub_cir_op_qubit_index<doxid-struct_q_panda_1_1_stitches_info_1a5b0d27762ea53e1c086a705603d88395>` :target:`m_meas_qubit<doxid-struct_q_panda_1_1_stitches_info_1a633e6988d1f532782dfbd13d8af58e97>`;
		:ref:`sub_cir_op_qubit_index<doxid-struct_q_panda_1_1_stitches_info_1a5b0d27762ea53e1c086a705603d88395>` :target:`m_prep_qubit<doxid-struct_q_panda_1_1_stitches_info_1a3564241e54b66e601cb9346ff4214c4c>`;
	};
.. _details-struct_q_panda_1_1_stitches_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Cutting point information Note: Each cut point corresponds to a measurement-qubit and a preparation-qubit of two sub-circuit respectively.

Typedefs
--------

.. index:: pair: typedef; sub_cir_op_qubit_index
.. _doxid-struct_q_panda_1_1_stitches_info_1a5b0d27762ea53e1c086a705603d88395:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	typedef std::pair<uint32_t, uint32_t> sub_cir_op_qubit_index

sub_circuit_index : qubit_index

