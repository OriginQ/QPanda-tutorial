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
	
		:target:`QProgToMatrix<doxid-class_q_panda_1_1_q_prog_to_matrix_1ae9675d858e62b1831c0e3e8de4aef663>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& p);

		// methods
	
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getMatrix<doxid-class_q_panda_1_1_q_prog_to_matrix_1a1ec162342ed91267c42d150208976d6e>`();
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getMatrixOfOneLayer<doxid-class_q_panda_1_1_q_prog_to_matrix_1a1dd83201e3ccd64a87d510dbc7c15650>`(:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`& layer, const :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& prog_dag);
	};
.. _details-class_q_panda_1_1_q_prog_to_matrix:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

get the matrix of a :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

Methods
-------

.. index:: pair: function; getMatrix
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1a1ec162342ed91267c42d150208976d6e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getMatrix()

calc the matrix of the input :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`



.. rubric:: Returns:

QStat the matrix of the input :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

.. index:: pair: function; getMatrixOfOneLayer
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1a1dd83201e3ccd64a87d510dbc7c15650:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getMatrixOfOneLayer(:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`& layer, const :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& prog_dag)

calc the matrix of nodes in one layer



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- SequenceLayer&

		- layer nodes

	*
		- QProgDAG&

		- DAG algorithm object



.. rubric:: Returns:

QStat the matrix of the layer

