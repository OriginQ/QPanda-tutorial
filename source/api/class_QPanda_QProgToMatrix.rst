.. index:: pair: class; QPanda::QProgToMatrix
.. _doxid-class_q_panda_1_1_q_prog_to_matrix:

class QPanda::QProgToMatrix
===========================

.. toctree::
	:hidden:

	class_QPanda_QProgToMatrix_MatrixOfOneLayer.rst

Overview
~~~~~~~~

get the matrix of a :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` :ref:`More...<details-class_q_panda_1_1_q_prog_to_matrix>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgToMatrix.h>
	
	class QProgToMatrix
	{
	public:
		// classes
	
		class :ref:`MatrixOfOneLayer<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer>`;

		// construction
	
		:target:`QProgToMatrix<doxid-class_q_panda_1_1_q_prog_to_matrix_1a18e30e54d2b88ee1889fa86c838bb32d>`(
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& p,
			const bool b_bid_endian = false
			);

		// methods
	
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`get_matrix<doxid-class_q_panda_1_1_q_prog_to_matrix_1abd6c4f9d1d6207a0ed7e7f11049960ee>`();
		:ref:`qmatrix_t<doxid-namespace_q_panda_1ae5390d4fcde76d93c817482cf46708f3>` :ref:`get_matrix_of_one_layer<doxid-class_q_panda_1_1_q_prog_to_matrix_1aef6cee69d1e51b0155bc6a2e8c5a0c96>`(:ref:`SeqLayer<doxid-namespace_q_panda_1a6ed9ed67bc56f43d141fc68fec4c6231>`<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>& layer);
	};
.. _details-class_q_panda_1_1_q_prog_to_matrix:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

get the matrix of a :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

Methods
-------

.. index:: pair: function; get_matrix
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1abd6c4f9d1d6207a0ed7e7f11049960ee:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` get_matrix()

calc the matrix of the input :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`



.. rubric:: Returns:

QStat the matrix of the input :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

.. index:: pair: function; get_matrix_of_one_layer
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1aef6cee69d1e51b0155bc6a2e8c5a0c96:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`qmatrix_t<doxid-namespace_q_panda_1ae5390d4fcde76d93c817482cf46708f3>` get_matrix_of_one_layer(:ref:`SeqLayer<doxid-namespace_q_panda_1a6ed9ed67bc56f43d141fc68fec4c6231>`<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>& layer)

calc the matrix of nodes in one layer



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- SeqLayer<pOptimizerNodeInfo>&

		- layer nodes

	*
		- QProgDAG&

		- DAG algorithm object



.. rubric:: Returns:

qmatrix_t the matrix of the layer

