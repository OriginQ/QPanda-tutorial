.. index:: pair: class; QPanda::QProgBuilder
.. _doxid-class_q_panda_1_1_q_prog_builder:

class QPanda::QProgBuilder
==========================

.. toctree::
	:hidden:

	enum_QPanda_QProgBuilder_GateType.rst

Quantum Program Builder.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginIRToQProg.h>
	
	class QProgBuilder
	{
	public:
		// enums
	
		enum :ref:`GateType<doxid-class_q_panda_1_1_q_prog_builder_1a06ddf4812a401a6835efd12e7767928d>`;

		// construction
	
		:target:`QProgBuilder<doxid-class_q_panda_1_1_q_prog_builder_1a0547c58a5c84814c37299a50b6a13391>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);

		// methods
	
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :target:`get_qprog<doxid-class_q_panda_1_1_q_prog_builder_1acb6b8ccc8b0c284309968a52169bd536>`();
		void :target:`alloc_qubit<doxid-class_q_panda_1_1_q_prog_builder_1a092c75f0975c717ccf164cc73b76cb4a>`(int num);
		void :target:`alloc_cbit<doxid-class_q_panda_1_1_q_prog_builder_1aebae2d1c406396ef8f27f461aac6f45b>`(int num);
		size_t :target:`add_prog<doxid-class_q_panda_1_1_q_prog_builder_1a500da87bc1d76f3199235b78c713a7c2>`();
	
		void :target:`insert_subprog<doxid-class_q_panda_1_1_q_prog_builder_1ae1f4e0946e780980c8a5e945ead2c3e5>`(
			size_t progid_dst,
			size_t progid_src
			);
	
		size_t :target:`add_qgate<doxid-class_q_panda_1_1_q_prog_builder_1a9cef0c4caa4757626e9b0f2491cc60e9>`(
			:ref:`GateType<doxid-class_q_panda_1_1_q_prog_builder_1a06ddf4812a401a6835efd12e7767928d>` type,
			std::vector<int> index,
			std::vector<double> parameters
			);
	
		size_t :target:`add_qgate_cc<doxid-class_q_panda_1_1_q_prog_builder_1a0abbad3d52a1fe90eaf1d40e2d7c2906>`(
			:ref:`GateType<doxid-class_q_panda_1_1_q_prog_builder_1a06ddf4812a401a6835efd12e7767928d>` type,
			std::vector<size_t> exprid,
			std::vector<int> index,
			std::vector<double> parameters
			);
	
		size_t :target:`add_measure_literal<doxid-class_q_panda_1_1_q_prog_builder_1aae8722bd2bbe37dc7fc3a50f7e63273d>`(
			size_t qidx,
			size_t cidx
			);
	
		size_t :target:`add_measure_cc<doxid-class_q_panda_1_1_q_prog_builder_1a9e30c5aac49cd8d51d0c48971b497c62>`(
			size_t exprid,
			size_t cidx
			);
	
		size_t :target:`add_reset_literal<doxid-class_q_panda_1_1_q_prog_builder_1a958dcf227094f033a279008ae081da69>`(size_t qidx);
		size_t :target:`add_reset_cc<doxid-class_q_panda_1_1_q_prog_builder_1a0c2b69decc872e46e2d68099129bfa9b>`(size_t exprid);
		size_t :target:`add_expr_stat<doxid-class_q_panda_1_1_q_prog_builder_1ad51f01c881d0b32c169ab387ea68f5ea>`(size_t exprid);
	
		size_t :target:`make_qif<doxid-class_q_panda_1_1_q_prog_builder_1aec37cfbb6b4450bb553bb5f314f7a94c>`(
			size_t exprid,
			size_t progid
			);
	
		size_t :target:`make_qifelse<doxid-class_q_panda_1_1_q_prog_builder_1a89c35e8d38c558dd224bdd8e3b9120f9>`(
			size_t exprid,
			size_t progid_true,
			size_t progid_false
			);
	
		size_t :target:`make_qwhile<doxid-class_q_panda_1_1_q_prog_builder_1abe10a58b4f762a112076f75d27f21e75>`(
			size_t exprid,
			size_t progid
			);
	
		void :target:`delete_prog<doxid-class_q_panda_1_1_q_prog_builder_1a3191c49fcbcc24068e5f74a6fb6f024e>`(size_t progid);
		size_t :target:`cc_init_id<doxid-class_q_panda_1_1_q_prog_builder_1a4380cbbcf5ecb31dc45bb45acf6583df>`(size_t cidx);
		size_t :target:`cc_init_literal<doxid-class_q_panda_1_1_q_prog_builder_1a7c0c4809eaf33f9d32db529baca5a2b8>`(double value);
	
		size_t :target:`cc_op_cc<doxid-class_q_panda_1_1_q_prog_builder_1a5bcd0167c11daea48aad6c77b62fe9c9>`(
			size_t exprid1,
			size_t exprid2,
			int op_type
			);
	
		size_t :target:`cc_op_literal<doxid-class_q_panda_1_1_q_prog_builder_1abd3495e6723bbace0804984d99909f8c>`(
			size_t exprid1,
			double literal2,
			int op_type
			);
	
		size_t :target:`literal_op_cc<doxid-class_q_panda_1_1_q_prog_builder_1af3073ef66c7486ad8ea83a475f252d7f>`(
			double literal1,
			size_t exprid2,
			int op_type
			);
	
		size_t :target:`op_cc<doxid-class_q_panda_1_1_q_prog_builder_1a5113f818285cc56861f6b7160e52fddc>`(
			size_t exprid,
			int op_type
			);
	
		void :target:`make_dagger<doxid-class_q_panda_1_1_q_prog_builder_1a7db65c1bde7e6d21c98a450e56cc0c48>`(size_t progid);
		size_t :target:`make_dagger_new<doxid-class_q_panda_1_1_q_prog_builder_1abed98cfeee9322f59c8430d3b47ab692>`(size_t progid);
	
		void :target:`make_control<doxid-class_q_panda_1_1_q_prog_builder_1ade39bd5aaa686d39ee18bf38248f9ee6>`(
			size_t progid,
			std::vector<int> idx
			);
	
		size_t :target:`make_control_new<doxid-class_q_panda_1_1_q_prog_builder_1a3d2ed260614e819f9cfe6639f62fe8c5>`(
			size_t progid,
			std::vector<int> idx
			);
	
		void :target:`make_control_cc<doxid-class_q_panda_1_1_q_prog_builder_1afb92954efc82abf54fbd22f260184da6>`(
			size_t progid,
			std::vector<size_t> expridx,
			std::vector<int> idx
			);
	
		size_t :target:`make_control_cc_new<doxid-class_q_panda_1_1_q_prog_builder_1a26b3d590634c9715a95da2f7e01592e4>`(
			size_t progid,
			std::vector<size_t> expridx,
			std::vector<int> idx
			);
	
		static :ref:`GateType<doxid-class_q_panda_1_1_q_prog_builder_1a06ddf4812a401a6835efd12e7767928d>` :target:`get_gatetype<doxid-class_q_panda_1_1_q_prog_builder_1adede88a7bb9bb0fb6a4654afd3823c73>`(std::string gatename);
	};
