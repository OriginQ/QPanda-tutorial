.. index:: pair: class; qasmParser::IntegerContext
.. _doxid-classqasm_parser_1_1_integer_context:

class qasmParser::IntegerContext
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class IntegerContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`IntegerContext<doxid-classqasm_parser_1_1_integer_context_1ae3dcb1bdf43a876e130512cbf1810c37>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_integer_context_1a771deed00e269f4bc3c8c52010d4304a>`() const;
		antlr4::tree::TerminalNode* :target:`INTEGER<doxid-classqasm_parser_1_1_integer_context_1a4d956e95f69edbe204c4be7e255a6aab>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_integer_context_1a6561085ce5976a88c2a3a329766295c1>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_integer_context_1a71669a9ca6bcbc5876079ca955cf680f>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_integer_context_1a70ffa3b4c2e72066f30d4e21939ac90f>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
