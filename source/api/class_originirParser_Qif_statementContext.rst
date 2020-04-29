.. index:: pair: class; originirParser::Qif_statementContext
.. _doxid-classoriginir_parser_1_1_qif__statement_context:

class originirParser::Qif_statementContext
==========================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Qif_statementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context_1aa326a1f4ba544765a860541c91b81aed>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);
	
		:target:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context_1a6e9d0562dec50aa5ffbcf551ad204247>`();

		// methods
	
		void :target:`copyFrom<doxid-classoriginir_parser_1_1_qif__statement_context_1a33b48efaadab92738d0962887ad3b087>`(Qif_statementContext* context);
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_qif__statement_context_1ae6d18193ffe91eb5fe59fa4c25fd715e>`() const;
	};

	// direct descendants

	class :ref:`Qif_ifContext<doxid-classoriginir_parser_1_1_qif__if_context>`;
	class :ref:`Qif_ifelseContext<doxid-classoriginir_parser_1_1_qif__ifelse_context>`;
