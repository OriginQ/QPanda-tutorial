.. index:: pair: class; qasmBaseVisitor
.. _doxid-classqasm_base_visitor:

class qasmBaseVisitor
=====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

This class provides an empty implementation of :ref:`qasmVisitor <doxid-classqasm_visitor>`, which can be extended to create a visitor which only needs to handle a subset of the available methods. :ref:`More...<details-classqasm_base_visitor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmBaseVisitor.h>
	
	class qasmBaseVisitor: public :ref:`qasmVisitor<doxid-classqasm_visitor>`
	{
	public:
		// methods
	
		virtual antlrcpp::Any :ref:`visitMainprogram<doxid-classqasm_base_visitor_1a0bf2acc524fe87113ce0db01be5823e6>`(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* context);
		virtual antlrcpp::Any :target:`visitHead_decl<doxid-classqasm_base_visitor_1aa804b972df928f8266cc5323fbd43a20>`(:ref:`qasmParser::Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitVersion_decl<doxid-classqasm_base_visitor_1aac5e8e9d01a1fbbf83e69fd348adb527>`(:ref:`qasmParser::Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitInclude_decl<doxid-classqasm_base_visitor_1a86b2823032582700afc5207657fa73ce>`(:ref:`qasmParser::Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitStatement<doxid-classqasm_base_visitor_1a16bbd72ecc697376ba3c1b7a51d13ae8>`(:ref:`qasmParser::StatementContext<doxid-classqasm_parser_1_1_statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitReg_decl<doxid-classqasm_base_visitor_1abe8d180d97f4716ab49dd7cb7387923a>`(:ref:`qasmParser::Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitOpaque_decl<doxid-classqasm_base_visitor_1aa76015fed3611338d47f3a7962c820cc>`(:ref:`qasmParser::Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitIf_decl<doxid-classqasm_base_visitor_1a2f2067c699ed47ee4c4829b826649b9a>`(:ref:`qasmParser::If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitBarrier_decl<doxid-classqasm_base_visitor_1ae3c282bb1016e0eac8e0f714ead3a671>`(:ref:`qasmParser::Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitGate_decl<doxid-classqasm_base_visitor_1aad2559f2e1e093061c4a3d63b5de937f>`(:ref:`qasmParser::Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* ctx);
		virtual antlrcpp::Any :target:`visitGoplist<doxid-classqasm_base_visitor_1a81ec2a615930de7fa23c212978ef91be>`(:ref:`qasmParser::GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitBop<doxid-classqasm_base_visitor_1ae316d68087a2b87e043ec1269cda1daa>`(:ref:`qasmParser::BopContext<doxid-classqasm_parser_1_1_bop_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQop<doxid-classqasm_base_visitor_1a5643914fa50a6efecada9fdc8e58de1d>`(:ref:`qasmParser::QopContext<doxid-classqasm_parser_1_1_qop_context>`* ctx);
		virtual antlrcpp::Any :target:`visitUop<doxid-classqasm_base_visitor_1aa32a254cedcdafcf1139049baa93e085>`(:ref:`qasmParser::UopContext<doxid-classqasm_parser_1_1_uop_context>`* ctx);
		virtual antlrcpp::Any :target:`visitAnylist<doxid-classqasm_base_visitor_1a6abb176fce0fe87c29d099b2bb1ab770>`(:ref:`qasmParser::AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitIdlist<doxid-classqasm_base_visitor_1a11a7c959ff280e481806d2ef456d532a>`(:ref:`qasmParser::IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitId_index<doxid-classqasm_base_visitor_1aec3baf8244917f8de12d5ac1b835a0ae>`(:ref:`qasmParser::Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* ctx);
		virtual antlrcpp::Any :target:`visitArgument<doxid-classqasm_base_visitor_1a0ca42e9a168b4b7f70a46b8a747e75d6>`(:ref:`qasmParser::ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* ctx);
		virtual antlrcpp::Any :target:`visitExplist<doxid-classqasm_base_visitor_1a251a3219766b3a6f20412668b87a1943>`(:ref:`qasmParser::ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* ctx);
		virtual antlrcpp::Any :target:`visitExp<doxid-classqasm_base_visitor_1a66e94ef84249d02a6dd6d3e469e83f20>`(:ref:`qasmParser::ExpContext<doxid-classqasm_parser_1_1_exp_context>`* ctx);
		virtual antlrcpp::Any :target:`visitId<doxid-classqasm_base_visitor_1a33e6dae78f4b66e4169b2409895f31db>`(:ref:`qasmParser::IdContext<doxid-classqasm_parser_1_1_id_context>`* ctx);
		virtual antlrcpp::Any :target:`visitInteger<doxid-classqasm_base_visitor_1a0d68ab9026fbd162e63144366457b86e>`(:ref:`qasmParser::IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDecimal<doxid-classqasm_base_visitor_1a9b46e0297d9e463f31b6a1bae78cd28e>`(:ref:`qasmParser::DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* ctx);
		virtual antlrcpp::Any :target:`visitFilename<doxid-classqasm_base_visitor_1a2d3840f07a8c13dbce318d9bf0247859>`(:ref:`qasmParser::FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* ctx);
	};

	// direct descendants

	class :ref:`QASMToQProg<doxid-class_q_panda_1_1_q_a_s_m_to_q_prog>`;

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

.. _details-classqasm_base_visitor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class provides an empty implementation of :ref:`qasmVisitor <doxid-classqasm_visitor>`, which can be extended to create a visitor which only needs to handle a subset of the available methods.

Methods
-------

.. index:: pair: function; visitMainprogram
.. _doxid-classqasm_base_visitor_1a0bf2acc524fe87113ce0db01be5823e6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual antlrcpp::Any visitMainprogram(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* context)

Visit parse trees produced by :ref:`qasmParser <doxid-classqasm_parser>`.

