.. index:: pair: class; originirParser::Single_gate_with_two_parameter_declarationContext
.. _doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context:

class originirParser::Single_gate_with_two_parameter_declarationContext
=======================================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Single_gate_with_two_parameter_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Single_gate_with_two_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1a65f3874a20d4f2774e6b58e69cf79cf5>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1a496d542862fbfaf37b1956ba871e1785>`() const;
		:ref:`Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context>`* :target:`single_gate_with_two_parameter_type<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1adf9e36f15387d94af20e330d818f249d>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1a18e709600d8ef1bb8b44bde2217beb82>`();
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1afc661b7eb4c70576dec35f9787cd7a4c>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1aad58cc98f4d571d841fce4ca02abdaeb>`(size_t i);
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1a11d9bee7012b81ddafc0794923e5358f>`();
		std::vector<:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`*> :target:`expression<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1a513045ee95acc85abf928e0272f7fdf0>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1a01fc2d97b21c0f41c83d1c7ff19dfed5>`(size_t i);
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1ab1ebad89c90248a01d8c2af0f00ba392>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1afe73d355e86f19ce73e161f44f016b90>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1ad99c1371665558b225ad02e1065f3d08>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context_1aa6b8d2f35fb187f3a488c367f335689a>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
