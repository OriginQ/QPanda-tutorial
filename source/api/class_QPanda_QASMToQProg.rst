.. index:: pair: class; QPanda::QASMToQProg
.. _doxid-class_q_panda_1_1_q_a_s_m_to_q_prog:

class QPanda::QASMToQProg
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

QASM instruction sets convert to quantum program. :ref:`More...<details-class_q_panda_1_1_q_a_s_m_to_q_prog>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QASMToQProg.h>
	
	class QASMToQProg: public :ref:`qasmBaseVisitor<doxid-classqasm_base_visitor>`
	{
	public:
		// construction
	
		:target:`QASMToQProg<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a1440d4b37968730816e89b45f827dccb>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm);

		// methods
	
		virtual antlrcpp::Any :ref:`visitMainprogram<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1add797f9d6d6899e2d19b01dfca31d22b>`(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* ctx);
		virtual antlrcpp::Any :target:`visitHead_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a582fa3e908d15c202ff34bd070d77a0c>`(:ref:`qasmParser::Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitVersion_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a9887563d7a626942d5d37f1c303ed29d>`(:ref:`qasmParser::Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitInclude_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1afb4ed09819bb9d1ccf7c50ec74c5bf0e>`(:ref:`qasmParser::Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitStatement<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1ae0ec62ac0dad2f0ba977086d0fce1c2b>`(:ref:`qasmParser::StatementContext<doxid-classqasm_parser_1_1_statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitReg_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a233b89ff18a342d3962fd627dd84921e>`(:ref:`qasmParser::Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitOpaque_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a8b7a67864063289d322517b1ef2b639c>`(:ref:`qasmParser::Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitIf_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a44b24b707bd79c7358abff820d536ae4>`(:ref:`qasmParser::If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitBarrier_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1acbfec2b3a23a72b0f8f3b49bc3ed5102>`(:ref:`qasmParser::Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitGate_decl<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a0e15e68bdbbf2cf7c2e827d756b22ebf>`(:ref:`qasmParser::Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitGoplist<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a18048767feb186ceaa5daa62ddd974b5>`(:ref:`qasmParser::GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitBop<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a761484c48d772b9b35caaf0dbe556712>`(:ref:`qasmParser::BopContext<doxid-classqasm_parser_1_1_bop_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQop<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1aff19c9d86cddcd8377f47e023d1e36dc>`(:ref:`qasmParser::QopContext<doxid-classqasm_parser_1_1_qop_context>`* ctx);
		virtual antlrcpp::Any :target:`visitUop<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a79958c4c3673ee8f9da80eb8ac8a65a5>`(:ref:`qasmParser::UopContext<doxid-classqasm_parser_1_1_uop_context>`* ctx);
		virtual antlrcpp::Any :target:`visitAnylist<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1ac23fe9ade2a5a4d67cba798c83827a4d>`(:ref:`qasmParser::AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitIdlist<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a370015b27bff0af90118b9a413d1ac2a>`(:ref:`qasmParser::IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitArgument<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a6d47937063948c13f2831cc700d75996>`(:ref:`qasmParser::ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* ctx);
		virtual antlrcpp::Any :target:`visitId_index<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a9cf03efca4eae5ebc6a577cb4b502799>`(:ref:`qasmParser::Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* ctx);
		virtual antlrcpp::Any :target:`visitExplist<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a3d362ded3f59fcbc364b94b1b56baa8b>`(:ref:`qasmParser::ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitExp<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1abd6e33c8f58c9b1bc4d61491172fe4e4>`(:ref:`qasmParser::ExpContext<doxid-classqasm_parser_1_1_exp_context>`* ctx);
		virtual antlrcpp::Any :target:`visitId<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a218da85122f9cf8bf1b0b80b33ee88db>`(:ref:`qasmParser::IdContext<doxid-classqasm_parser_1_1_id_context>`* ctx);
		virtual antlrcpp::Any :target:`visitInteger<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a5317887fb4b0303b7f880ccc0be159ad>`(:ref:`qasmParser::IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDecimal<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a61548929abfed71d7f5d53ae82b8d549>`(:ref:`qasmParser::DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* ctx);
		virtual antlrcpp::Any :target:`visitFilename<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a1919e880c009063b60a77dcd2ed71691>`(:ref:`qasmParser::FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* ctx);
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`find_qvec_map_value<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1ab0fbcc038347bb5bc9aeab0305d22288>`(std::string str_key);
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :target:`find_cvec_map_value<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1afcdadc52a4d3f5184a3c5fdd799ee4dd>`(std::string str_key);
	
		void :target:`execute_gate_function<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1aac7d57d01cf50fef2e22f449edf8ee87>`(
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_zero_param_single_gate<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a95af0f926731b061f238a3f0e76fb61c>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			bool is_dagger,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_one_param_single_gate<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a894cc28d8a9599b0d22f8b93819d198d>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_two_param_single_gate_func<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1aee581432c20b7aed050c91bd514a9f7c>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_three_param_single_gate<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1aa3c3d2b61ef78294bf336a95472eb231>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_zero_param_double_gate<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a22e893f6d044e0e387cab0267984cd7a>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_zero_param_triple_gate<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a9e5b8c26abaaf1a8d55b869779bb0f2b>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_zero_param_double_circuit<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a8ed65c140d536b60587ec9a1fe27d55a>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_one_param_double_circuit<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a83ce6f5b59a1963c4bbe8cda90faba3f>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_three_param_double_circuit<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a78f051426c4d721ccc034b508d1b5b3a>`(
			:ref:`QASMGateType<doxid-namespace_q_panda_1a15ea0e7d93f36cdc8f6b05fd91ef7b12>` type,
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		void :target:`build_qprog<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1abd3cdbcff3c302d3af222ad5e68d1325>`(
			:ref:`GateOperationInfo<doxid-struct_q_panda_1_1_gate_operation_info>` op_info,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog
			);
	
		:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` :ref:`get_qprog<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a2ea30745e5651e63e9904303352c5bb9>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual antlrcpp::Any :ref:`visitMainprogram<doxid-classqasm_visitor_1ab92a4a4c0a149e01df36439b00d551c6>`(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitHead_decl<doxid-classqasm_visitor_1a17e51d512a9fffdda83adfab0875eaca>`(:ref:`qasmParser::Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitVersion_decl<doxid-classqasm_visitor_1a9c486a0fc618ce663f2b760a34d6b339>`(:ref:`qasmParser::Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitInclude_decl<doxid-classqasm_visitor_1a4cbde57d0e29cc498a432ffa7c40000c>`(:ref:`qasmParser::Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitStatement<doxid-classqasm_visitor_1ad8ec10703807be439d541808919eeb7f>`(:ref:`qasmParser::StatementContext<doxid-classqasm_parser_1_1_statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitReg_decl<doxid-classqasm_visitor_1ae181dc20abb07ef574443ff84c1a7258>`(:ref:`qasmParser::Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitOpaque_decl<doxid-classqasm_visitor_1a0576b40bded3c632f2d2158a50dfbd64>`(:ref:`qasmParser::Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitIf_decl<doxid-classqasm_visitor_1ad843ce920a52cd39c206fa35df953fbc>`(:ref:`qasmParser::If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitBarrier_decl<doxid-classqasm_visitor_1a7c4afc775857e0f914ec499699444d25>`(:ref:`qasmParser::Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitGate_decl<doxid-classqasm_visitor_1a84cfebeb0596b2fd66866d2a32d06d27>`(:ref:`qasmParser::Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitGoplist<doxid-classqasm_visitor_1a28edf8cce865bc0fd1fb6fec0891ccbb>`(:ref:`qasmParser::GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitBop<doxid-classqasm_visitor_1a86cd0ec72f5b11ecaf1fbbce767540a2>`(:ref:`qasmParser::BopContext<doxid-classqasm_parser_1_1_bop_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQop<doxid-classqasm_visitor_1af14e205be9c42326e2776eb235dd36df>`(:ref:`qasmParser::QopContext<doxid-classqasm_parser_1_1_qop_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitUop<doxid-classqasm_visitor_1a87004cc1e9cd6395360bb61f67239ea7>`(:ref:`qasmParser::UopContext<doxid-classqasm_parser_1_1_uop_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitAnylist<doxid-classqasm_visitor_1a3969188bb4c9d8453ff7a6f7b53ccd98>`(:ref:`qasmParser::AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitIdlist<doxid-classqasm_visitor_1a771c78a8ef8c8f5c43f0fed084ae08fa>`(:ref:`qasmParser::IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitId_index<doxid-classqasm_visitor_1a58e717158d05ca7660eb4eedea7efc7c>`(:ref:`qasmParser::Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitArgument<doxid-classqasm_visitor_1aaf45897a06ef34fb32a0b93b1c2f838a>`(:ref:`qasmParser::ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitExplist<doxid-classqasm_visitor_1a0fe32d9ce227beb9454716490b27347b>`(:ref:`qasmParser::ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitExp<doxid-classqasm_visitor_1a770c73bb0db6ad549842dc5f880fd5ed>`(:ref:`qasmParser::ExpContext<doxid-classqasm_parser_1_1_exp_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitId<doxid-classqasm_visitor_1aa64d339b752b1b2972169a9c4a4caa9b>`(:ref:`qasmParser::IdContext<doxid-classqasm_parser_1_1_id_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitInteger<doxid-classqasm_visitor_1ac8eb7df5f1d6ae51bc07930b3c5d8074>`(:ref:`qasmParser::IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDecimal<doxid-classqasm_visitor_1a3970782307f706067fd6bc4a2d3a3c63>`(:ref:`qasmParser::DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitFilename<doxid-classqasm_visitor_1a6ea813f3f70f1ae02a536fc5037e34f2>`(:ref:`qasmParser::FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitMainprogram<doxid-classqasm_base_visitor_1a0bf2acc524fe87113ce0db01be5823e6>`(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* context);
		virtual antlrcpp::Any :ref:`visitHead_decl<doxid-classqasm_base_visitor_1aa804b972df928f8266cc5323fbd43a20>`(:ref:`qasmParser::Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitVersion_decl<doxid-classqasm_base_visitor_1aac5e8e9d01a1fbbf83e69fd348adb527>`(:ref:`qasmParser::Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitInclude_decl<doxid-classqasm_base_visitor_1a86b2823032582700afc5207657fa73ce>`(:ref:`qasmParser::Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitStatement<doxid-classqasm_base_visitor_1a16bbd72ecc697376ba3c1b7a51d13ae8>`(:ref:`qasmParser::StatementContext<doxid-classqasm_parser_1_1_statement_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitReg_decl<doxid-classqasm_base_visitor_1abe8d180d97f4716ab49dd7cb7387923a>`(:ref:`qasmParser::Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitOpaque_decl<doxid-classqasm_base_visitor_1aa76015fed3611338d47f3a7962c820cc>`(:ref:`qasmParser::Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitIf_decl<doxid-classqasm_base_visitor_1a2f2067c699ed47ee4c4829b826649b9a>`(:ref:`qasmParser::If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitBarrier_decl<doxid-classqasm_base_visitor_1ae3c282bb1016e0eac8e0f714ead3a671>`(:ref:`qasmParser::Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitGate_decl<doxid-classqasm_base_visitor_1aad2559f2e1e093061c4a3d63b5de937f>`(:ref:`qasmParser::Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitGoplist<doxid-classqasm_base_visitor_1a81ec2a615930de7fa23c212978ef91be>`(:ref:`qasmParser::GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitBop<doxid-classqasm_base_visitor_1ae316d68087a2b87e043ec1269cda1daa>`(:ref:`qasmParser::BopContext<doxid-classqasm_parser_1_1_bop_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitQop<doxid-classqasm_base_visitor_1a5643914fa50a6efecada9fdc8e58de1d>`(:ref:`qasmParser::QopContext<doxid-classqasm_parser_1_1_qop_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitUop<doxid-classqasm_base_visitor_1aa32a254cedcdafcf1139049baa93e085>`(:ref:`qasmParser::UopContext<doxid-classqasm_parser_1_1_uop_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitAnylist<doxid-classqasm_base_visitor_1a6abb176fce0fe87c29d099b2bb1ab770>`(:ref:`qasmParser::AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitIdlist<doxid-classqasm_base_visitor_1a11a7c959ff280e481806d2ef456d532a>`(:ref:`qasmParser::IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitId_index<doxid-classqasm_base_visitor_1aec3baf8244917f8de12d5ac1b835a0ae>`(:ref:`qasmParser::Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitArgument<doxid-classqasm_base_visitor_1a0ca42e9a168b4b7f70a46b8a747e75d6>`(:ref:`qasmParser::ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitExplist<doxid-classqasm_base_visitor_1a251a3219766b3a6f20412668b87a1943>`(:ref:`qasmParser::ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitExp<doxid-classqasm_base_visitor_1a66e94ef84249d02a6dd6d3e469e83f20>`(:ref:`qasmParser::ExpContext<doxid-classqasm_parser_1_1_exp_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitId<doxid-classqasm_base_visitor_1a33e6dae78f4b66e4169b2409895f31db>`(:ref:`qasmParser::IdContext<doxid-classqasm_parser_1_1_id_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitInteger<doxid-classqasm_base_visitor_1a0d68ab9026fbd162e63144366457b86e>`(:ref:`qasmParser::IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitDecimal<doxid-classqasm_base_visitor_1a9b46e0297d9e463f31b6a1bae78cd28e>`(:ref:`qasmParser::DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* ctx);
		virtual antlrcpp::Any :ref:`visitFilename<doxid-classqasm_base_visitor_1a2d3840f07a8c13dbce318d9bf0247859>`(:ref:`qasmParser::FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* ctx);

.. _details-class_q_panda_1_1_q_a_s_m_to_q_prog:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QASM instruction sets convert to quantum program.

Methods
-------

.. index:: pair: function; visitMainprogram
.. _doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1add797f9d6d6899e2d19b01dfca31d22b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual antlrcpp::Any visitMainprogram(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* ctx)

They are abstract visitors for a parse tree produced by :ref:`qasmParser <doxid-classqasm_parser>`.

.. index:: pair: function; get_qprog
.. _doxid-class_q_panda_1_1_q_a_s_m_to_q_prog_1a2ea30745e5651e63e9904303352c5bb9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QProg<doxid-class_q_panda_1_1_q_prog>` get_qprog()

get converted quantum programs



.. rubric:: Returns:

:ref:`QProg <doxid-class_q_panda_1_1_q_prog>`

