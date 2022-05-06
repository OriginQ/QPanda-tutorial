.. index:: pair: class; originirParser::Gate_func_statementContext
.. _doxid-classoriginir_parser_1_1_gate__func__statement_context:

class originirParser::Gate_func_statementContext
================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Gate_func_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Gate_func_statementContext<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a4d7d86869a31cf8633fdb8d8d5b33757>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_gate__func__statement_context_1ab573befadf4e51adb32f6ed12e71bcdd>`() const;
		antlr4::tree::TerminalNode* :target:`QGATE_KEY<doxid-classoriginir_parser_1_1_gate__func__statement_context_1ac3d473e144b6d0c0a127ea9325d06672>`();
		:ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`* :target:`id<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a72185a82dc83f4eb9b5c27e741537f87>`();
		std::vector<:ref:`Id_listContext<doxid-classoriginir_parser_1_1_id__list_context>`*> :target:`id_list<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a8c37511a7600eb48008500cfe56313b5>`();
		:ref:`Id_listContext<doxid-classoriginir_parser_1_1_id__list_context>`* :target:`id_list<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a9d9bbb4128767fd5599b1be018a9ea7a>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`NEWLINE<doxid-classoriginir_parser_1_1_gate__func__statement_context_1afbc91c31ab2920a51739eae50b2ef831>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a1d1f894a43344d1c3115c059b9fe3015>`(size_t i);
		antlr4::tree::TerminalNode* :target:`ENDQGATE_KEY<doxid-classoriginir_parser_1_1_gate__func__statement_context_1acbe76b48512949ba8cf7527a544239fe>`();
		std::vector<:ref:`Define_gate_statementContext<doxid-classoriginir_parser_1_1_define__gate__statement_context>`*> :target:`define_gate_statement<doxid-classoriginir_parser_1_1_gate__func__statement_context_1ad37227661defc3e80445d9fd679ebd54>`();
		:ref:`Define_gate_statementContext<doxid-classoriginir_parser_1_1_define__gate__statement_context>`* :target:`define_gate_statement<doxid-classoriginir_parser_1_1_gate__func__statement_context_1af442ba7cbf6375afe100a9fb1c8bc26b>`(size_t i);
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a581a080aaf020b44d04949d83e6ff113>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a508cbce0d57c5925a41fb1e0f5389009>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a42689542e74c2d920c6adb4d02136516>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a5420a410813276d27985f590ddf6e2f4>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a864f942b90b848a78d9a9e6947792be1>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_gate__func__statement_context_1a8fba37e18ab7c890f1b889be34b55121>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
