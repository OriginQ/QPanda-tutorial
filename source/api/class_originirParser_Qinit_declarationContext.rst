.. index:: pair: class; originirParser::Qinit_declarationContext
.. _doxid-classoriginir_parser_1_1_qinit__declaration_context:

class originirParser::Qinit_declarationContext
==============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Qinit_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Qinit_declarationContext<doxid-classoriginir_parser_1_1_qinit__declaration_context_1af3b4bc9b5143c9a00f16f371e7d4ec59>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_qinit__declaration_context_1a9418311ada74ce323003fef8891f48b8>`() const;
		antlr4::tree::TerminalNode* :target:`QINIT_KEY<doxid-classoriginir_parser_1_1_qinit__declaration_context_1a41e17920a1d9d9e4eeca5cbaeecae899>`();
		antlr4::tree::TerminalNode* :target:`Integer_Literal<doxid-classoriginir_parser_1_1_qinit__declaration_context_1a1150cada813f0382f3dc67efb6652800>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_qinit__declaration_context_1a5469a99c48b5c078ea353ab5359ca711>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_qinit__declaration_context_1a8bc82f0bd21e9b6e65769d0d44914c09>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_qinit__declaration_context_1ab373ad8a2b8d115093f034b1a152ab12>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_qinit__declaration_context_1a48b61da2dd1c04cf74721282f1bee366>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
