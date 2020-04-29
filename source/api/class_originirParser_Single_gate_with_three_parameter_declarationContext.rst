.. index:: pair: class; originirParser::Single_gate_with_three_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context:

class originirParser::Single_gate_with_three_parameter_declarationContext
=========================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_three_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_three_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a935cf0845bac7313eb6f3a9d7f3819df>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1acf7628441e42cacba6f873e302b0b12d>`() const;
		:ref:`Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context>`* :target:`single_gate_with_three_parameter_type<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a5e210be6159e21ad0d3a11057615768e>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1adf327832148f65df69bd7e755b6320aa>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a222429eab4b03fd2dffe298fb7db9e56>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1aa4c9d8b57ee5d0dc0159226ec58c1d87>`(size_t i);
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1aaa63d9d56375a33f8574b218acb055aa>`();
		std::vector<:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`*> :target:`expression<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a095d979e3d0bddc3a0c532e18f6594ec>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a85cc590a50ffcf0bb5ca7a44a12425b7>`(size_t i);
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a8d7547bef3312470b0af66663dd785f3>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a4a944c3383f91f45126a9fb09fd74c03>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1a4d68d14a4f42ae197c5058c93ce67a4f>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context_1aba5f35b0db69af1e6802749f0a3f6d83>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
