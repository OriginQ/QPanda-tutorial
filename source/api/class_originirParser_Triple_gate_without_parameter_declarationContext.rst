.. index:: pair: class; originirParser::Triple_gate_without_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context:

class originirParser::Triple_gate_without_parameter_declarationContext
======================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Triple_gate_without_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Triple_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1aad49c2dbc8e93265ae6ad66489bb0a4c>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1ac31864e4cd06381a0e9134dc79c94f3c>`() const;
		:ref:`Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context>`* :target:`triple_gate_without_parameter_type<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1a60d54a3b66035f994831744a493da52f>`();
		std::vector<:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`*> :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1aaa7a19cae7d8de3c1e858be710f6c451>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1ad8a1564c6be0411639e3fd137c8adcbd>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1a7ce28baae0e3a8d2f1954f73b9ef68f4>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1a1e093a68dd677614ed2e346f7262270b>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1ac8a5c135aaba9538a8f7a4be0c95dca9>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1a12a3516abd22d419e29fdd6a38c4918b>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context_1abd21516825157486ef306f7ab9f3bd52>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
