.. index:: pair: class; qasmParser::Gate_declContext
.. _doxid-classqasm_parser_1_1_gate__decl_context:

class qasmParser::Gate_declContext
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class Gate_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context_1a61e49362b2d16a671f45be1797997ac8>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_gate__decl_context_1a2af7c4c63c7a6ceb40530c7f503e8b39>`() const;
		antlr4::tree::TerminalNode* :target:`GATE_KEY<doxid-classqasm_parser_1_1_gate__decl_context_1a73be04622992b6a0e29a3d0ef0f3069d>`();
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_gate__decl_context_1aa53a7670aebc0180b3243b1669b14ca4>`();
		std::vector<:ref:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`*> :target:`idlist<doxid-classqasm_parser_1_1_gate__decl_context_1a335ecbe217cb95adb10031a0c56c2787>`();
		:ref:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* :target:`idlist<doxid-classqasm_parser_1_1_gate__decl_context_1a2932a803ca148572e97d484207bad11e>`(size_t i);
		antlr4::tree::TerminalNode* :target:`LBRACE<doxid-classqasm_parser_1_1_gate__decl_context_1a570fb4b6ef6f81df42e70696bfc36e96>`();
		:ref:`GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* :target:`goplist<doxid-classqasm_parser_1_1_gate__decl_context_1a37dad9cf37e2ff69082ac7d3302b51e2>`();
		antlr4::tree::TerminalNode* :target:`RBRACE<doxid-classqasm_parser_1_1_gate__decl_context_1a66698ee45c30e84cf9d134d6b62567da>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classqasm_parser_1_1_gate__decl_context_1a73b0bf4b27e43d2224649cbe82a594aa>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classqasm_parser_1_1_gate__decl_context_1ad3ae031e072318aa1518d2a9d7fa3c8e>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_gate__decl_context_1a6d79c53fe205a065bd41b7347b2e6560>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_gate__decl_context_1a4b80880ad188734a21f2f7e189448f01>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_gate__decl_context_1a525346b69c13297711b01cf0c54e0252>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
