.. index:: pair: class; originirParser::Single_gate_with_three_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context:

class originirParser::Single_gate_with_three_parameter_typeContext
==================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_three_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context_1a64993fc868805acc44e1d4ae5bef9ddf>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context_1a3ebbb5217494dbe280cb0e2bfe793865>`() const;
		antlr4::tree::TerminalNode* :target:`U3_GATE<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context_1a05486bdcc9c17c19afcc53cacba5bafc>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context_1ad7ea5a2651a2e24e0569e5f2477eb4b1>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context_1a94ef6581ee20501db7230ad5e2a5d453>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context_1a8fb50a6b77098f6d1077d651c99d4ea0>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
