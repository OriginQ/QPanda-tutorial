.. index:: pair: class; originirParser::StatementContext
.. _doxid-classoriginir_parser_1_1_statement_context:

class originirParser::StatementContext
======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class StatementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`StatementContext<doxid-classoriginir_parser_1_1_statement_context_1abc959a59203026141e607f633f13e308>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_statement_context_1a9f88e4b0275a7c84bddc468ae4ef26ee>`() const;
		:ref:`Quantum_gate_declarationContext<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context>`* :target:`quantum_gate_declaration<doxid-classoriginir_parser_1_1_statement_context_1aaa2fe02f14d5d6dff221d0f34af71742>`();
		antlr4::tree::TerminalNode* :target:`NEWLINE<doxid-classoriginir_parser_1_1_statement_context_1abb9fe37318bb725282944cef9e009f7b>`();
		:ref:`Control_statementContext<doxid-classoriginir_parser_1_1_control__statement_context>`* :target:`control_statement<doxid-classoriginir_parser_1_1_statement_context_1aa5bbeb1b22ed2329f72679932f4f1972>`();
		:ref:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`* :target:`qif_statement<doxid-classoriginir_parser_1_1_statement_context_1a25b23e8bc5dc6bda3d6675252504c85f>`();
		:ref:`Qwhile_statementContext<doxid-classoriginir_parser_1_1_qwhile__statement_context>`* :target:`qwhile_statement<doxid-classoriginir_parser_1_1_statement_context_1a384068ed9c89c7fdd4f5bad0a830adb8>`();
		:ref:`Dagger_statementContext<doxid-classoriginir_parser_1_1_dagger__statement_context>`* :target:`dagger_statement<doxid-classoriginir_parser_1_1_statement_context_1a1bd9e1fa380996108d3746b1db9d6eed>`();
		:ref:`Measure_statementContext<doxid-classoriginir_parser_1_1_measure__statement_context>`* :target:`measure_statement<doxid-classoriginir_parser_1_1_statement_context_1a4ed60bb5c0c352e2fb32783cd41cf907>`();
		:ref:`Reset_statementContext<doxid-classoriginir_parser_1_1_reset__statement_context>`* :target:`reset_statement<doxid-classoriginir_parser_1_1_statement_context_1a60cef50b1e7495368d710318ed0d8e1f>`();
		:ref:`Expression_statementContext<doxid-classoriginir_parser_1_1_expression__statement_context>`* :target:`expression_statement<doxid-classoriginir_parser_1_1_statement_context_1a2d0e5b3254dabfea38786589f2359331>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_statement_context_1a123120bb9fdf00b3d6b6f6904c2b0caf>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_statement_context_1a50d7cb59cd5352a50aa636af94fa06ea>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_statement_context_1aa260912fd526e33b1c21845e252915a3>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
