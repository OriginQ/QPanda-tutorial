.. index:: pair: class; originirParser::Qwhile_statementContext
.. _doxid-classoriginir_parser_1_1_qwhile__statement_context:

class originirParser::Qwhile_statementContext
=============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Qwhile_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Qwhile_statementContext<doxid-classoriginir_parser_1_1_qwhile__statement_context_1acd231a4838647fdf1e3b705f7fdf114c>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_qwhile__statement_context_1abddc39bd7c12f550a0b1a37c05be6ba0>`() const;
		antlr4::tree::TerminalNode* :target:`QWHILE_KEY<doxid-classoriginir_parser_1_1_qwhile__statement_context_1af9843d1f3d061e0a355133126618fc9e>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_qwhile__statement_context_1a79d4f587f70bd7e7c09612a19bcfec43>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`NEWLINE<doxid-classoriginir_parser_1_1_qwhile__statement_context_1a6866b0f9963dfa42b0417aecb17f1384>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_qwhile__statement_context_1a4f1c44227f83563db7b06a27248df453>`(size_t i);
		antlr4::tree::TerminalNode* :target:`ENDQWHILE_KEY<doxid-classoriginir_parser_1_1_qwhile__statement_context_1a4532ff9bff869575d3aba8d79e298e61>`();
		std::vector<:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`*> :target:`statement<doxid-classoriginir_parser_1_1_qwhile__statement_context_1a373d09b06b87f203995a7538b874ceb4>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1_1_qwhile__statement_context_1a955880a3bd3b091556ac431298c62327>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_qwhile__statement_context_1aa66291a958add5b360882106cde71526>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_qwhile__statement_context_1af2d1fd89e01abaa68b2297e9a8a4d20f>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_qwhile__statement_context_1aefec4b2588770f6b963ee46353f1e74c>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
