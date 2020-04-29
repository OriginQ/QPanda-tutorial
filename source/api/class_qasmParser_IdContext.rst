.. index:: pair: class; qasmParser::IdContext
.. _doxid-classqasm_parser_1_1_id_context:

class qasmParser::IdContext
===========================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class IdContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`IdContext<doxid-classqasm_parser_1_1_id_context_1aab4fadaf7ce8ad912c4c5ca32b0e4752>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_id_context_1a435cd0c6107a826ed154e401f33b2361>`() const;
		antlr4::tree::TerminalNode* :target:`IDENTIFIER<doxid-classqasm_parser_1_1_id_context_1a5fbcb8c9aa448a30d152bcc96081ef66>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_id_context_1a518ff15755b0239b83d61db82a61e037>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_id_context_1af410da5eb1a0469f8bb8c5fc7a2397b4>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_id_context_1a9fc3ca54cd20f71f0c1eaa11fc0c2b3c>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
