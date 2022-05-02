.. index:: pair: class; originirParser::IdContext
.. _doxid-classoriginir_parser_1_1_id_context:

class originirParser::IdContext
===============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class IdContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`IdContext<doxid-classoriginir_parser_1_1_id_context_1a8faa2334d786d02bc3aceb3bcb9c7d99>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_id_context_1a3fccbce872d0738718e11152ce6e0cbd>`() const;
		antlr4::tree::TerminalNode* :target:`Identifier<doxid-classoriginir_parser_1_1_id_context_1a7bd3805fd43aaf89649a9e00860e2a13>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_id_context_1aa12ec4f7d66592e2c8db93d8b8b6ada2>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_id_context_1ae089626a01a998b5dc86dc225302a394>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_id_context_1aee5687f49bd262784ce654a8252ad36f>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
