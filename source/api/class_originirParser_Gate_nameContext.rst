.. index:: pair: class; originirParser::Gate_nameContext
.. _doxid-classoriginir_parser_1_1_gate__name_context:

class originirParser::Gate_nameContext
======================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Gate_nameContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Gate_nameContext<doxid-classoriginir_parser_1_1_gate__name_context_1aeaa67d6da7c846ecbf3507b809b94b4b>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_gate__name_context_1a76aeb71cb2fdc69fda83396e71172c12>`() const;
		:ref:`Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context>`* :target:`single_gate_without_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a4cb09490f67d4e92c65ece9434e379eb>`();
		:ref:`Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context>`* :target:`single_gate_with_one_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a7f5f10e2c88749a2c4b4a3130d6fa317>`();
		:ref:`Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context>`* :target:`single_gate_with_two_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a1b37a11a4c5aec56a36406e071a0c42e>`();
		:ref:`Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context>`* :target:`single_gate_with_three_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a7f6504423f7419b41bce0ee3b1c54041>`();
		:ref:`Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context>`* :target:`single_gate_with_four_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a4bbdf9480bcc2cf6a635956462470689>`();
		:ref:`Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context>`* :target:`double_gate_without_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a2f31a42c30beaf5606374434ab187117>`();
		:ref:`Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context>`* :target:`double_gate_with_one_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1acfb3e4b477bbb7e1e908135e79580115>`();
		:ref:`Double_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__type_context>`* :target:`double_gate_with_four_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a7d81e99439ebdb1cc8b23e104886829e>`();
		:ref:`Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context>`* :target:`triple_gate_without_parameter_type<doxid-classoriginir_parser_1_1_gate__name_context_1a4df31912820d3bdc626c24e7cd8b7003>`();
		:ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`* :target:`id<doxid-classoriginir_parser_1_1_gate__name_context_1ab705f29df5e02e1e623c5bfd3a078c9f>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_gate__name_context_1a0586750b3a7208239787f571e36a6cda>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_gate__name_context_1ad02e59a8da7f6b8a7139061ea3e5a723>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_gate__name_context_1a1fa088ac7a6cafeed1fca5128dd2d46d>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
