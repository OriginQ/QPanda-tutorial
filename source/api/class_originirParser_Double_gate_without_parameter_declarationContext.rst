.. index:: pair: class; originirParser::Double_gate_without_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context:

class originirParser::Double_gate_without_parameter_declarationContext
======================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Double_gate_without_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Double_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1ac1a13fc8d415fd7dfc6ece0fc6b26658>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1ae039c188d527950ff583228a28b0ba14>`() const;
		:ref:`Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context>`* :target:`double_gate_without_parameter_type<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1a33909cc6fc7bc22d2cea8c71587d646f>`();
		std::vector<:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`*> :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1a2e5c75cf1ab6169266b1b664e72e4312>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1af45ccf659cc24526a4109671fe1b7ab1>`(size_t i);
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1abf3de43deb04008278639ded7f963ed1>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1a85b617f80fdf9d69dc9cbf0456a656bd>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1ab938378ff02bc75b3c6db253c686dc58>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context_1a3ecf25f74b1a857b34a48bedf99c0d30>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
