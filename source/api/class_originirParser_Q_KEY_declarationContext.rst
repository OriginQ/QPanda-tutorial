.. index:: pair: class; originirParser::Q_KEY_declarationContext
.. _doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context:

class originirParser::Q_KEY_declarationContext
==============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Q_KEY_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context_1a3ff60ed674707e6484fe43bb4248d634>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context_1ae8be23674fb9fe386c4f687e6e032e05>`() const;
		antlr4::tree::TerminalNode* :target:`Q_KEY<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context_1a16810d6f6e436c742092d026eb37ab06>`();
		:ref:`IndexContext<doxid-classoriginir_parser_1_1_index_context>`* :target:`index<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context_1aee18127de4b90ae162763ce91b1c5c0f>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context_1a22c04c33147a5aa4dad8cc192a1dee0c>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context_1a98b59914b8a4c9b67b8839089d2dd76f>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context_1ac846209d622f9189bef72ca96e698ab3>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
