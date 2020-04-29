.. index:: pair: class; originirParser::Qif_ifelseContext
.. _doxid-classoriginir_parser_1_1_qif__ifelse_context:

class originirParser::Qif_ifelseContext
=======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Qif_ifelseContext: public :ref:`originirParser::Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`
	{
	public:
		// construction
	
		:target:`Qif_ifelseContext<doxid-classoriginir_parser_1_1_qif__ifelse_context_1aa78ec5201c6c55b9e060c21b1ed76c6c>`(:ref:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`* ctx);

		// methods
	
		antlr4::tree::TerminalNode* :target:`QIF_KEY<doxid-classoriginir_parser_1_1_qif__ifelse_context_1a7b9bf88dc17465d484aff1dab5d62bda>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_qif__ifelse_context_1a8c088f640ec44e6c6b1fd1916a6ace7c>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`NEWLINE<doxid-classoriginir_parser_1_1_qif__ifelse_context_1aa436f084a73cded658ee0dcf56f16c6f>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_qif__ifelse_context_1ad06c9fea32d6b1608cc32d16205980ee>`(size_t i);
		antlr4::tree::TerminalNode* :target:`ENDIF_KEY<doxid-classoriginir_parser_1_1_qif__ifelse_context_1afacf85d87953be269eedc51a340f482f>`();
		std::vector<:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`*> :target:`statement<doxid-classoriginir_parser_1_1_qif__ifelse_context_1a4bec081ffacf8e792ae78142266d0ea1>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1_1_qif__ifelse_context_1aaad9f7770046ff6fd99fe430abe23937>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_qif__ifelse_context_1ab063e0e4d7e6912f7d742e99d677487b>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_qif__ifelse_context_1afa24d82998c7b982b0d5a84dbf4ca0a3>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_qif__ifelse_context_1a8c5c055330c658ace01200088e9a99de>`(antlr4::tree::ParseTreeVisitor* visitor);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		void :ref:`copyFrom<doxid-classoriginir_parser_1_1_qif__statement_context_1a33b48efaadab92738d0962887ad3b087>`(:ref:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`* context);
		virtual size_t :ref:`getRuleIndex<doxid-classoriginir_parser_1_1_qif__statement_context_1ae6d18193ffe91eb5fe59fa4c25fd715e>`() const;

