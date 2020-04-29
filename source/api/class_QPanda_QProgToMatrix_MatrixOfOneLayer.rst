.. index:: pair: class; QPanda::QProgToMatrix::MatrixOfOneLayer
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer:

class QPanda::QProgToMatrix::MatrixOfOneLayer
=============================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	class MatrixOfOneLayer
	{
	public:
		// fields
	
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`m_current_layer_mat<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a754853fd981ab9ac37e9f86d31faaf7b>`;
		gateQubitInfo_t :ref:`m_double_qubit_gates<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1afa13502053f0bbf9ef9d8961817c30fc>`;
		gateQubitInfo_t :ref:`m_single_qubit_gates<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a4d2216e0ea5ad7c4882522b8654055c3>`;
		gateQubitInfo_t :ref:`m_controled_gates<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a7f1abb15d6254db8b51b98e8402902eb>`;
		calcUnitVec_t :target:`m_calc_unit_vec<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a1549d46a37f83f1610e8d77ed68f07e7>`;
		const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`m_mat_I<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a42030dd0615d38853d1830fc7abc6099>`;
		std::vector<int>& :ref:`m_qubits_in_use<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1aa2b3b9ebb1da9d416a4fea08559b3336>`;

		// construction
	
		:target:`MatrixOfOneLayer<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a83c6eb6523cfaaf8eab5d185a32f00d1>`(
			:ref:`SequenceLayer<doxid-namespace_q_panda_1abc4290cf1f142782fed752eaaffb7d9c>`& layer,
			const :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& prog_dag,
			std::vector<int>& qubits_in_use
			);

		// methods
	
		void :target:`merge_double_gate<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1af9fad019b3fe0bc04ad465566336c71e>`();
		void :target:`merge_calc_unit<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a27806256c7bf402f59a656a30b931932>`();
		void :target:`merge_controled_gate<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1aad907b94e5941ebc286e373e10fdb3d6>`();
		void :target:`merge_sing_gate<doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a549ea9a0d1707b726bccca7b0e15af6a>`();
	};
.. _details-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Fields
------

.. index:: pair: variable; m_double_qubit_gates
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1afa13502053f0bbf9ef9d8961817c30fc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	gateQubitInfo_t m_double_qubit_gates

double qubit gate vector

.. index:: pair: variable; m_single_qubit_gates
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a4d2216e0ea5ad7c4882522b8654055c3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	gateQubitInfo_t m_single_qubit_gates

single qubit gate vector

.. index:: pair: variable; m_controled_gates
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1a7f1abb15d6254db8b51b98e8402902eb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	gateQubitInfo_t m_controled_gates

controled qubit gate vector

.. index:: pair: variable; m_qubits_in_use
.. _doxid-class_q_panda_1_1_q_prog_to_matrix_1_1_matrix_of_one_layer_1aa2b3b9ebb1da9d416a4fea08559b3336:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int>& m_qubits_in_use

the number of all the qubits in the target :ref:`QCircuit <doxid-class_q_panda_1_1_q_circuit>`.

