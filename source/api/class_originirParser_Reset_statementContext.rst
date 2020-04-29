.. index:: pair: class; originirParser::Reset_statementContext
.. _doxid-classoriginir_parser_1_1_reset__statement_context:

class originirParser::Reset_statementContext
============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Reset_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Reset_statementContext<doxid-classoriginir_parser_1_1_reset__statement_context_1a53457951364fc0d8d065172a72b2873c>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_reset__statement_context_1a6b6061073f38d48be8141fe0543016c0>`() const;
		antlr4::tree::TerminalNode* :target:`RESET_KEY<doxid-classoriginir_parser_1_1_reset__statement_context_1a11162044d39986099c58dc050b16ea64>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_reset__statement_context_1a93a7950eb8f26985c848693fec25c5a6>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_reset__statement_context_1a37f8c3f608bc79677734bafb175829a2>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_reset__statement_context_1a49f1fa24a6279934bfe1467bc05d12bd>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_reset__statement_context_1a065055c552857af2d24f67c449757cf7>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
