.. index:: pair: class; qasmParser::UopContext
.. _doxid-classqasm_parser_1_1_uop_context:

class qasmParser::UopContext
============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class UopContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`UopContext<doxid-classqasm_parser_1_1_uop_context_1a010e71df6fa1789637e962124c3de720>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_uop_context_1a8967189d50f5c358172787652fdf5c00>`() const;
		antlr4::tree::TerminalNode* :target:`U_GATE_KEY<doxid-classqasm_parser_1_1_uop_context_1a0ad11f5caea56724b4b4da1172cb24d5>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classqasm_parser_1_1_uop_context_1a5de9590ce7bf13910efa197275019fc3>`();
		:ref:`ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* :target:`explist<doxid-classqasm_parser_1_1_uop_context_1a681c7f0b91f84f239d80cf7acbd4633a>`();
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classqasm_parser_1_1_uop_context_1a362ab17de4b20962f1886feee7092015>`();
		std::vector<:ref:`ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`*> :target:`argument<doxid-classqasm_parser_1_1_uop_context_1a0cdda9849b51e67abad01676d0746953>`();
		:ref:`ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* :target:`argument<doxid-classqasm_parser_1_1_uop_context_1a189f5131dfd6e0385806e11e4798ed0c>`(size_t i);
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_uop_context_1a8d24315e015ecfdb1efec332b769a617>`();
		antlr4::tree::TerminalNode* :target:`CX_GATE_KEY<doxid-classqasm_parser_1_1_uop_context_1ae4bf58bc07273f766622ed771ab38865>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classqasm_parser_1_1_uop_context_1a21244768e691d02c6d79b2e5e63f847c>`();
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_uop_context_1a7ad2d5308df532e9ad6850e573afbcac>`();
		:ref:`AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* :target:`anylist<doxid-classqasm_parser_1_1_uop_context_1a3770895040f4f0927a4539e564a14c99>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_uop_context_1a90914118bbda8df0dc450f9315628928>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_uop_context_1a8decf14b4c9dc770e60a78ff01ced66e>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_uop_context_1abc4034e45f568120b5ea3ee4c7ed6da3>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
