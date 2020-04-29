.. index:: pair: class; qasmParser::IdlistContext
.. _doxid-classqasm_parser_1_1_idlist_context:

class qasmParser::IdlistContext
===============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class IdlistContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context_1a92c76ce77b65195348e8ecc9b0490c25>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_idlist_context_1aa852618253d7ff184efa0cd5cb448fab>`() const;
		std::vector<:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`*> :target:`id<doxid-classqasm_parser_1_1_idlist_context_1aeb775ff8679ad57f03ec4045279bdf34>`();
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_idlist_context_1adba91b4c024d2f0501a84315e9ef7971>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classqasm_parser_1_1_idlist_context_1a680e6f7e17b144883584648c328317b3>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classqasm_parser_1_1_idlist_context_1ab569c86eddc0dcb59f30c57a57df5f75>`(size_t i);
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_idlist_context_1a4397af7ba28ce4bde882a07493f7a9d4>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_idlist_context_1a369766f196334de1f6b18154095a9144>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_idlist_context_1aec23499e81b6dfb93c856bf3da8ae472>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
