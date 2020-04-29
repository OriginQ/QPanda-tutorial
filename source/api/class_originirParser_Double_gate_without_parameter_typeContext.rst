.. index:: pair: class; originirParser::Double_gate_without_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context:

class originirParser::Double_gate_without_parameter_typeContext
===============================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Double_gate_without_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1aa4e3cd4a41468ba81eb5cb40ff1a1366>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1afe63a7030160eddbd0023b5d2c3bb989>`() const;
		antlr4::tree::TerminalNode* :target:`CNOT_GATE<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1a938caafbf8130dc32730441ff7a78978>`();
		antlr4::tree::TerminalNode* :target:`CZ_GATE<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1a6fd5a323e5adf124ca8803a440017610>`();
		antlr4::tree::TerminalNode* :target:`ISWAP_GATE<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1a18e9ecdc7bf716ff6f9f798b11755d8f>`();
		antlr4::tree::TerminalNode* :target:`SQISWAP_GATE<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1ab2b6dbc5e65c5842bb86a7ae15500a5d>`();
		antlr4::tree::TerminalNode* :target:`SWAPZ1_GATE<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1a10ea075e3c7adac5f09964fc4ba62411>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1a43310c1dcbb9f3e2d87ea614b1b8251e>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1a284eca43088fce77ee1b28f50d4aa87d>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context_1a75d0d401389e394626d7c8e72d585bea>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
