.. index:: pair: class; originirParser::Double_gate_with_one_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context:

class originirParser::Double_gate_with_one_parameter_typeContext
================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Double_gate_with_one_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context_1a0914f4099a30647892034103b92baa20>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context_1ac109e930595646c0c1fc10b8379b54ae>`() const;
		antlr4::tree::TerminalNode* :target:`ISWAPTHETA_GATE<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context_1a09c99db974bfde74cc313a1ca0b219be>`();
		antlr4::tree::TerminalNode* :target:`CR_GATE<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context_1af7b9fa2084d71e62ed36eb264fa66f68>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context_1a9d2e1a58fb9f9a4409d2dd6512940db8>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context_1ac92dc2fcab287fb5bd22ba7e29d35d3f>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context_1aee33b325ffa4c8f166f3f860aa5591f0>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
