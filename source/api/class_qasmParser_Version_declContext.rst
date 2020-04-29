.. index:: pair: class; qasmParser::Version_declContext
.. _doxid-classqasm_parser_1_1_version__decl_context:

class qasmParser::Version_declContext
=====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class Version_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Version_declContext<doxid-classqasm_parser_1_1_version__decl_context_1a686816354a2306e29d42cc3b61df2921>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_version__decl_context_1a54d202bf9a3c629391d1ab47718e6a31>`() const;
		antlr4::tree::TerminalNode* :target:`OPENQASM_KEY<doxid-classqasm_parser_1_1_version__decl_context_1add7624a08444c2e67f13b0e2056ef457>`();
		:ref:`DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* :target:`decimal<doxid-classqasm_parser_1_1_version__decl_context_1a3e9c427646ad64854955b4414071a007>`();
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_version__decl_context_1a314a75978c28559b05a661a77f39e5d9>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_version__decl_context_1add8ef7b465e0cc0968c6d1816180284b>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_version__decl_context_1a123770efe70b7c87366b4a04ab3b2f3c>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_version__decl_context_1aeac79960562ede700575195d01a5f327>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
