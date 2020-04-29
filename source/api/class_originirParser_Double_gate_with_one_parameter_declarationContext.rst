.. index:: pair: class; originirParser::Double_gate_with_one_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context:

class originirParser::Double_gate_with_one_parameter_declarationContext
=======================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Double_gate_with_one_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Double_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a12d2095b8794c0a313d0237d08bc52ea>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1ac6d59c406a891d0b407394bcea7c6167>`() const;
		:ref:`Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context>`* :target:`double_gate_with_one_parameter_type<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1ab92af2337e40714507da39a480e39a90>`();
		std::vector<:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`*> :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a6cf62d6af8e29e0a65df34f7054c8c6e>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a2436e20aaa4d826277e514a37703d46f>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a6242c4f104471144c39bec5639786302>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1ac9f7a59d996466ba3fba13974bd351af>`(size_t i);
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a69a7063df226a838330f42e76d4b24fe>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a1b6a4dfb0a7aadf2d2749862c0a7c2b9>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a18305837959138415944108a4fd7ab3e>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1ac665fc0c2053339111b6cc470ecbbac4>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1a388cb6c949eac8a2b361f7624ec5b7c2>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context_1aac5b8a4953d083288f287cb83771d6fa>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
