.. index:: pair: class; originirParser::Measure_statementContext
.. _doxid-classoriginir_parser_1_1_measure__statement_context:

class originirParser::Measure_statementContext
==============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Measure_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Measure_statementContext<doxid-classoriginir_parser_1_1_measure__statement_context_1add424636ecc2fceaea0ed2896a85e0a4>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_measure__statement_context_1aaca282a1b82c5ec230e11a7e414134ad>`() const;
		antlr4::tree::TerminalNode* :target:`MEASURE_KEY<doxid-classoriginir_parser_1_1_measure__statement_context_1a48a86ffc2b06a6fe7ddd6ee643be43a8>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1_1_measure__statement_context_1a7378a0213a71d0ab8d85a89e05b424c2>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_measure__statement_context_1a0c17f2fd75fa332eae69bed1d63d4a03>`();
		:ref:`C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`* :target:`c_KEY_declaration<doxid-classoriginir_parser_1_1_measure__statement_context_1a58d13d0c639f85068927b4c02910dcd2>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_measure__statement_context_1a32d739c0277aa334098b2e1161e3383e>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_measure__statement_context_1ab7414bdf6f6885d7fa3b41795bf6acfe>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_measure__statement_context_1a4ba4b6768755d2d7a624f61350a1493e>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
