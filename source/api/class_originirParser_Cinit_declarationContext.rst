.. index:: pair: class; originirParser::Cinit_declarationContext
.. _doxid-classoriginir_parser_1_1_cinit__declaration_context:

class originirParser::Cinit_declarationContext
==============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Cinit_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Cinit_declarationContext<doxid-classoriginir_parser_1_1_cinit__declaration_context_1a86345dbe17b2d1584180b5a295ac435b>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_cinit__declaration_context_1af9c61d031d43caf8ec4de62736254505>`() const;
		antlr4::tree::TerminalNode* :target:`CREG_KEY<doxid-classoriginir_parser_1_1_cinit__declaration_context_1a363803b5311a61901593757ed017fda4>`();
		antlr4::tree::TerminalNode* :target:`Integer_Literal<doxid-classoriginir_parser_1_1_cinit__declaration_context_1aedf5dc869f300ef7f5fb896473f1d95b>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_cinit__declaration_context_1a8e3a78c8ec97ebc79521b973802a8873>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_cinit__declaration_context_1a7d445d91673748b79f8210994e8cbaae>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_cinit__declaration_context_1ab96d2c94cb7d676d28a5ad50c50e36a0>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_cinit__declaration_context_1a1d2e55d821c956448e3e5c82c061b059>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
