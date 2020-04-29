.. index:: pair: class; originirParser::Single_gate_with_four_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context:

class originirParser::Single_gate_with_four_parameter_declarationContext
========================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_four_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1ad506555be666d6f20882b686d4214a3b>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1a7b297b9bd6875c1cc5b24d1d862081e4>`() const;
		:ref:`Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context>`* :target:`single_gate_with_four_parameter_type<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1ab5457a8eb5174d5a31639881ef2dd5c7>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1a7926b339db7ac731ea5791370cb757fc>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1a42b3ab22af0052fec6960e00471c8f38>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1abe40ff86a79712c08f4a9cb0ab9ac50e>`(size_t i);
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1a9d95c738738a8e8a76db9fc5cc1e201c>`();
		std::vector<:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`*> :target:`expression<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1aab9db203de958ed4335d79a64772bec7>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1a53a8766d5615ceedbd034b77d1843d15>`(size_t i);
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1ab2d3a5025ecd7de39e4df84c8b908377>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1aad1feb65fc58a4afbad4c500e8846fb1>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1a298460632d4f78cd33d6faaf151da2b6>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context_1aca2cc5da2e42a86f91dded5273fa95bf>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
