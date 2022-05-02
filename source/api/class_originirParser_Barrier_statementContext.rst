.. index:: pair: class; originirParser::Barrier_statementContext
.. _doxid-classoriginir_parser_1_1_barrier__statement_context:

class originirParser::Barrier_statementContext
==============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Barrier_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Barrier_statementContext<doxid-classoriginir_parser_1_1_barrier__statement_context_1a1a725847f5dbd475074a76b7860955e7>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_barrier__statement_context_1a9397dcbb3710ef394970354f039837b8>`() const;
		antlr4::tree::TerminalNode* :target:`BARRIER_KEY<doxid-classoriginir_parser_1_1_barrier__statement_context_1ab485a74bc359584059cfd8ceac65bc52>`();
		:ref:`Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context>`* :target:`controlbit_list<doxid-classoriginir_parser_1_1_barrier__statement_context_1a81bc011cc33b6e3bec76b37d0e9640a3>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_barrier__statement_context_1a1015526aba3f7e4d3d8f193e5368ec2a>`();
		antlr4::tree::TerminalNode* :target:`Q_KEY<doxid-classoriginir_parser_1_1_barrier__statement_context_1aab4e3582f2f6cc7b4967a197322b0490>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_barrier__statement_context_1a36905eaeb407e6fca372f04753d5c579>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_barrier__statement_context_1a78a617a8b9e19ee1bc1f3473c7fd75fb>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_barrier__statement_context_1adf878571e005fed7022b1539a5df9b86>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
