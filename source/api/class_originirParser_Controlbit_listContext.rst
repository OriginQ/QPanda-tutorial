.. index:: pair: class; originirParser::Controlbit_listContext
.. _doxid-classoriginir_parser_1_1_controlbit__list_context:

class originirParser::Controlbit_listContext
============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Controlbit_listContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context_1af5aac53979ee7a024519ce5728da8bdc>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_controlbit__list_context_1af08eeaecb2673ce6e30eb1551d635df4>`() const;
		std::vector<:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`*> :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_controlbit__list_context_1ab9955e605583bafc781c162b85520373>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_controlbit__list_context_1ad43dc6720838722d8a5246f63d888cd0>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_controlbit__list_context_1a91478bc9165ed398b7ce4a5d6e59ec39>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_controlbit__list_context_1abf100e31a6a40c5f6ad88f6581282c66>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_controlbit__list_context_1ace416c5f7030d17b131973151537388e>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_controlbit__list_context_1abbc41f158b5f6ffb4f501eea917f444d>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_controlbit__list_context_1a89d9a55389b8385241cf7f5bacadc5b2>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
