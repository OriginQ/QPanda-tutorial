.. index:: pair: class; qasmParser::ArgumentContext
.. _doxid-classqasm_parser_1_1_argument_context:

class qasmParser::ArgumentContext
=================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class ArgumentContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`ArgumentContext<doxid-classqasm_parser_1_1_argument_context_1afce7f418fa55d58241d1429c40d5811e>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_argument_context_1aa1dcd1cd45e66d4c1b60b58692ab385c>`() const;
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_argument_context_1a4391dc2ad7913d7efba795008aa007a9>`();
		antlr4::tree::TerminalNode* :target:`LBRACKET<doxid-classqasm_parser_1_1_argument_context_1a0123e79d4b96570008fdf885f9aec489>`();
		:ref:`IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* :target:`integer<doxid-classqasm_parser_1_1_argument_context_1ad8c6f34844cf480ce7c86125b8598bff>`();
		antlr4::tree::TerminalNode* :target:`RBRACKET<doxid-classqasm_parser_1_1_argument_context_1af8c96b30c6d311c5f5142b70a8f81766>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_argument_context_1a0bd422ef9c1e03ba0dd101e26488cebb>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_argument_context_1a82931952acedb3f977cf960ea28ca932>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_argument_context_1a352fffefb390f3c9fed4fa042436459c>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
