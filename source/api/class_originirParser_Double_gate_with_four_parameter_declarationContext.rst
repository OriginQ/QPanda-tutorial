.. index:: pair: class; originirParser::Double_gate_with_four_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context:

class originirParser::Double_gate_with_four_parameter_declarationContext
========================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Double_gate_with_four_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Double_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1ac5a535b6fc6e80074bab0c4a596f0a8e>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1a54f72d6b5b195464be7ccd59fa432063>`() const;
		:ref:`Double_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__type_context>`* :target:`double_gate_with_four_parameter_type<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1ab40d0788a96eeb31e3336b9a8e4158cd>`();
		std::vector<:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`*> :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1ae25e7b30526a7bfa7e370420807daeac>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1a94cab0ea1561e7a6f5ad4de6a884ac68>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1ab65d3524d469dc15d168186165a8e9b7>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1a2f8a3d81d19e3b3699a7c178a1af012d>`(size_t i);
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1a8e62b2f864e09c181e309b4250cf398e>`();
		std::vector<:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`*> :target:`expression<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1a04017922c631e505bd4027bd6f12a9a4>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1ad2044ec2a22cbbe4796b4daa2b38b8ac>`(size_t i);
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1a914b20433d8552b65b87f89b3be5a772>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1af077bc32dd50fcb597b4f72495dd2bce>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1aaa1c2f33b869efe78ea0e7f10e573a1d>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context_1a22aa426293e20dd70aaccc43a1b3ae09>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
