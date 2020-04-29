.. index:: pair: class; originirParser::Logical_and_expressionContext
.. _doxid-classoriginir_parser_1_1_logical__and__expression_context:

class originirParser::Logical_and_expressionContext
===================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Logical_and_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context_1ad0cb5c9509e2c936cba5bede0fa525dd>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_logical__and__expression_context_1a75147573a96948877f50b9ea245d5592>`() const;
		:ref:`Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`* :target:`equality_expression<doxid-classoriginir_parser_1_1_logical__and__expression_context_1a9d3987164a3fda2fb08d27b1d59886de>`();
		Logical_and_expressionContext* :target:`logical_and_expression<doxid-classoriginir_parser_1_1_logical__and__expression_context_1a3adaeedc8a98d9c8947015b24beab69d>`();
		antlr4::tree::TerminalNode* :target:`AND<doxid-classoriginir_parser_1_1_logical__and__expression_context_1a76ae1e84a54f42f5a56232826e1098a2>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_logical__and__expression_context_1a436f8aa486eaabbe65053bfecf383414>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_logical__and__expression_context_1a6043102ed70c2b2199d395c23bb578fd>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_logical__and__expression_context_1aadf9c06c5f07e3d414b1a1c4246e34e1>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
