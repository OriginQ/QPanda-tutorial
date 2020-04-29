.. index:: pair: class; originirParser::Equality_expressionContext
.. _doxid-classoriginir_parser_1_1_equality__expression_context:

class originirParser::Equality_expressionContext
================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Equality_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context_1abfd999287eebd7630e6b692a88d4c0c3>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_equality__expression_context_1aeb46f75154411d186ac86d3635898a71>`() const;
		:ref:`Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`* :target:`relational_expression<doxid-classoriginir_parser_1_1_equality__expression_context_1a77430fe00dd96e86f599fcdd3415531e>`();
		Equality_expressionContext* :target:`equality_expression<doxid-classoriginir_parser_1_1_equality__expression_context_1aa643f38318d378a6245c4c9f1df3d41c>`();
		antlr4::tree::TerminalNode* :target:`EQ<doxid-classoriginir_parser_1_1_equality__expression_context_1ac7e428976e0ee680555ca3e77cbb48c1>`();
		antlr4::tree::TerminalNode* :target:`NE<doxid-classoriginir_parser_1_1_equality__expression_context_1aee048d62257260d8ed563ea5901a4a26>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_equality__expression_context_1a9ecb346f5052631833c3f62d6b477292>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_equality__expression_context_1a471e03ce70c5800b4ffe27e0cf0c9719>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_equality__expression_context_1a8243a192292524c9c4b4d7ab74b68166>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
