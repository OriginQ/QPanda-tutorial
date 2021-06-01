.. index:: pair: class; qasmParser::RealContext
.. _doxid-classqasm_parser_1_1_real_context:

class qasmParser::RealContext
=============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class RealContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`RealContext<doxid-classqasm_parser_1_1_real_context_1a432dbb0ed279ba6b1c50a68a6d5640ac>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_real_context_1a9b47146cd6aa4c715fd939c13735bd7f>`() const;
		antlr4::tree::TerminalNode* :target:`REALEXP<doxid-classqasm_parser_1_1_real_context_1a2b6fce8f5d0bfaaf17fb0c8525f68283>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_real_context_1a82ce2c0762eabb060423735b55d3954e>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_real_context_1a88b9e7d6c0ee6db83ae057c8a37188b5>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_real_context_1a693d6ee2a6e5faf49588cfaf9af8b540>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
