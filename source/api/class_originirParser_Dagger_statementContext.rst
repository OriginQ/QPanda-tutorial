.. index:: pair: class; originirParser::Dagger_statementContext
.. _doxid-classoriginir_parser_1_1_dagger__statement_context:

class originirParser::Dagger_statementContext
=============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Dagger_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Dagger_statementContext<doxid-classoriginir_parser_1_1_dagger__statement_context_1a8fd0b485d2b2c08325a63c63dc829dc5>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_dagger__statement_context_1ae91e2178f6b76d6e000446c22966ccc3>`() const;
		antlr4::tree::TerminalNode* :target:`DAGGER_KEY<doxid-classoriginir_parser_1_1_dagger__statement_context_1a4ac355369fcae6d9944dcb97a7394213>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`NEWLINE<doxid-classoriginir_parser_1_1_dagger__statement_context_1ac9e80728a4ed36b22f070a0c9b90d789>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_dagger__statement_context_1a0de6f88b04a56bab5a0e190027d9c0df>`(size_t i);
		antlr4::tree::TerminalNode* :target:`ENDDAGGER_KEY<doxid-classoriginir_parser_1_1_dagger__statement_context_1a966d551c6111c4137194309c1f82a779>`();
		std::vector<:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`*> :target:`statement<doxid-classoriginir_parser_1_1_dagger__statement_context_1a136f9fd14fc4a1683d1f1111a6cf1adf>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1_1_dagger__statement_context_1a4d4d9f66f5c291efc8004b53a6177712>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_dagger__statement_context_1a5a5b53e5dbb7225043e7dcf006a95490>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_dagger__statement_context_1a2ab82dd33542844f0cbcd37eb0e7df30>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_dagger__statement_context_1ad497d35624292cef87d062566ae71202>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
