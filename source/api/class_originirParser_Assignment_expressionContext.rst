.. index:: pair: class; originirParser::Assignment_expressionContext
.. _doxid-classoriginir_parser_1_1_assignment__expression_context:

class originirParser::Assignment_expressionContext
==================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Assignment_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Assignment_expressionContext<doxid-classoriginir_parser_1_1_assignment__expression_context_1a04df8f2b71e299c2a4c4eb2772a67419>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_assignment__expression_context_1a1ba7b538f88fcea0b627e3860c6fec8f>`() const;
		:ref:`Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`* :target:`logical_or_expression<doxid-classoriginir_parser_1_1_assignment__expression_context_1ab0b0ac5bdaec44174bea343c3a1c4388>`();
		:ref:`C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`* :target:`c_KEY_declaration<doxid-classoriginir_parser_1_1_assignment__expression_context_1a8d4f1b37838d830732808daa2eae1a1f>`();
		antlr4::tree::TerminalNode* :target:`ASSIGN<doxid-classoriginir_parser_1_1_assignment__expression_context_1a1f02abc97f3d451b411e5ab359cdfa52>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_assignment__expression_context_1a875cbe664007bdc44ef26be7c9276d74>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_assignment__expression_context_1a2a6a80d394cea3cb9f5739019b4f3829>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_assignment__expression_context_1a54b41c3afdbf4bef7ba1c41abd7dc359>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
