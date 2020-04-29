.. index:: pair: class; qasmVisitor
.. _doxid-classqasm_visitor:

class qasmVisitor
=================

.. toctree::
	:hidden:

Overview
~~~~~~~~

This class defines an abstract visitor for a parse tree produced by :ref:`qasmParser <doxid-classqasm_parser>`. :ref:`More...<details-classqasm_visitor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmVisitor.h>
	
	class qasmVisitor: public AbstractParseTreeVisitor
	{
	public:
		// methods
	
		virtual antlrcpp::Any :ref:`visitMainprogram<doxid-classqasm_visitor_1ab92a4a4c0a149e01df36439b00d551c6>`(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitHead_decl<doxid-classqasm_visitor_1a17e51d512a9fffdda83adfab0875eaca>`(:ref:`qasmParser::Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitVersion_decl<doxid-classqasm_visitor_1a9c486a0fc618ce663f2b760a34d6b339>`(:ref:`qasmParser::Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitInclude_decl<doxid-classqasm_visitor_1a4cbde57d0e29cc498a432ffa7c40000c>`(:ref:`qasmParser::Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitStatement<doxid-classqasm_visitor_1ad8ec10703807be439d541808919eeb7f>`(:ref:`qasmParser::StatementContext<doxid-classqasm_parser_1_1_statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitReg_decl<doxid-classqasm_visitor_1ae181dc20abb07ef574443ff84c1a7258>`(:ref:`qasmParser::Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitOpaque_decl<doxid-classqasm_visitor_1a0576b40bded3c632f2d2158a50dfbd64>`(:ref:`qasmParser::Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitIf_decl<doxid-classqasm_visitor_1ad843ce920a52cd39c206fa35df953fbc>`(:ref:`qasmParser::If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitBarrier_decl<doxid-classqasm_visitor_1a7c4afc775857e0f914ec499699444d25>`(:ref:`qasmParser::Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitGate_decl<doxid-classqasm_visitor_1a84cfebeb0596b2fd66866d2a32d06d27>`(:ref:`qasmParser::Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitGoplist<doxid-classqasm_visitor_1a28edf8cce865bc0fd1fb6fec0891ccbb>`(:ref:`qasmParser::GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitBop<doxid-classqasm_visitor_1a86cd0ec72f5b11ecaf1fbbce767540a2>`(:ref:`qasmParser::BopContext<doxid-classqasm_parser_1_1_bop_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQop<doxid-classqasm_visitor_1af14e205be9c42326e2776eb235dd36df>`(:ref:`qasmParser::QopContext<doxid-classqasm_parser_1_1_qop_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitUop<doxid-classqasm_visitor_1a87004cc1e9cd6395360bb61f67239ea7>`(:ref:`qasmParser::UopContext<doxid-classqasm_parser_1_1_uop_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitAnylist<doxid-classqasm_visitor_1a3969188bb4c9d8453ff7a6f7b53ccd98>`(:ref:`qasmParser::AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitIdlist<doxid-classqasm_visitor_1a771c78a8ef8c8f5c43f0fed084ae08fa>`(:ref:`qasmParser::IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitId_index<doxid-classqasm_visitor_1a58e717158d05ca7660eb4eedea7efc7c>`(:ref:`qasmParser::Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitArgument<doxid-classqasm_visitor_1aaf45897a06ef34fb32a0b93b1c2f838a>`(:ref:`qasmParser::ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitExplist<doxid-classqasm_visitor_1a0fe32d9ce227beb9454716490b27347b>`(:ref:`qasmParser::ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitExp<doxid-classqasm_visitor_1a770c73bb0db6ad549842dc5f880fd5ed>`(:ref:`qasmParser::ExpContext<doxid-classqasm_parser_1_1_exp_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitId<doxid-classqasm_visitor_1aa64d339b752b1b2972169a9c4a4caa9b>`(:ref:`qasmParser::IdContext<doxid-classqasm_parser_1_1_id_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitInteger<doxid-classqasm_visitor_1ac8eb7df5f1d6ae51bc07930b3c5d8074>`(:ref:`qasmParser::IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDecimal<doxid-classqasm_visitor_1a3970782307f706067fd6bc4a2d3a3c63>`(:ref:`qasmParser::DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitFilename<doxid-classqasm_visitor_1a6ea813f3f70f1ae02a536fc5037e34f2>`(:ref:`qasmParser::FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* context) = 0;
	};

	// direct descendants

	class :ref:`qasmBaseVisitor<doxid-classqasm_base_visitor>`;
.. _details-classqasm_visitor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class defines an abstract visitor for a parse tree produced by :ref:`qasmParser <doxid-classqasm_parser>`.

Methods
-------

.. index:: pair: function; visitMainprogram
.. _doxid-classqasm_visitor_1ab92a4a4c0a149e01df36439b00d551c6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual antlrcpp::Any visitMainprogram(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* context) = 0

Visit parse trees produced by :ref:`qasmParser <doxid-classqasm_parser>`.

