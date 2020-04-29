.. index:: pair: class; originirParser::Triple_gate_without_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context:

class originirParser::Triple_gate_without_parameter_typeContext
===============================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Triple_gate_without_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context_1a2e237483f2b32ee62f6c6201a08b0c21>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context_1a37f8110d16b67085f1c1cbc8f1dafdc4>`() const;
		antlr4::tree::TerminalNode* :target:`TOFFOLI_GATE<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context_1a4e2ebc6fd749f2ca7a710c197489a42d>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context_1a7ddb99973138fe36b6513e754c58239a>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context_1a29e61b3d82d818a298d2916fe3f21073>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context_1a53413e8a8f8152d4a03368abda478c5a>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
