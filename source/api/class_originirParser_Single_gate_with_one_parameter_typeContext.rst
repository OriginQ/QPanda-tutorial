.. index:: pair: class; originirParser::Single_gate_with_one_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context:

class originirParser::Single_gate_with_one_parameter_typeContext
================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_one_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1a465da20603f6415a9e6f1af7c11724ba>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1a57599e97234d07779cee1b299b26a124>`() const;
		antlr4::tree::TerminalNode* :target:`RX_GATE<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1a820b58a94f4570e0f9761720d1ab5e20>`();
		antlr4::tree::TerminalNode* :target:`RY_GATE<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1a2ad817649b5bd64dfa085091b500e54d>`();
		antlr4::tree::TerminalNode* :target:`RZ_GATE<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1a99e5832633d85af84d6539bf4316d261>`();
		antlr4::tree::TerminalNode* :target:`U1_GATE<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1ab40363e5a47baad737a4f1ecdbdb34c6>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1aa0215ef573502aeeeb18fa33d050b919>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1acc84bbef6d176e59bd9b8579c9f97f03>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context_1a3cfccff91497e68cca6d0802b441f083>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
