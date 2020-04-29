.. index:: pair: class; qasmParser::DecimalContext
.. _doxid-classqasm_parser_1_1_decimal_context:

class qasmParser::DecimalContext
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class DecimalContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`DecimalContext<doxid-classqasm_parser_1_1_decimal_context_1a49f936631de4dc754b0800327e673e82>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_decimal_context_1a33f3a78b9b1115cfdce86c48b2edfe05>`() const;
		antlr4::tree::TerminalNode* :target:`DECIMAL<doxid-classqasm_parser_1_1_decimal_context_1ab2aad5be75da88b66c2868da47c467dc>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_decimal_context_1a57a224bc626c9e839a2334b6e881dcdd>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_decimal_context_1abdea7f6656846454d7638663956f49fb>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_decimal_context_1aa9640a90ffcb70712f88c06dcf1a260e>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
