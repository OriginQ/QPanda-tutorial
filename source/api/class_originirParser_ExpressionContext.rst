.. index:: pair: class; originirParser::ExpressionContext
.. _doxid-classoriginir_parser_1_1_expression_context:

class originirParser::ExpressionContext
=======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class ExpressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context_1a414d1c378e0ee8cb108c2e7661b0532b>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_expression_context_1a0fcea7e8885a6a36427b82eb4a931745>`() const;
		:ref:`Assignment_expressionContext<doxid-classoriginir_parser_1_1_assignment__expression_context>`* :target:`assignment_expression<doxid-classoriginir_parser_1_1_expression_context_1af70941d8408fbece54431cf50ecea0e8>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_expression_context_1a06d327a2161cd2306f1a810e608fcd0f>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_expression_context_1afa12cc555a90f430dfdddc97eabe13a0>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_expression_context_1aee52c8556f9c3eb9d5a45ec7a8049fb3>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
