.. index:: pair: class; qasmParser::BopContext
.. _doxid-classqasm_parser_1_1_bop_context:

class qasmParser::BopContext
============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class BopContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`BopContext<doxid-classqasm_parser_1_1_bop_context_1ae8b4d506dcb103730c411a5c82639f23>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_bop_context_1a3265712d0ac9a988d89c4390b2bb1e16>`() const;
		antlr4::tree::TerminalNode* :target:`BARRIER_KEY<doxid-classqasm_parser_1_1_bop_context_1aeb3840b6685a3a99565c5b807e4345ff>`();
		:ref:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* :target:`idlist<doxid-classqasm_parser_1_1_bop_context_1a2e7f83b700776370e685e67b2bf4d29b>`();
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_bop_context_1a932b7b57c27ad0161ac53cda3dc9d590>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_bop_context_1a52f881d6d5c4b964a504eda281a5f245>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_bop_context_1a1c5966bd0791c36c452e7942437679de>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_bop_context_1a2b4d7975138973e1135cae4d36ab0650>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
