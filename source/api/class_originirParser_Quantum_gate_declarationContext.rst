.. index:: pair: class; originirParser::Quantum_gate_declarationContext
.. _doxid-classoriginir_parser_1_1_quantum__gate__declaration_context:

class originirParser::Quantum_gate_declarationContext
=====================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Quantum_gate_declarationContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Quantum_gate_declarationContext<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a31a414bea46ae954e450d29e26a07d5d>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1ac287b65c54ed96756b18d18a2b53863c>`() const;
		:ref:`Single_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context>`* :target:`single_gate_without_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a73b8f4fc91f8d03c59b862fc98a45ab3>`();
		:ref:`Single_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context>`* :target:`single_gate_with_one_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a28938c8c875985dad0845489e3dfee30>`();
		:ref:`Single_gate_with_two_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context>`* :target:`single_gate_with_two_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a0ce2321ea7ad3b5b28f2f214b9c826d8>`();
		:ref:`Single_gate_with_three_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context>`* :target:`single_gate_with_three_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a989bcc5eccd46a2cb721780ddef615d9>`();
		:ref:`Single_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context>`* :target:`single_gate_with_four_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a6b5c092972c0eda0862cd528afc92048>`();
		:ref:`Double_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context>`* :target:`double_gate_without_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a43b7dd1a3594025f3c3130549481d347>`();
		:ref:`Double_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context>`* :target:`double_gate_with_one_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a55e7276df9d02d61c528c7eb8e7c03f1>`();
		:ref:`Double_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context>`* :target:`double_gate_with_four_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a0184019cde68bb44d623f5a503ca2c6a>`();
		:ref:`Triple_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context>`* :target:`triple_gate_without_parameter_declaration<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1aad3eb28eccca72b9f4bdba9b299663cd>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1ac0a4f96aa3bec6f4be4d0c1396b05c7a>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1a9265873f108817a8bbc5a40b4e00fc70>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context_1aa98339cc1e7c97acc8d475140578295d>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
