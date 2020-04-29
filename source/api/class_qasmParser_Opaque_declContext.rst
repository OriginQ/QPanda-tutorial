.. index:: pair: class; qasmParser::Opaque_declContext
.. _doxid-classqasm_parser_1_1_opaque__decl_context:

class qasmParser::Opaque_declContext
====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class Opaque_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context_1a58fd949454887283bee25a184ca8f0d0>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_opaque__decl_context_1a39d62b2e2210197c32b0cd1ec00db89c>`() const;
		antlr4::tree::TerminalNode* :target:`OPAQUE_KEY<doxid-classqasm_parser_1_1_opaque__decl_context_1ad94d505ed5deefce3218daeb643f5685>`();
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_opaque__decl_context_1ab9d7e2f44b9e60f3ec48d48cd5a83bf5>`();
		std::vector<:ref:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`*> :target:`idlist<doxid-classqasm_parser_1_1_opaque__decl_context_1ae013c7931aefa3a94fc077cbe4cecd79>`();
		:ref:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* :target:`idlist<doxid-classqasm_parser_1_1_opaque__decl_context_1ab6721e06475ed30327688a712833372a>`(size_t i);
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_opaque__decl_context_1ad42405cfbb9fea86a6b61a67e611a941>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classqasm_parser_1_1_opaque__decl_context_1a5f0ad4d823c15d0e44a8ac00a208ce83>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classqasm_parser_1_1_opaque__decl_context_1aea9ab93d9b4cf7fdb571579123689cc0>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_opaque__decl_context_1a59975f77ed9c4631f39b6f6f8486aa1b>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_opaque__decl_context_1a14f32d853cec2c822e5b87042d975aed>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_opaque__decl_context_1a6bfceb71292907f19217802f324d70c3>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
