.. index:: pair: class; originirBaseVisitor
.. _doxid-classoriginir_base_visitor:

class originirBaseVisitor
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

This class provides an empty implementation of :ref:`originirVisitor <doxid-classoriginir_visitor>`, which can be extended to create a visitor which only needs to handle a subset of the available methods. :ref:`More...<details-classoriginir_base_visitor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirBaseVisitor.h>
	
	class originirBaseVisitor: public :ref:`originirVisitor<doxid-classoriginir_visitor>`
	{
	public:
		// methods
	
		virtual antlrcpp::Any :ref:`visitTranslationunit<doxid-classoriginir_base_visitor_1a14cc8955d38c3ba8a4a095e80c98d561>`(:ref:`originirParser::TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context>`* context);
		virtual antlrcpp::Any :target:`visitDeclaration<doxid-classoriginir_base_visitor_1ad17f334e1fa8089a6474a8f7429df364>`(:ref:`originirParser::DeclarationContext<doxid-classoriginir_parser_1_1_declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQinit_declaration<doxid-classoriginir_base_visitor_1a2f67884dacd237cdbad7c0f62ab71f11>`(:ref:`originirParser::Qinit_declarationContext<doxid-classoriginir_parser_1_1_qinit__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitCinit_declaration<doxid-classoriginir_base_visitor_1afdd576aaa3de32107bb52acb2cfbd5b3>`(:ref:`originirParser::Cinit_declarationContext<doxid-classoriginir_parser_1_1_cinit__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQuantum_gate_declaration<doxid-classoriginir_base_visitor_1a6c129efb98bec5cf98017acd83bb3ba5>`(:ref:`originirParser::Quantum_gate_declarationContext<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitIndex<doxid-classoriginir_base_visitor_1ae907bb6425faf391f2f6fffc95034936>`(:ref:`originirParser::IndexContext<doxid-classoriginir_parser_1_1_index_context>`* ctx);
		virtual antlrcpp::Any :target:`visitC_KEY_declaration<doxid-classoriginir_base_visitor_1a2ee2891cf21a468521ba2fb35ecee07f>`(:ref:`originirParser::C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQ_KEY_declaration<doxid-classoriginir_base_visitor_1a7415df4a51c5949507a16d54aac4ed48>`(:ref:`originirParser::Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_without_parameter_declaration<doxid-classoriginir_base_visitor_1ab04f96f474d207aeaa8f1c3b0072a61d>`(:ref:`originirParser::Single_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_one_parameter_declaration<doxid-classoriginir_base_visitor_1a73b95d3caab0fc9e730377a7f02c9fea>`(:ref:`originirParser::Single_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_two_parameter_declaration<doxid-classoriginir_base_visitor_1a2c40156df2a2aebf8d1007a95e9b5d3d>`(:ref:`originirParser::Single_gate_with_two_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_three_parameter_declaration<doxid-classoriginir_base_visitor_1a8b1a6bd6a2700ed1f2fbb32be6274c3b>`(:ref:`originirParser::Single_gate_with_three_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_four_parameter_declaration<doxid-classoriginir_base_visitor_1afed22a63dcc0d0856cc991a5df7df798>`(:ref:`originirParser::Single_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDouble_gate_without_parameter_declaration<doxid-classoriginir_base_visitor_1af9d911eb4321afa6838a6e860e1b2424>`(:ref:`originirParser::Double_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDouble_gate_with_one_parameter_declaration<doxid-classoriginir_base_visitor_1a4f4b2d1090d727cc10eb2b2b968bd543>`(:ref:`originirParser::Double_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDouble_gate_with_four_parameter_declaration<doxid-classoriginir_base_visitor_1a3fdc8860ebf6cbab204f62cb6ff73c93>`(:ref:`originirParser::Double_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitTriple_gate_without_parameter_declaration<doxid-classoriginir_base_visitor_1ae80cb67db6aae613a8026a06f6581f1e>`(:ref:`originirParser::Triple_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_without_parameter_type<doxid-classoriginir_base_visitor_1ad6f8a2b3235673fa77ad1bf492fb3428>`(:ref:`originirParser::Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_one_parameter_type<doxid-classoriginir_base_visitor_1a7468df28afc0cc9e51822429f162eb46>`(:ref:`originirParser::Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_two_parameter_type<doxid-classoriginir_base_visitor_1a05966ebfa9d9f1543830442a48fd16dc>`(:ref:`originirParser::Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_three_parameter_type<doxid-classoriginir_base_visitor_1a6b73b4cd1e3686e78445cc705a53c916>`(:ref:`originirParser::Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitSingle_gate_with_four_parameter_type<doxid-classoriginir_base_visitor_1a354d31e76df2454149d0cdb23ca77369>`(:ref:`originirParser::Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDouble_gate_without_parameter_type<doxid-classoriginir_base_visitor_1aa74b871e05f88fbcf98bc31f8f86b4fe>`(:ref:`originirParser::Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDouble_gate_with_one_parameter_type<doxid-classoriginir_base_visitor_1a0d875ca79afabda0a6f22cbe8d4f3336>`(:ref:`originirParser::Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDouble_gate_with_four_parameter_type<doxid-classoriginir_base_visitor_1a14d2591877ff2a021f4c2222f7cd430d>`(:ref:`originirParser::Double_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitTriple_gate_without_parameter_type<doxid-classoriginir_base_visitor_1a0a4a164a2fb0f88bfd321761370e6171>`(:ref:`originirParser::Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context>`* ctx);
		virtual antlrcpp::Any :target:`visitPri_ckey<doxid-classoriginir_base_visitor_1afe5aaf30b01df8f992d89dd1ac88d6a0>`(:ref:`originirParser::Pri_ckeyContext<doxid-classoriginir_parser_1_1_pri__ckey_context>`* ctx);
		virtual antlrcpp::Any :target:`visitPri_cst<doxid-classoriginir_base_visitor_1a978a64cf274cb44e6d4907faafba2568>`(:ref:`originirParser::Pri_cstContext<doxid-classoriginir_parser_1_1_pri__cst_context>`* ctx);
		virtual antlrcpp::Any :target:`visitPri_expr<doxid-classoriginir_base_visitor_1abddfe62c74fa1bf487ee5c1c1be6bcd3>`(:ref:`originirParser::Pri_exprContext<doxid-classoriginir_parser_1_1_pri__expr_context>`* ctx);
		virtual antlrcpp::Any :target:`visitUnary_expression<doxid-classoriginir_base_visitor_1a9d225ce0e75ae584891923c720617cc3>`(:ref:`originirParser::Unary_expressionContext<doxid-classoriginir_parser_1_1_unary__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitMultiplicative_expression<doxid-classoriginir_base_visitor_1a5f9f66d084d7c304e3951f3257a0e056>`(:ref:`originirParser::Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitAddtive_expression<doxid-classoriginir_base_visitor_1abfd75c91644787622a00bb5b6df1c614>`(:ref:`originirParser::Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitRelational_expression<doxid-classoriginir_base_visitor_1af97f12b486c3932558867ffc31d12acc>`(:ref:`originirParser::Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitEquality_expression<doxid-classoriginir_base_visitor_1a92bfcf9a858d089d2aba292946c4a503>`(:ref:`originirParser::Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitLogical_and_expression<doxid-classoriginir_base_visitor_1a8ca12ae81247c282f39ba7a177fca906>`(:ref:`originirParser::Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitLogical_or_expression<doxid-classoriginir_base_visitor_1ae679f3ae5c213a135342116c7ab81c8c>`(:ref:`originirParser::Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitAssignment_expression<doxid-classoriginir_base_visitor_1ae32269ed199c13f6d0e41725935b64e7>`(:ref:`originirParser::Assignment_expressionContext<doxid-classoriginir_parser_1_1_assignment__expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitExpression<doxid-classoriginir_base_visitor_1a5ca705d4b519e7a22e2e767f386e26b9>`(:ref:`originirParser::ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* ctx);
		virtual antlrcpp::Any :target:`visitControlbit_list<doxid-classoriginir_base_visitor_1a82f34edf13f703bb7111b4d0e5b6edda>`(:ref:`originirParser::Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context>`* ctx);
		virtual antlrcpp::Any :target:`visitStatement<doxid-classoriginir_base_visitor_1add6285a2761f96d6cac0955a92c1150a>`(:ref:`originirParser::StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitDagger_statement<doxid-classoriginir_base_visitor_1a7f250e7b9429e94127eab8e0e2353105>`(:ref:`originirParser::Dagger_statementContext<doxid-classoriginir_parser_1_1_dagger__statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitControl_statement<doxid-classoriginir_base_visitor_1a2b1a0120b24ff0006e9621ab4a4aca19>`(:ref:`originirParser::Control_statementContext<doxid-classoriginir_parser_1_1_control__statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQelse_statement_fragment<doxid-classoriginir_base_visitor_1afbd32242b383ea486792a80e1f8169dd>`(:ref:`originirParser::Qelse_statement_fragmentContext<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQif_if<doxid-classoriginir_base_visitor_1a64a6422da91f9fb9faafe5816be66602>`(:ref:`originirParser::Qif_ifContext<doxid-classoriginir_parser_1_1_qif__if_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQif_ifelse<doxid-classoriginir_base_visitor_1a7d0a8177e1c5e7f92cfb66aa12c990a3>`(:ref:`originirParser::Qif_ifelseContext<doxid-classoriginir_parser_1_1_qif__ifelse_context>`* ctx);
		virtual antlrcpp::Any :target:`visitQwhile_statement<doxid-classoriginir_base_visitor_1aa637f71f65963c2977deef69abfba718>`(:ref:`originirParser::Qwhile_statementContext<doxid-classoriginir_parser_1_1_qwhile__statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitMeasure_statement<doxid-classoriginir_base_visitor_1aa6e8af30b9e7e956f4f2cdfad8e5fa9c>`(:ref:`originirParser::Measure_statementContext<doxid-classoriginir_parser_1_1_measure__statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitReset_statement<doxid-classoriginir_base_visitor_1acefa583e2d9f550c2dbaeb02d2b54bc1>`(:ref:`originirParser::Reset_statementContext<doxid-classoriginir_parser_1_1_reset__statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitExpression_statement<doxid-classoriginir_base_visitor_1a0d499fff0219c95cd2ea5eb91d612d27>`(:ref:`originirParser::Expression_statementContext<doxid-classoriginir_parser_1_1_expression__statement_context>`* ctx);
		virtual antlrcpp::Any :target:`visitConstant<doxid-classoriginir_base_visitor_1a640d6f56a0e65420d973b67618e8c911>`(:ref:`originirParser::ConstantContext<doxid-classoriginir_parser_1_1_constant_context>`* ctx);
	};

	// direct descendants

	class :ref:`OriginIRVisitor<doxid-class_q_panda_1_1_origin_i_r_visitor>`;

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual antlrcpp::Any :ref:`visitTranslationunit<doxid-classoriginir_visitor_1afabf405697abbff4744d8e30e9dce7bc>`(:ref:`originirParser::TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDeclaration<doxid-classoriginir_visitor_1abb80f1743facd0c41a0eafbade8fbefb>`(:ref:`originirParser::DeclarationContext<doxid-classoriginir_parser_1_1_declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQinit_declaration<doxid-classoriginir_visitor_1ae1482d0a0054f467be39ad865cbac93d>`(:ref:`originirParser::Qinit_declarationContext<doxid-classoriginir_parser_1_1_qinit__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitCinit_declaration<doxid-classoriginir_visitor_1a4337389f960db0a4314770c74fe6cfd2>`(:ref:`originirParser::Cinit_declarationContext<doxid-classoriginir_parser_1_1_cinit__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQuantum_gate_declaration<doxid-classoriginir_visitor_1a4558aa4ac5cfcb1d94597d94bbd7c245>`(:ref:`originirParser::Quantum_gate_declarationContext<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitIndex<doxid-classoriginir_visitor_1af4104aeb1a819a096daf45c78b8d4b01>`(:ref:`originirParser::IndexContext<doxid-classoriginir_parser_1_1_index_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitC_KEY_declaration<doxid-classoriginir_visitor_1aa0e79512132fae4d0666e5f5f9328f70>`(:ref:`originirParser::C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQ_KEY_declaration<doxid-classoriginir_visitor_1a67c701c6033a604077d84790ce331cb7>`(:ref:`originirParser::Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_without_parameter_declaration<doxid-classoriginir_visitor_1a207064859ea5a14f04a96e45d045feff>`(:ref:`originirParser::Single_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_one_parameter_declaration<doxid-classoriginir_visitor_1a288ac3dc5e50e19ef5b3c50075a67300>`(:ref:`originirParser::Single_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_two_parameter_declaration<doxid-classoriginir_visitor_1a1238c1457efd1b44a73241b550678204>`(:ref:`originirParser::Single_gate_with_two_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_three_parameter_declaration<doxid-classoriginir_visitor_1a20e8d4c49e44a1d32e852232df9a6a99>`(:ref:`originirParser::Single_gate_with_three_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_four_parameter_declaration<doxid-classoriginir_visitor_1a715006a175402c3687b81a824d48f91b>`(:ref:`originirParser::Single_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDouble_gate_without_parameter_declaration<doxid-classoriginir_visitor_1a330ff4f28a1b8b9a49587567bac80fd8>`(:ref:`originirParser::Double_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDouble_gate_with_one_parameter_declaration<doxid-classoriginir_visitor_1a94f72e10a20134d865036113bac9c454>`(:ref:`originirParser::Double_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDouble_gate_with_four_parameter_declaration<doxid-classoriginir_visitor_1a6b35d772a224894b5a6acab1e3c3b80c>`(:ref:`originirParser::Double_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitTriple_gate_without_parameter_declaration<doxid-classoriginir_visitor_1a650ba14d421b0fc96f1ee8aac39af4df>`(:ref:`originirParser::Triple_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_without_parameter_type<doxid-classoriginir_visitor_1a2b2d973981441bb17e7d575106f22252>`(:ref:`originirParser::Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_one_parameter_type<doxid-classoriginir_visitor_1a774b6f00bfb4721574e9d2ff8c5d04ef>`(:ref:`originirParser::Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_two_parameter_type<doxid-classoriginir_visitor_1a46bd8a9a9f01652d6d3a39f81fff2cb8>`(:ref:`originirParser::Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_three_parameter_type<doxid-classoriginir_visitor_1a3d1d35bfec5bb10234ff3dc540389c30>`(:ref:`originirParser::Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitSingle_gate_with_four_parameter_type<doxid-classoriginir_visitor_1a6344a834440e372c72a93d4111e03a4f>`(:ref:`originirParser::Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDouble_gate_without_parameter_type<doxid-classoriginir_visitor_1ae92b1b5816bbf9cb56bb197aa4c6c508>`(:ref:`originirParser::Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDouble_gate_with_one_parameter_type<doxid-classoriginir_visitor_1acd0e38df429ed0ddf1e212d27d54aced>`(:ref:`originirParser::Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDouble_gate_with_four_parameter_type<doxid-classoriginir_visitor_1aec75cbd82197f4ce3f49ce4b35db8262>`(:ref:`originirParser::Double_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitTriple_gate_without_parameter_type<doxid-classoriginir_visitor_1a99541b3032ebf22df1a2588aa2184a9b>`(:ref:`originirParser::Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitPri_ckey<doxid-classoriginir_visitor_1aa0536a564fefdc47148aed8ca5f64f6b>`(:ref:`originirParser::Pri_ckeyContext<doxid-classoriginir_parser_1_1_pri__ckey_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitPri_cst<doxid-classoriginir_visitor_1a2c167188c3ccfec7358c973315b7b0b8>`(:ref:`originirParser::Pri_cstContext<doxid-classoriginir_parser_1_1_pri__cst_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitPri_expr<doxid-classoriginir_visitor_1ab3ad33baf4acdb03692847f2e4b8d4eb>`(:ref:`originirParser::Pri_exprContext<doxid-classoriginir_parser_1_1_pri__expr_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitUnary_expression<doxid-classoriginir_visitor_1a2df2aea4add7d445c87fc0440a393104>`(:ref:`originirParser::Unary_expressionContext<doxid-classoriginir_parser_1_1_unary__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitMultiplicative_expression<doxid-classoriginir_visitor_1a958ae8cccd94b1d6b78e749e0537a435>`(:ref:`originirParser::Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitAddtive_expression<doxid-classoriginir_visitor_1a1c4c8cbeda0b35d0f8b12145ecd05d33>`(:ref:`originirParser::Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitRelational_expression<doxid-classoriginir_visitor_1a00d18d7b76cfa9d791b4c87581912f7b>`(:ref:`originirParser::Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitEquality_expression<doxid-classoriginir_visitor_1a80cc6eedd7156e3d86bd2a6d66b96186>`(:ref:`originirParser::Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitLogical_and_expression<doxid-classoriginir_visitor_1a67a8c994bb9e58e602bd186f880cf98d>`(:ref:`originirParser::Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitLogical_or_expression<doxid-classoriginir_visitor_1afc9ab3638f609091c41712434ff7a65d>`(:ref:`originirParser::Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitAssignment_expression<doxid-classoriginir_visitor_1a69919dd8fca6babda06bb8a591113b02>`(:ref:`originirParser::Assignment_expressionContext<doxid-classoriginir_parser_1_1_assignment__expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitExpression<doxid-classoriginir_visitor_1a96863a8fad5b282b5e2bc56bc48fb4a0>`(:ref:`originirParser::ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitControlbit_list<doxid-classoriginir_visitor_1aa36bb95f0fa9aba7cfe481d4922a01d5>`(:ref:`originirParser::Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitStatement<doxid-classoriginir_visitor_1a52b586173bfbe017a1cffe1c73b1aed4>`(:ref:`originirParser::StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitDagger_statement<doxid-classoriginir_visitor_1aa79dc2ac1a1b7ff1c85d7ab961fd5e7c>`(:ref:`originirParser::Dagger_statementContext<doxid-classoriginir_parser_1_1_dagger__statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitControl_statement<doxid-classoriginir_visitor_1a677f5b1d33654e76c7e62f1aa9ef846c>`(:ref:`originirParser::Control_statementContext<doxid-classoriginir_parser_1_1_control__statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQelse_statement_fragment<doxid-classoriginir_visitor_1a20f88c103605209420db646adb5666de>`(:ref:`originirParser::Qelse_statement_fragmentContext<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQif_if<doxid-classoriginir_visitor_1a84c35b9037f67fe882b755ace2748825>`(:ref:`originirParser::Qif_ifContext<doxid-classoriginir_parser_1_1_qif__if_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQif_ifelse<doxid-classoriginir_visitor_1a2effd56b537d2ceafbe07c5b79f578e5>`(:ref:`originirParser::Qif_ifelseContext<doxid-classoriginir_parser_1_1_qif__ifelse_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitQwhile_statement<doxid-classoriginir_visitor_1ad57bec937e5cf88af27b31dc8cf1e5f3>`(:ref:`originirParser::Qwhile_statementContext<doxid-classoriginir_parser_1_1_qwhile__statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitMeasure_statement<doxid-classoriginir_visitor_1a2a9575d11bbec345f91d7a54408348e2>`(:ref:`originirParser::Measure_statementContext<doxid-classoriginir_parser_1_1_measure__statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitReset_statement<doxid-classoriginir_visitor_1aea822832627154b0d27abb3461e61dab>`(:ref:`originirParser::Reset_statementContext<doxid-classoriginir_parser_1_1_reset__statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitExpression_statement<doxid-classoriginir_visitor_1abeef7f57a2b1b8e25d9108a68e011191>`(:ref:`originirParser::Expression_statementContext<doxid-classoriginir_parser_1_1_expression__statement_context>`* context) = 0;
		virtual antlrcpp::Any :ref:`visitConstant<doxid-classoriginir_visitor_1a643e97d350ab10b740e5d599ceb3121c>`(:ref:`originirParser::ConstantContext<doxid-classoriginir_parser_1_1_constant_context>`* context) = 0;

.. _details-classoriginir_base_visitor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

This class provides an empty implementation of :ref:`originirVisitor <doxid-classoriginir_visitor>`, which can be extended to create a visitor which only needs to handle a subset of the available methods.

Methods
-------

.. index:: pair: function; visitTranslationunit
.. _doxid-classoriginir_base_visitor_1a14cc8955d38c3ba8a4a095e80c98d561:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual antlrcpp::Any visitTranslationunit(:ref:`originirParser::TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context>`* context)

Visit parse trees produced by :ref:`originirParser <doxid-classoriginir_parser>`.

