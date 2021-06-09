.. index:: pair: class; originirParser::ExpContext
.. _doxid-classoriginir_parser_1_1_exp_context:

class originirParser::ExpContext
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class ExpContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`ExpContext<doxid-classoriginir_parser_1_1_exp_context_1a5496590b9cbd36d4718fd66465cf481e>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_exp_context_1ade94a12d7b38ab4f1d6f1ccb3d127b6b>`() const;
		:ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`* :target:`id<doxid-classoriginir_parser_1_1_exp_context_1aedf0020c869b39988e75897b6501451b>`();
		antlr4::tree::TerminalNode* :target:`Integer_Literal<doxid-classoriginir_parser_1_1_exp_context_1a9e72df0a88b5f02335f764884664114e>`();
		antlr4::tree::TerminalNode* :target:`Double_Literal<doxid-classoriginir_parser_1_1_exp_context_1a16488442a426301ae1eea1ce117f8935>`();
		antlr4::tree::TerminalNode* :target:`PI<doxid-classoriginir_parser_1_1_exp_context_1a04406b9b2c01da64658d2e19a4abbebc>`();
		antlr4::tree::TerminalNode* :target:`LPAREN<doxid-classoriginir_parser_1_1_exp_context_1a8e6214fb87dd25ab000b1d9eefdd5a3f>`();
		std::vector<ExpContext*> :target:`exp<doxid-classoriginir_parser_1_1_exp_context_1a0216efca583de6681365328e28183777>`();
		ExpContext* :target:`exp<doxid-classoriginir_parser_1_1_exp_context_1a8392549cafa716f931741982eaf4ccfb>`(size_t i);
		antlr4::tree::TerminalNode* :target:`RPAREN<doxid-classoriginir_parser_1_1_exp_context_1a019e0dbfc933d6c62f0251569c9b031a>`();
		antlr4::tree::TerminalNode* :target:`MINUS<doxid-classoriginir_parser_1_1_exp_context_1a9e4f13a75f48fe08dedbf0a399888dc6>`();
		antlr4::tree::TerminalNode* :target:`MUL<doxid-classoriginir_parser_1_1_exp_context_1a661d49705a9e60b5110112e409027749>`();
		antlr4::tree::TerminalNode* :target:`DIV<doxid-classoriginir_parser_1_1_exp_context_1af0dc3f269450ca4916a1ec94e685b5e7>`();
		antlr4::tree::TerminalNode* :target:`PLUS<doxid-classoriginir_parser_1_1_exp_context_1ab95d68769bd6459185ca51da1d02c51e>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_exp_context_1adf02614d688044b6e2b242af85f85130>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_exp_context_1ae42201f17d89467f906d35050c2c4fd9>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_exp_context_1aea74d79462e1050d77e90624e900fcfa>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
