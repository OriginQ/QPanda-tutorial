.. index:: pair: class; originirVisitor
.. _doxid-classoriginir_visitor:

class originirVisitor
=====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

This class defines an abstract visitor for a parse tree produced by :ref:`originirParser <doxid-classoriginir_parser>`. :ref:`More...<details-classoriginir_visitor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirVisitor.h>
	
	class originirVisitor: public AbstractParseTreeVisitor
	{
	public:
		// methods
	
		virtual antlrcpp::Any :ref:`visitTranslationunit<doxid-classoriginir_visitor_1afabf405697abbff4744d8e30e9dce7bc>`(:ref:`originirParser::TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDeclaration<doxid-classoriginir_visitor_1abb80f1743facd0c41a0eafbade8fbefb>`(:ref:`originirParser::DeclarationContext<doxid-classoriginir_parser_1_1_declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQinit_declaration<doxid-classoriginir_visitor_1ae1482d0a0054f467be39ad865cbac93d>`(:ref:`originirParser::Qinit_declarationContext<doxid-classoriginir_parser_1_1_qinit__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitCinit_declaration<doxid-classoriginir_visitor_1a4337389f960db0a4314770c74fe6cfd2>`(:ref:`originirParser::Cinit_declarationContext<doxid-classoriginir_parser_1_1_cinit__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQuantum_gate_declaration<doxid-classoriginir_visitor_1a4558aa4ac5cfcb1d94597d94bbd7c245>`(:ref:`originirParser::Quantum_gate_declarationContext<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitIndex<doxid-classoriginir_visitor_1af4104aeb1a819a096daf45c78b8d4b01>`(:ref:`originirParser::IndexContext<doxid-classoriginir_parser_1_1_index_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitC_KEY_declaration<doxid-classoriginir_visitor_1aa0e79512132fae4d0666e5f5f9328f70>`(:ref:`originirParser::C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQ_KEY_declaration<doxid-classoriginir_visitor_1a67c701c6033a604077d84790ce331cb7>`(:ref:`originirParser::Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_without_parameter_declaration<doxid-classoriginir_visitor_1a207064859ea5a14f04a96e45d045feff>`(:ref:`originirParser::Single_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_one_parameter_declaration<doxid-classoriginir_visitor_1a288ac3dc5e50e19ef5b3c50075a67300>`(:ref:`originirParser::Single_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_two_parameter_declaration<doxid-classoriginir_visitor_1a1238c1457efd1b44a73241b550678204>`(:ref:`originirParser::Single_gate_with_two_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_three_parameter_declaration<doxid-classoriginir_visitor_1a20e8d4c49e44a1d32e852232df9a6a99>`(:ref:`originirParser::Single_gate_with_three_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_four_parameter_declaration<doxid-classoriginir_visitor_1a715006a175402c3687b81a824d48f91b>`(:ref:`originirParser::Single_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDouble_gate_without_parameter_declaration<doxid-classoriginir_visitor_1a330ff4f28a1b8b9a49587567bac80fd8>`(:ref:`originirParser::Double_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDouble_gate_with_one_parameter_declaration<doxid-classoriginir_visitor_1a94f72e10a20134d865036113bac9c454>`(:ref:`originirParser::Double_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDouble_gate_with_four_parameter_declaration<doxid-classoriginir_visitor_1a6b35d772a224894b5a6acab1e3c3b80c>`(:ref:`originirParser::Double_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitTriple_gate_without_parameter_declaration<doxid-classoriginir_visitor_1a650ba14d421b0fc96f1ee8aac39af4df>`(:ref:`originirParser::Triple_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_without_parameter_type<doxid-classoriginir_visitor_1a2b2d973981441bb17e7d575106f22252>`(:ref:`originirParser::Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_one_parameter_type<doxid-classoriginir_visitor_1a774b6f00bfb4721574e9d2ff8c5d04ef>`(:ref:`originirParser::Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_two_parameter_type<doxid-classoriginir_visitor_1a46bd8a9a9f01652d6d3a39f81fff2cb8>`(:ref:`originirParser::Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_three_parameter_type<doxid-classoriginir_visitor_1a3d1d35bfec5bb10234ff3dc540389c30>`(:ref:`originirParser::Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitSingle_gate_with_four_parameter_type<doxid-classoriginir_visitor_1a6344a834440e372c72a93d4111e03a4f>`(:ref:`originirParser::Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDouble_gate_without_parameter_type<doxid-classoriginir_visitor_1ae92b1b5816bbf9cb56bb197aa4c6c508>`(:ref:`originirParser::Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDouble_gate_with_one_parameter_type<doxid-classoriginir_visitor_1acd0e38df429ed0ddf1e212d27d54aced>`(:ref:`originirParser::Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDouble_gate_with_four_parameter_type<doxid-classoriginir_visitor_1aec75cbd82197f4ce3f49ce4b35db8262>`(:ref:`originirParser::Double_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitTriple_gate_without_parameter_type<doxid-classoriginir_visitor_1a99541b3032ebf22df1a2588aa2184a9b>`(:ref:`originirParser::Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitPri_ckey<doxid-classoriginir_visitor_1aa0536a564fefdc47148aed8ca5f64f6b>`(:ref:`originirParser::Pri_ckeyContext<doxid-classoriginir_parser_1_1_pri__ckey_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitPri_cst<doxid-classoriginir_visitor_1a2c167188c3ccfec7358c973315b7b0b8>`(:ref:`originirParser::Pri_cstContext<doxid-classoriginir_parser_1_1_pri__cst_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitPri_expr<doxid-classoriginir_visitor_1ab3ad33baf4acdb03692847f2e4b8d4eb>`(:ref:`originirParser::Pri_exprContext<doxid-classoriginir_parser_1_1_pri__expr_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitUnary_expression<doxid-classoriginir_visitor_1a2df2aea4add7d445c87fc0440a393104>`(:ref:`originirParser::Unary_expressionContext<doxid-classoriginir_parser_1_1_unary__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitMultiplicative_expression<doxid-classoriginir_visitor_1a958ae8cccd94b1d6b78e749e0537a435>`(:ref:`originirParser::Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitAddtive_expression<doxid-classoriginir_visitor_1a1c4c8cbeda0b35d0f8b12145ecd05d33>`(:ref:`originirParser::Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitRelational_expression<doxid-classoriginir_visitor_1a00d18d7b76cfa9d791b4c87581912f7b>`(:ref:`originirParser::Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitEquality_expression<doxid-classoriginir_visitor_1a80cc6eedd7156e3d86bd2a6d66b96186>`(:ref:`originirParser::Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitLogical_and_expression<doxid-classoriginir_visitor_1a67a8c994bb9e58e602bd186f880cf98d>`(:ref:`originirParser::Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitLogical_or_expression<doxid-classoriginir_visitor_1afc9ab3638f609091c41712434ff7a65d>`(:ref:`originirParser::Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitAssignment_expression<doxid-classoriginir_visitor_1a69919dd8fca6babda06bb8a591113b02>`(:ref:`originirParser::Assignment_expressionContext<doxid-classoriginir_parser_1_1_assignment__expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitExpression<doxid-classoriginir_visitor_1a96863a8fad5b282b5e2bc56bc48fb4a0>`(:ref:`originirParser::ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitControlbit_list<doxid-classoriginir_visitor_1aa36bb95f0fa9aba7cfe481d4922a01d5>`(:ref:`originirParser::Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitStatement<doxid-classoriginir_visitor_1a52b586173bfbe017a1cffe1c73b1aed4>`(:ref:`originirParser::StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitDagger_statement<doxid-classoriginir_visitor_1aa79dc2ac1a1b7ff1c85d7ab961fd5e7c>`(:ref:`originirParser::Dagger_statementContext<doxid-classoriginir_parser_1_1_dagger__statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitControl_statement<doxid-classoriginir_visitor_1a677f5b1d33654e76c7e62f1aa9ef846c>`(:ref:`originirParser::Control_statementContext<doxid-classoriginir_parser_1_1_control__statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQelse_statement_fragment<doxid-classoriginir_visitor_1a20f88c103605209420db646adb5666de>`(:ref:`originirParser::Qelse_statement_fragmentContext<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQif_if<doxid-classoriginir_visitor_1a84c35b9037f67fe882b755ace2748825>`(:ref:`originirParser::Qif_ifContext<doxid-classoriginir_parser_1_1_qif__if_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQif_ifelse<doxid-classoriginir_visitor_1a2effd56b537d2ceafbe07c5b79f578e5>`(:ref:`originirParser::Qif_ifelseContext<doxid-classoriginir_parser_1_1_qif__ifelse_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitQwhile_statement<doxid-classoriginir_visitor_1ad57bec937e5cf88af27b31dc8cf1e5f3>`(:ref:`originirParser::Qwhile_statementContext<doxid-classoriginir_parser_1_1_qwhile__statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitMeasure_statement<doxid-classoriginir_visitor_1a2a9575d11bbec345f91d7a54408348e2>`(:ref:`originirParser::Measure_statementContext<doxid-classoriginir_parser_1_1_measure__statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitReset_statement<doxid-classoriginir_visitor_1aea822832627154b0d27abb3461e61dab>`(:ref:`originirParser::Reset_statementContext<doxid-classoriginir_parser_1_1_reset__statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitExpression_statement<doxid-classoriginir_visitor_1abeef7f57a2b1b8e25d9108a68e011191>`(:ref:`originirParser::Expression_statementContext<doxid-classoriginir_parser_1_1_expression__statement_context>`* context) = 0;
		virtual antlrcpp::Any :target:`visitConstant<doxid-classoriginir_visitor_1a643e97d350ab10b740e5d599ceb3121c>`(:ref:`originirParser::ConstantContext<doxid-classoriginir_parser_1_1_constant_context>`* context) = 0;
	};

	// direct descendants

	class :ref:`originirBaseVisitor<doxid-classoriginir_base_visitor>`;
.. _details-classoriginir_visitor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class defines an abstract visitor for a parse tree produced by :ref:`originirParser <doxid-classoriginir_parser>`.

Methods
-------

.. index:: pair: function; visitTranslationunit
.. _doxid-classoriginir_visitor_1afabf405697abbff4744d8e30e9dce7bc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual antlrcpp::Any visitTranslationunit(:ref:`originirParser::TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context>`* context) = 0

Visit parse trees produced by :ref:`originirParser <doxid-classoriginir_parser>`.

