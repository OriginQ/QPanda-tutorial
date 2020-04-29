.. index:: pair: class; originirParser::Multiplicative_expressionContext
.. _doxid-classoriginir_parser_1_1_multiplicative__expression_context:

class originirParser::Multiplicative_expressionContext
======================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Multiplicative_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1a5cddc8881b3bf3d072d4bc5a4c77865d>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1ab3f9b796e17915d0f654461e3b8569bb>`() const;
		:ref:`Unary_expressionContext<doxid-classoriginir_parser_1_1_unary__expression_context>`* :target:`unary_expression<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1ad69b52d9c0de0a8c88354a2e0dfc0e03>`();
		Multiplicative_expressionContext* :target:`multiplicative_expression<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1a57cd215f62b0b62e439fdb84a3e5026a>`();
		antlr4::tree::TerminalNode* :target:`MUL<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1a87273687a62c873c8504bdbb548bdf7c>`();
		antlr4::tree::TerminalNode* :target:`DIV<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1ab70e814e5fad73b700812ce44a7bd2d2>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1a01605919180ce2c0e662d6f70ccea90a>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1a12fdacf7ee5d947696b4cb489e0567ab>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_multiplicative__expression_context_1a87440e3e826b5839cea60245a0a464af>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
