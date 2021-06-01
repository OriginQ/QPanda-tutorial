.. index:: pair: class; originirParser::Define_gate_declarationContext
.. _doxid-classoriginir_parser_1_1_define__gate__declaration_context:

class originirParser::Define_gate_declarationContext
====================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Define_gate_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Define_gate_declarationContext<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1aa7809dc954bdcb46248c5a668e4559fd>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1a74bb66117d200dbd95b729d8723aa103>`() const;
		:ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`* :target:`id<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1ae6403168d25542e3d4d8b25ae37e63eb>`();
		std::vector<:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`*> :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1ab7de9f4c1eb3b9b9df685f8f317d3101>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1ac6b08362a6a3968b9ee8935685962c4f>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1a19428ac74bee524a5c6e50323317f48a>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1ae1f198e1f4350d62d246660aa11097fb>`(size_t i);
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1a92071bc733613eb462209be7e2f881c4>`();
		std::vector<:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`*> :target:`expression<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1a7bde0170879fcb36bc6fce3398c2de39>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1a6cba348132d8db3a8ae01febfbb7fcb4>`(size_t i);
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1a860787af2faffcc8df51f96d2e5b08c8>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1acb0d1abeeecbfa6044906eaaf27a07be>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1ad71bb416c0ebed1102ea33aa629f0735>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_define__gate__declaration_context_1a750e8760527718f24f023c2e9a5f82a2>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
