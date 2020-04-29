.. index:: pair: class; qasmParser::Include_declContext
.. _doxid-classqasm_parser_1_1_include__decl_context:

class qasmParser::Include_declContext
=====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class Include_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Include_declContext<doxid-classqasm_parser_1_1_include__decl_context_1a2ba5f8030a0f87567ef06c483b561aa7>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_include__decl_context_1ac50ff07ff957f4496a889ee33d19ff2b>`() const;
		antlr4::tree::TerminalNode* :target:`INCLUDE_KEY<doxid-classqasm_parser_1_1_include__decl_context_1af25d783d32577c26ca96cca63a86e7ec>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`DQM<doxid-classqasm_parser_1_1_include__decl_context_1a243866072cb75f00d175918515503f4b>`();
		antlr4::tree::TerminalNode* :target:`DQM<doxid-classqasm_parser_1_1_include__decl_context_1ac52b4924e714a694abb09142721660c6>`(size_t i);
		:ref:`FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* :target:`filename<doxid-classqasm_parser_1_1_include__decl_context_1a906e264a8dfd27180a5636f24303422e>`();
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_include__decl_context_1afe867c9149e88dd091d7658562ac76e4>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_include__decl_context_1a60c852fd5384f2138680405a25619f7c>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_include__decl_context_1ae26b18de59628393176acc4d19913f80>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_include__decl_context_1afcfa3b79c10f4afc1763cdbb2093ba08>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
