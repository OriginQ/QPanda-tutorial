.. index:: pair: class; qasmParser::Barrier_declContext
.. _doxid-classqasm_parser_1_1_barrier__decl_context:

class qasmParser::Barrier_declContext
=====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class Barrier_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context_1aab1a1d57eb17a420383ab20bf60a8a5e>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_barrier__decl_context_1ae102f3d9d30a7cab8711fd84ab1a7743>`() const;
		antlr4::tree::TerminalNode* :target:`BARRIER_KEY<doxid-classqasm_parser_1_1_barrier__decl_context_1a7a14f2bb4bf51708653042db3477f2d0>`();
		:ref:`AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* :target:`anylist<doxid-classqasm_parser_1_1_barrier__decl_context_1ac4215cb5bedbbfa0404edce6740c9298>`();
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_barrier__decl_context_1a8cefee1b069cd853a6ca909589f9eeeb>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_barrier__decl_context_1ad9dd6c34e764d6a326c7d80fbeacf750>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_barrier__decl_context_1a56ab5b6ac4786ccbb16a98489c2b8274>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_barrier__decl_context_1a64941a33820794708efb686f507d92f3>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
