.. index:: pair: class; qasmParser::MainprogramContext
.. _doxid-classqasm_parser_1_1_mainprogram_context:

class qasmParser::MainprogramContext
====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class MainprogramContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context_1aa4adeb1fda26023ec079aef133e345f8>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_mainprogram_context_1a39d78b81484353af90c62dd8b5a7cf38>`() const;
		:ref:`Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* :target:`head_decl<doxid-classqasm_parser_1_1_mainprogram_context_1a1c151b649eb0e0a978fb08f0699d7f2b>`();
		std::vector<:ref:`StatementContext<doxid-classqasm_parser_1_1_statement_context>`*> :target:`statement<doxid-classqasm_parser_1_1_mainprogram_context_1ab6402d5898a71e17d1669ae432a988d4>`();
		:ref:`StatementContext<doxid-classqasm_parser_1_1_statement_context>`* :target:`statement<doxid-classqasm_parser_1_1_mainprogram_context_1af69a8fcf6dd3c281c7bb88e7c3badc55>`(size_t i);
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_mainprogram_context_1ae8e852b95c5f871a20edf2b33a55f933>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_mainprogram_context_1a2aac7483989befda47aeca9bc45d8980>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_mainprogram_context_1adf6c0c13bf7ef6cbea2ef78ad5991119>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
