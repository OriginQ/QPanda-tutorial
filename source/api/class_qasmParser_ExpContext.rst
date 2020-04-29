.. index:: pair: class; qasmParser::ExpContext
.. _doxid-classqasm_parser_1_1_exp_context:

class qasmParser::ExpContext
============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class ExpContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`ExpContext<doxid-classqasm_parser_1_1_exp_context_1a0d5be134b707606745ed830df3184d9e>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_exp_context_1a84a09b9c6c0e320073735b4006319b49>`() const;
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_exp_context_1ad1753e0ac946ce0db6d0395a724a3c5f>`();
		:ref:`DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* :target:`decimal<doxid-classqasm_parser_1_1_exp_context_1ac8a7a5a85beff68071d4e7b55912868c>`();
		:ref:`IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* :target:`integer<doxid-classqasm_parser_1_1_exp_context_1aac3dc7d3f6ad0e55e52f21392d743396>`();
		antlr4::tree::TerminalNode* :target:`PI_KEY<doxid-classqasm_parser_1_1_exp_context_1acf22266345694a4df71eb6c8362920d8>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classqasm_parser_1_1_exp_context_1a0b6d34321b9724af2ff0cca246324f25>`();
		std::vector<ExpContext*> :target:`exp<doxid-classqasm_parser_1_1_exp_context_1a10e8aa1dad177334ef1d2f223b912af9>`();
		ExpContext* :target:`exp<doxid-classqasm_parser_1_1_exp_context_1a7a1a0ee42d0b613cff6cab18df725988>`(size_t i);
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classqasm_parser_1_1_exp_context_1a583cb891f5a24b14ddbe8c39f2b7faa3>`();
		antlr4::tree::TerminalNode* :target:`MINUS<doxid-classqasm_parser_1_1_exp_context_1a1d1c19b0776332179239bae99bf10821>`();
		antlr4::tree::TerminalNode* :target:`MUL<doxid-classqasm_parser_1_1_exp_context_1a020a436e8efe9e82c9c9c1344701bcdc>`();
		antlr4::tree::TerminalNode* :target:`DIV<doxid-classqasm_parser_1_1_exp_context_1ad2aab7cc712e7c356805df6056e535fa>`();
		antlr4::tree::TerminalNode* :target:`PLUS<doxid-classqasm_parser_1_1_exp_context_1a239e6fcf5d757bc8d58ba54c8d90c82c>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_exp_context_1a49b281fa3fcf246b85fdca0179b1672a>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_exp_context_1ad252954b06be8ca9fd171aa868ad4535>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_exp_context_1a88313d21bacc23db3bf93848f0589d1a>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
