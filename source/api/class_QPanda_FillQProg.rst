.. index:: pair: class; QPanda::FillQProg
.. _doxid-class_q_panda_1_1_fill_q_prog:

class QPanda::FillQProg
=======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Fill quantum program by I quantum gate. :ref:`More...<details-class_q_panda_1_1_fill_q_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <FillQProg.h>
	
	class FillQProg
	{
	public:
		// construction
	
		:target:`FillQProg<doxid-class_q_panda_1_1_fill_q_prog_1a389f1d5b056e4df0c59d3f27d59d3614>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& input_prog);

		// methods
	
		void :ref:`fill_by_I<doxid-class_q_panda_1_1_fill_q_prog_1a06025fd96916cc59618b1dd9e158f7d8>`();
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& :target:`get_output_prog<doxid-class_q_panda_1_1_fill_q_prog_1a9eb544ee9e4e50004c5e723e33fe3b8d>`();
	
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`get_unused_qubits_in_layer<doxid-class_q_panda_1_1_fill_q_prog_1a609f8bd036b737538536516c3a6d0032>`(
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& all_qubits,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& inuse_qubits
			);
	};
.. _details-class_q_panda_1_1_fill_q_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Fill quantum program by I quantum gate.

Methods
-------

.. index:: pair: function; fill_by_I
.. _doxid-class_q_panda_1_1_fill_q_prog_1a06025fd96916cc59618b1dd9e158f7d8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void fill_by_I()

Fill the input :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` by I gate.

