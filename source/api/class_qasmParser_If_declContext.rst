.. index:: pair: class; qasmParser::If_declContext
.. _doxid-classqasm_parser_1_1_if__decl_context:

class qasmParser::If_declContext
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class If_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`If_declContext<doxid-classqasm_parser_1_1_if__decl_context_1a94c735bb1dd24a9fa4c951d13e0a2fbc>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_if__decl_context_1a9c5c5eefcc7af92ac4af798e1c24fa2b>`() const;
		antlr4::tree::TerminalNode* :target:`IF_KEY<doxid-classqasm_parser_1_1_if__decl_context_1a17e2f6d8d09b21eedbd442d1d45137e1>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classqasm_parser_1_1_if__decl_context_1a754850f5f3754dbc7fa1b2be056ff8dd>`();
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_if__decl_context_1af8f3d722074ee08a5fabb08d488cfdce>`();
		antlr4::tree::TerminalNode* :target:`EQ<doxid-classqasm_parser_1_1_if__decl_context_1ae8dc85e46f4e029c5c18f4af2b7dc585>`();
		:ref:`IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* :target:`integer<doxid-classqasm_parser_1_1_if__decl_context_1a89e2a86ba93d28475fb1364eae92c39a>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classqasm_parser_1_1_if__decl_context_1a639d400a42f226f602640f56db58feaa>`();
		:ref:`QopContext<doxid-classqasm_parser_1_1_qop_context>`* :target:`qop<doxid-classqasm_parser_1_1_if__decl_context_1a174fd96e827132ceedcaf6813ff42d53>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_if__decl_context_1a331a4f5979023f05c829bb6f1c573371>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_if__decl_context_1ab4ff5fa3fab8a94451f4b7d1ed23767f>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_if__decl_context_1a38256c850166b71fe94e1e00f24db2eb>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
