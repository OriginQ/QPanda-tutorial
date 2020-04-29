.. index:: pair: class; originirParser::Expression_statementContext
.. _doxid-classoriginir_parser_1_1_expression__statement_context:

class originirParser::Expression_statementContext
=================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Expression_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Expression_statementContext<doxid-classoriginir_parser_1_1_expression__statement_context_1a70b8bdccae6453d31bcf4d884b877824>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_expression__statement_context_1a0d296af7dd3c2fec2c84606c89f25127>`() const;
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_expression__statement_context_1a9ba193d7d74eaf98a91ce58a9a2145e7>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_expression__statement_context_1a5212e1a11317274ca459ffc840d4c303>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_expression__statement_context_1a5f615049f4af0fe4ac5bcfa8111a1348>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_expression__statement_context_1a767690911d5f70846d0fed6040051fd3>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
