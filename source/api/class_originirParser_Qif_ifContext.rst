.. index:: pair: class; originirParser::Qif_ifContext
.. _doxid-classoriginir_parser_1_1_qif__if_context:

class originirParser::Qif_ifContext
===================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Qif_ifContext: public :ref:`originirParser::Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`
	{
	public:
		// construction
	
		:target:`Qif_ifContext<doxid-classoriginir_parser_1_1_qif__if_context_1af0ab7345912adce75f9ccb0e5cb0b825>`(:ref:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`* ctx);

		// methods
	
		antlr4::tree::TerminalNode* :target:`QIF_KEY<doxid-classoriginir_parser_1_1_qif__if_context_1a931bf224ef5521f199bb04ce1188fd26>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_qif__if_context_1a3da98d325311d7c801877c6a1f51dc32>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`NEWLINE<doxid-classoriginir_parser_1_1_qif__if_context_1a8ce9cd160a61001e3eb5f691cce0ba70>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_qif__if_context_1a3b2cd8336f3ad4fde4869ea5dbbc75c9>`(size_t i);
		:ref:`Qelse_statement_fragmentContext<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context>`* :target:`qelse_statement_fragment<doxid-classoriginir_parser_1_1_qif__if_context_1ab1ceb384f2eff9cfd32aab68a129781e>`();
		antlr4::tree::TerminalNode* :target:`ENDIF_KEY<doxid-classoriginir_parser_1_1_qif__if_context_1a9eff5f642262aa1daecaac03ad7a39bc>`();
		std::vector<:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`*> :target:`statement<doxid-classoriginir_parser_1_1_qif__if_context_1aa6bae2e371b7032932d63f86aa0081db>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1_1_qif__if_context_1a205aa42889fc3ee6d253a7139552da39>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_qif__if_context_1a797d2434ceac648c8cb71cd538a52cfe>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_qif__if_context_1a9f4c3eb5a6c93ad2afefe96134b55ee6>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_qif__if_context_1a94e806e0ff1e05af59b11b3dc6b0ce5f>`(antlr4::tree::ParseTreeVisitor* visitor);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		void :ref:`copyFrom<doxid-classoriginir_parser_1_1_qif__statement_context_1a33b48efaadab92738d0962887ad3b087>`(:ref:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`* context);
		virtual size_t :ref:`getRuleIndex<doxid-classoriginir_parser_1_1_qif__statement_context_1ae6d18193ffe91eb5fe59fa4c25fd715e>`() const;

