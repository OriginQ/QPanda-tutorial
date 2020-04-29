.. index:: pair: class; originirParser::Single_gate_without_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context:

class originirParser::Single_gate_without_parameter_declarationContext
======================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_without_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context_1a155c550de472ff58ccddc9814ff196be>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context_1a37c3469340ddddab881d17c0b2be5a1e>`() const;
		:ref:`Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context>`* :target:`single_gate_without_parameter_type<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context_1a71bac521debf4d8f7c1209bd8d3cbb44>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context_1a3a5832d9e56d4d819a79e3fa58138dcf>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context_1a3a6bbcc863df51f2ada6df6dcad8dec8>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context_1af4dfea5be2d99d0a48941ca66e6da8df>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context_1a5e1b6f21e8858f9ba4abc84ca0918271>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
