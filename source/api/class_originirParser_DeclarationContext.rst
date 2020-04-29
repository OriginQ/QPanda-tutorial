.. index:: pair: class; originirParser::DeclarationContext
.. _doxid-classoriginir_parser_1_1_declaration_context:

class originirParser::DeclarationContext
========================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class DeclarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`DeclarationContext<doxid-classoriginir_parser_1_1_declaration_context_1a15de7ae10f06b4face5044f4de6b8147>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_declaration_context_1a4ec9abff3c0d86b7624d27da0e34949e>`() const;
		:ref:`Qinit_declarationContext<doxid-classoriginir_parser_1_1_qinit__declaration_context>`* :target:`qinit_declaration<doxid-classoriginir_parser_1_1_declaration_context_1a4da8d9f7feabb4419df1bde66a2f60e0>`();
		:ref:`Cinit_declarationContext<doxid-classoriginir_parser_1_1_cinit__declaration_context>`* :target:`cinit_declaration<doxid-classoriginir_parser_1_1_declaration_context_1a87166ee505864351e31e9986a82ec703>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_declaration_context_1a351a4976856bf16fb9620a9a18c9e164>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_declaration_context_1a10a88e3435e40dc90af40a94edd8fa56>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_declaration_context_1af9961b8b84e8b4d85b89a6566975f5b5>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
