.. index:: pair: class; originirParser::Logical_or_expressionContext
.. _doxid-classoriginir_parser_1_1_logical__or__expression_context:

class originirParser::Logical_or_expressionContext
==================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Logical_or_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context_1aa2137d8ffda3cfe82e654b56ec2f411e>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_logical__or__expression_context_1ad0ef4c3de6b8a861bdfb7eb88670fdb2>`() const;
		:ref:`Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`* :target:`logical_and_expression<doxid-classoriginir_parser_1_1_logical__or__expression_context_1a61f8efb4841704cd81085f5bb9779cec>`();
		Logical_or_expressionContext* :target:`logical_or_expression<doxid-classoriginir_parser_1_1_logical__or__expression_context_1a1ec053581c482b6709fa251ed371326d>`();
		antlr4::tree::TerminalNode* :target:`OR<doxid-classoriginir_parser_1_1_logical__or__expression_context_1a63bc6485e23b0cee9ffda410a0989e0c>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_logical__or__expression_context_1a55e8fde0677850ca1098eb4a2688ae62>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_logical__or__expression_context_1af2fa04b3b51994ba059797463011e587>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_logical__or__expression_context_1a53e4f7a0908011c782558d07a6239030>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
