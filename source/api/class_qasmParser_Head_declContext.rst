.. index:: pair: class; qasmParser::Head_declContext
.. _doxid-classqasm_parser_1_1_head__decl_context:

class qasmParser::Head_declContext
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class Head_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Head_declContext<doxid-classqasm_parser_1_1_head__decl_context_1a9c9fcf14f06364bda638d990a436e74d>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_head__decl_context_1aa0f705ede9712278e95bf8d440b9c6ac>`() const;
		:ref:`Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* :target:`version_decl<doxid-classqasm_parser_1_1_head__decl_context_1afe4764170c0fc09701f947aa8b428a03>`();
		:ref:`Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* :target:`include_decl<doxid-classqasm_parser_1_1_head__decl_context_1a2d304f71ba1a8103ccc0703eb14342c3>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_head__decl_context_1aa8eb7a299da7427ecae388053fc02bb0>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_head__decl_context_1aa632e0109a437eb9549e50cd20a22790>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_head__decl_context_1a745fe0f5dfe3a4dd9526efcc82ed4266>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
