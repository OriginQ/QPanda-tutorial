.. index:: pair: class; originirParser::ConstantContext
.. _doxid-classoriginir_parser_1_1_constant_context:

class originirParser::ConstantContext
=====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class ConstantContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`ConstantContext<doxid-classoriginir_parser_1_1_constant_context_1ad3d17436a2f052cfa2d17f7b9a2de896>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_constant_context_1a8d28e525cbe628907acfff27a66d1bd6>`() const;
		antlr4::tree::TerminalNode* :target:`Integer_Literal<doxid-classoriginir_parser_1_1_constant_context_1a4679983a37b561878fcbdcbee4ab19dd>`();
		antlr4::tree::TerminalNode* :target:`Double_Literal<doxid-classoriginir_parser_1_1_constant_context_1ad338527d08fc524a951b082b4333e766>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_constant_context_1aa40737df7e40d077a9eca45e5bc79e29>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_constant_context_1a946c8142e36d890b1deaf413817945b9>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_constant_context_1a743b3f7a08272e0f1d982f4693cf1872>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
