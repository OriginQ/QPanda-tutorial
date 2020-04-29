.. index:: pair: class; originirParser::C_KEY_declarationContext
.. _doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context:

class originirParser::C_KEY_declarationContext
==============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class C_KEY_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context_1a907e6b26d5072a578896058cb60732e6>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context_1a8908831c898818fb049696e190573b82>`() const;
		antlr4::tree::TerminalNode* :target:`C_KEY<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context_1acc79dad40e93883f400176fa58f50d65>`();
		:ref:`IndexContext<doxid-classoriginir_parser_1_1_index_context>`* :target:`index<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context_1ac696074c3d779e2fa2f83e73716a6876>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context_1af528edca754007fe15924cc593bb6bf9>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context_1ab5e4a55df3522bfb0b315b0e1bfd24eb>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context_1a63b1f8280b70ebce5fb050e22acc995d>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
