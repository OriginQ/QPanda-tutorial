.. index:: pair: class; originirParser::Single_gate_with_one_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context:

class originirParser::Single_gate_with_one_parameter_declarationContext
=======================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_one_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a489c16da1d93583106b8fb0687dbf889>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a891856ca3ce4d6f8bce0445a25febe97>`() const;
		:ref:`Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context>`* :target:`single_gate_with_one_parameter_type<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a9d14097b1e7a34c075cc12f4cc9b3719>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1afc757d50becbb86b716cd9e8d9a59771>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1ae4b04c6d25d97a1e3359ab56cf5736bc>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a32fd61ae98e2777295ffc0865db6ee7f>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a8e75d55ff58b72f46b5a701b9e4bc56b>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a64c919ffc3dfbc478072496f1dafb843>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1ac27242202b7c04ef498699f40e92ce38>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a7f7b285797d26c10ef6a93d0e5f47173>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context_1a3b33fc6947a1c19fedf5eb6b9f0cde5a>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
