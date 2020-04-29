.. index:: pair: class; originirParser::Pri_exprContext
.. _doxid-classoriginir_parser_1_1_pri__expr_context:

class originirParser::Pri_exprContext
=====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Pri_exprContext: public :ref:`originirParser::Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`
	{
	public:
		// construction
	
		:target:`Pri_exprContext<doxid-classoriginir_parser_1_1_pri__expr_context_1ac7f33d69d6c184c26a7ffa6289fead03>`(:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* ctx);

		// methods
	
		std::vector<antlr4::tree::TerminalNode*> :target:`LPAREN<doxid-classoriginir_parser_1_1_pri__expr_context_1a81ca306c43059d9c85393adc3f872a0a>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_pri__expr_context_1a627493f6c9956d51e40b9ec4e40a2ea6>`(size_t i);
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_pri__expr_context_1a5c5fa2ca98978a98d48c8d8cbe2dd349>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_pri__expr_context_1a8a115772684bff9a81cac2a93a6fd045>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_pri__expr_context_1a9da27cedbf3037744540c02aa70fa81c>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_pri__expr_context_1a11c06068a0f006dc15b8782472b0a9a2>`(antlr4::tree::ParseTreeVisitor* visitor);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		void :ref:`copyFrom<doxid-classoriginir_parser_1_1_primary__expression_context_1aac335f00cc8b3a5c4f4831663e672850>`(:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* context);
		virtual size_t :ref:`getRuleIndex<doxid-classoriginir_parser_1_1_primary__expression_context_1a11fc39c65fe7cd7a38aacf26d18bddcc>`() const;

