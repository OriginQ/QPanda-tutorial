.. index:: pair: class; originirParser::Control_statementContext
.. _doxid-classoriginir_parser_1_1_control__statement_context:

class originirParser::Control_statementContext
==============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Control_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Control_statementContext<doxid-classoriginir_parser_1_1_control__statement_context_1aa9a0d6a7815df65d7196abbaa28ebed3>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_control__statement_context_1aa35be979280b7d1cb222d07ee1be7cf9>`() const;
		antlr4::tree::TerminalNode* :target:`CONTROL_KEY<doxid-classoriginir_parser_1_1_control__statement_context_1a14eb55f63024b3715ce87f733c4bcc3a>`();
		:ref:`Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context>`* :target:`controlbit_list<doxid-classoriginir_parser_1_1_control__statement_context_1a246e9cc786df3587a8173848dbdd7453>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`NEWLINE<doxid-classoriginir_parser_1_1_control__statement_context_1af744b247ff03eb977ca2810fcac87a33>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_control__statement_context_1ae7ad9eba49aa1664be84a99cfb5ce7ea>`(size_t i);
		antlr4::tree::TerminalNode* :target:`ENDCONTROL_KEY<doxid-classoriginir_parser_1_1_control__statement_context_1a5e0e308d046a6246f00763acc847e75a>`();
		std::vector<:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`*> :target:`statement<doxid-classoriginir_parser_1_1_control__statement_context_1a9817a0a1350adc13ce39443e04a6e58c>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1_1_control__statement_context_1a0e92143c9c31e0dff602703dbb383363>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_control__statement_context_1a8b2e9044467644dab3e61b6684c6b716>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_control__statement_context_1aec1a38daacadaca05c2ce5cd1f51786a>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_control__statement_context_1a08d86270ae34c731122b6d626f40831e>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
