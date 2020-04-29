.. index:: pair: class; originirParser::Single_gate_without_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context:

class originirParser::Single_gate_without_parameter_typeContext
===============================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_without_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1aa136e000dda7213266658f68bbffb5d6>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1ad8f6de57f5820718ef36565133c64047>`() const;
		antlr4::tree::TerminalNode* :target:`H_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1a3aed1a97b132faddd73698dbf015d0e6>`();
		antlr4::tree::TerminalNode* :target:`T_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1aa1b3850d4309a9c7157e9a9afa72c5e6>`();
		antlr4::tree::TerminalNode* :target:`S_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1a9f4c06c05bd45b9b3bc27ea17fcca7db>`();
		antlr4::tree::TerminalNode* :target:`X_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1a9b85f3975c52b544e6a393c65b293ae8>`();
		antlr4::tree::TerminalNode* :target:`Y_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1ac757a1816e3330a7df87c2a72b5d170d>`();
		antlr4::tree::TerminalNode* :target:`Z_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1af890942d1b08e97dd378e7e30590245f>`();
		antlr4::tree::TerminalNode* :target:`X1_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1a813dbda364c5b7be9a44f629f19935de>`();
		antlr4::tree::TerminalNode* :target:`Y1_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1aa5dc49caa9a2c32824b75e9ee326a961>`();
		antlr4::tree::TerminalNode* :target:`Z1_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1a15a6f2a8cf131f3b63c0de68a8c259f1>`();
		antlr4::tree::TerminalNode* :target:`I_GATE<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1aaff522db09b21418717c6288e27036b6>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1a7831fec917463484a7ae29a4f0f3d694>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1a923a5780f046ea2d92e07697a3f1f333>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context_1aeb22bc340a6550b816e50f10970f99c2>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
