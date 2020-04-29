.. index:: pair: class; originirParser::Single_gate_with_four_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context:

class originirParser::Single_gate_with_four_parameter_typeContext
=================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_four_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context_1ac0525a7c1cf743db7e6a87bced32bb2e>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context_1a65067154a9cf62c9b78c3cf760b90ac4>`() const;
		antlr4::tree::TerminalNode* :target:`U4_GATE<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context_1ab135608cef400868aa5f953e73c8f21e>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context_1ae87c9c78a1d5a154d84953196e590b6d>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context_1a13b2fc99ed22e4984d0658499bfd729c>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context_1a4ef93d95caac67403db8cb24b1ac3a3d>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
