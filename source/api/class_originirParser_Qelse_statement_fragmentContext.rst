.. index:: pair: class; originirParser::Qelse_statement_fragmentContext
.. _doxid-classoriginir_parser_1_1_qelse__statement__fragment_context:

class originirParser::Qelse_statement_fragmentContext
=====================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Qelse_statement_fragmentContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Qelse_statement_fragmentContext<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1a85c60c47e4e3de618d5f24073acc9361>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1a2f36fbb8bdb89e78879c7188fe7c4248>`() const;
		antlr4::tree::TerminalNode* :target:`ELSE_KEY<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1a9a243e5f84fbd453836ff8c95f96ff39>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1af93e36c64be7d3a59168cc9b6fa74550>`();
		std::vector<:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`*> :target:`statement<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1a0e91e54de62357d8182e150b87fbbf49>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1a9aca0d95b0d06f5804b4a24edfc019be>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1a37ad862b4b114cfd48c0ee544bf6eb02>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1a3fb9c257b2ff8edb4a78014d1b2890a4>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context_1aa8aafaa3332b9385b8f11671c58c02db>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
