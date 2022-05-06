.. index:: pair: class; originirParser::Define_gate_statementContext
.. _doxid-classoriginir_parser_1_1_define__gate__statement_context:

class originirParser::Define_gate_statementContext
==================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Define_gate_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Define_gate_statementContext<doxid-classoriginir_parser_1_1_define__gate__statement_context_1a4e050a1ba593ac41c6975b66483ccda7>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_define__gate__statement_context_1a24f8a24444c7ec4c48bb144eb867b20d>`() const;
		:ref:`Gate_nameContext<doxid-classoriginir_parser_1_1_gate__name_context>`* :target:`gate_name<doxid-classoriginir_parser_1_1_define__gate__statement_context_1abd9461b9c4b710bb3e43b8f8533af48e>`();
		:ref:`Id_listContext<doxid-classoriginir_parser_1_1_id__list_context>`* :target:`id_list<doxid-classoriginir_parser_1_1_define__gate__statement_context_1af3cffbf650b2dd4e20864d5c97419838>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_define__gate__statement_context_1af72c405334f8b65dd4e9bfd1b72534de>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_define__gate__statement_context_1a06596c1ffedbfd1cffacf12653412a56>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_define__gate__statement_context_1ad6d90d6bf15c6f1efe23878d6a6ad013>`();
		:ref:`ExplistContext<doxid-classoriginir_parser_1_1_explist_context>`* :target:`explist<doxid-classoriginir_parser_1_1_define__gate__statement_context_1ae55f15eace1652b4caa07d4d5da10555>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_define__gate__statement_context_1a719edfa9eac85fe2cfb46172c4559f55>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_define__gate__statement_context_1ad664418d56eab6ca2262c7ce46ae1de1>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_define__gate__statement_context_1ac523532cdfc7e55c3e5608e2127041f5>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_define__gate__statement_context_1aa78567e5816512d57279d9308aad8ed1>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
