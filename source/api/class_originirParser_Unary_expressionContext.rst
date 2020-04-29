.. index:: pair: class; originirParser::Unary_expressionContext
.. _doxid-classoriginir_parser_1_1_unary__expression_context:

class originirParser::Unary_expressionContext
=============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Unary_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Unary_expressionContext<doxid-classoriginir_parser_1_1_unary__expression_context_1aa9fc29440110f310e6ecbd6a365d95c1>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_unary__expression_context_1a4b4d4a8b1a92dd8c7aad58a24a9fdac0>`() const;
		:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* :target:`primary_expression<doxid-classoriginir_parser_1_1_unary__expression_context_1a1961f1f7649240d09f3f4a4a2e169d8f>`();
		antlr4::tree::TerminalNode* :target:`PLUS<doxid-classoriginir_parser_1_1_unary__expression_context_1a3204838b4048fb57bc2cec3418df885c>`();
		antlr4::tree::TerminalNode* :target:`MINUS<doxid-classoriginir_parser_1_1_unary__expression_context_1a947b476745fb40b840ef45710a7573c9>`();
		antlr4::tree::TerminalNode* :target:`NOT<doxid-classoriginir_parser_1_1_unary__expression_context_1a1745b73a76a141200cac868dec2577a8>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_unary__expression_context_1ad4621259aff21aef7574e35d6f607905>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_unary__expression_context_1ad7d7ea217a73dc6e82c8d68002fd8d8a>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_unary__expression_context_1ac6b1c21171d6ed9e134986ad1f6c23c6>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
