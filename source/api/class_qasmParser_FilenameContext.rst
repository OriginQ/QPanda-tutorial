.. index:: pair: class; qasmParser::FilenameContext
.. _doxid-classqasm_parser_1_1_filename_context:

class qasmParser::FilenameContext
=================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class FilenameContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`FilenameContext<doxid-classqasm_parser_1_1_filename_context_1a0bcb3edc9c739e60fa369f423ccd2cae>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_filename_context_1abf39e2df2361cf9b04a3b2afe84add10>`() const;
		antlr4::tree::TerminalNode* :target:`FILENAME<doxid-classqasm_parser_1_1_filename_context_1af090ce262e95d2e92d54c3f0879d80d9>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_filename_context_1a2047ec9516602234b2050a7844b413ab>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_filename_context_1a57221461a7b493673c9f5bdde1ffa72a>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_filename_context_1a1f1f32a4edd519753bbaa7acaeb9bdf0>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
