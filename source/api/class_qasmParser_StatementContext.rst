.. index:: pair: class; qasmParser::StatementContext
.. _doxid-classqasm_parser_1_1_statement_context:

class qasmParser::StatementContext
==================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class StatementContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`StatementContext<doxid-classqasm_parser_1_1_statement_context_1a8fad68823c81ac398a68dfa0db51299a>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_statement_context_1a160a654b2c89a227baedaa753d3bff98>`() const;
		:ref:`Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* :target:`reg_decl<doxid-classqasm_parser_1_1_statement_context_1ae15dc863f59a34396684d17a728ebcf9>`();
		:ref:`Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* :target:`gate_decl<doxid-classqasm_parser_1_1_statement_context_1a9e530bc7a61a0e96a16a28997ea3aac1>`();
		:ref:`Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* :target:`opaque_decl<doxid-classqasm_parser_1_1_statement_context_1a50dcc9c83d6fb75db50c920c4999dd66>`();
		:ref:`If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* :target:`if_decl<doxid-classqasm_parser_1_1_statement_context_1af274de15628d57788d4e52ccdae1be50>`();
		:ref:`Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* :target:`barrier_decl<doxid-classqasm_parser_1_1_statement_context_1a04f64766387be98eb52770069b0dd1c1>`();
		:ref:`QopContext<doxid-classqasm_parser_1_1_qop_context>`* :target:`qop<doxid-classqasm_parser_1_1_statement_context_1ac305a5195e811e18709f5553a6249173>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_statement_context_1a6b60dc9338b7c534a884567ec2f1a086>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_statement_context_1a027657e9d4ba367d97bb910a1e46a2e9>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_statement_context_1aa0658ccbcf2059b6e2df8add17b7876a>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
