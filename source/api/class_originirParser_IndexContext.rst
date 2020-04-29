.. index:: pair: class; originirParser::IndexContext
.. _doxid-classoriginir_parser_1_1_index_context:

class originirParser::IndexContext
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class IndexContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`IndexContext<doxid-classoriginir_parser_1_1_index_context_1a047195ba356d0bb29f4986e24edff51f>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_index_context_1a3c0dbe1126cd73a5fbe7de520fca723b>`() const;
		antlr4::tree::TerminalNode* :target:`LBRACK<doxid-classoriginir_parser_1_1_index_context_1a513edd1740eb0b9d95c693e9e98d6886>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1_1_index_context_1a3b70b73cffa74e5210a7e808df4bfb51>`();
		antlr4::tree::TerminalNode* :target:`RBRACK<doxid-classoriginir_parser_1_1_index_context_1a457e71d3bb82da83bfcf6caab652cfd5>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_index_context_1a5a72cfded527746cad46c40645cfe779>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_index_context_1aad2293fb2f9dcb5f5d097a6ef241e914>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_index_context_1a9c7cbb6593a7441d73c90f18acce13ca>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
