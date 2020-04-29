.. index:: pair: class; originirParser::TranslationunitContext
.. _doxid-classoriginir_parser_1_1_translationunit_context:

class originirParser::TranslationunitContext
============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class TranslationunitContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context_1a0036caaded147c03c80c6b81aebd27ed>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_translationunit_context_1a31cbb1c4a89cb9bc42cbaefe492f46e2>`() const;
		:ref:`DeclarationContext<doxid-classoriginir_parser_1_1_declaration_context>`* :target:`declaration<doxid-classoriginir_parser_1_1_translationunit_context_1abf40e167af07d469c379985b28714bc1>`();
		std::vector<:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`*> :target:`statement<doxid-classoriginir_parser_1_1_translationunit_context_1acdbc9264e8a9d441e3eec5136544fdea>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1_1_translationunit_context_1af15439f78624005a8b31342a6c6358e7>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_translationunit_context_1ae91d78b1935b7bcf3a23951cb45e3b7a>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_translationunit_context_1a1b0d5cef40ba2196e07370d44f43d5f4>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_translationunit_context_1a05df316b2d201befe54051ce54a859a8>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
