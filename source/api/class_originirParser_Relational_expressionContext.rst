.. index:: pair: class; originirParser::Relational_expressionContext
.. _doxid-classoriginir_parser_1_1_relational__expression_context:

class originirParser::Relational_expressionContext
==================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Relational_expressionContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context_1afa2701f1cbefa32db509f9d9e4327eb5>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_relational__expression_context_1af272530aed5721a07bbb2ea30d6efc0e>`() const;
		:ref:`Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`* :target:`addtive_expression<doxid-classoriginir_parser_1_1_relational__expression_context_1af83696cfc479f59a95df3c19313d599f>`();
		Relational_expressionContext* :target:`relational_expression<doxid-classoriginir_parser_1_1_relational__expression_context_1a4ed55ed40406cffc6deb259e395fb950>`();
		antlr4::tree::TerminalNode* :target:`LT<doxid-classoriginir_parser_1_1_relational__expression_context_1a9068d26ae3e1131064bfbcf9c51183e9>`();
		antlr4::tree::TerminalNode* :target:`GT<doxid-classoriginir_parser_1_1_relational__expression_context_1a8856d967a33c111bc5a03a1efa2930bb>`();
		antlr4::tree::TerminalNode* :target:`LEQ<doxid-classoriginir_parser_1_1_relational__expression_context_1a4e39b4d0a7a10bb423a3678c1b2bc4b5>`();
		antlr4::tree::TerminalNode* :target:`GEQ<doxid-classoriginir_parser_1_1_relational__expression_context_1a824549428bb280dfe4b66b20be912b0e>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_relational__expression_context_1a3d7f1146583fdf1c24258b576fe891d4>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_relational__expression_context_1a5f1d97cb73a4e195c9d838708cadeb45>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_relational__expression_context_1a2e370af360b284837f10a1cf0c8ddaf9>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
