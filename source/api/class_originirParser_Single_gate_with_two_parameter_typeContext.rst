.. index:: pair: class; originirParser::Single_gate_with_two_parameter_typeContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context:

class originirParser::Single_gate_with_two_parameter_typeContext
================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_two_parameter_typeContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context_1a4bc4db7a20ae867951e48fe524d6130f>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context_1a9988054941ba44bf3f5410542b33b0a7>`() const;
		antlr4::tree::TerminalNode* :target:`U2_GATE<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context_1a3765c45dff999423097613bce7a5a0e0>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context_1af4a195b8b6ea837ec093c0447810e26e>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context_1ac36239f1651df531bdcd045fb1e2f315>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context_1ac71b2e99e8a73cf69f5565b682b78287>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
