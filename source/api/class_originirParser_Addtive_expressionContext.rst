.. index:: pair: class; originirParser::Addtive_expressionContext
.. _doxid-classoriginir_parser_1_1_addtive__expression_context:

class originirParser::Addtive_expressionContext
===============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Addtive_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context_1aca7440739a8419cc16a648092a7e0b09>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_addtive__expression_context_1a569d671fa385ce48d294dd6417ffb1b9>`() const;
		:ref:`Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`* :target:`multiplicative_expression<doxid-classoriginir_parser_1_1_addtive__expression_context_1ac9b2c5a4f7100b05979b69232f1dc2d6>`();
		Addtive_expressionContext* :target:`addtive_expression<doxid-classoriginir_parser_1_1_addtive__expression_context_1ad972f71756f2e5a06614358f481d9c36>`();
		antlr4::tree::TerminalNode* :target:`PLUS<doxid-classoriginir_parser_1_1_addtive__expression_context_1a191da8720a94361dee37407ac8212a1e>`();
		antlr4::tree::TerminalNode* :target:`MINUS<doxid-classoriginir_parser_1_1_addtive__expression_context_1ace9fb623a2aa610a2e8a3a7bc9575cf4>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_addtive__expression_context_1a0804569dd703ec8f9359b09f569ece9f>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_addtive__expression_context_1a74520f01b0e8c1f24cdccb6d86ce25a9>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_addtive__expression_context_1a472ad9a8b0ce37d3d3359527d476576f>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
