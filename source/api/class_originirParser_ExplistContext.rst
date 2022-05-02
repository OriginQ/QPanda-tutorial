.. index:: pair: class; originirParser::ExplistContext
.. _doxid-classoriginir_parser_1_1_explist_context:

class originirParser::ExplistContext
====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class ExplistContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`ExplistContext<doxid-classoriginir_parser_1_1_explist_context_1a504cbd33ebb0c73bb96994799b0ff176>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_explist_context_1a426b72bdcf731e7b2dd076c50cb8137e>`() const;
		std::vector<:ref:`ExpContext<doxid-classoriginir_parser_1_1_exp_context>`*> :target:`exp<doxid-classoriginir_parser_1_1_explist_context_1a759161ed6d88484cb602d29914118949>`();
		:ref:`ExpContext<doxid-classoriginir_parser_1_1_exp_context>`* :target:`exp<doxid-classoriginir_parser_1_1_explist_context_1aaf080d53e0d287f7012af74b1e7b47ab>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_explist_context_1a829e619bf8831243e623c0dda03f085f>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_explist_context_1a68205ae488aa599def14e283e5fd2358>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_explist_context_1ad2f24a8c566bd484fcb737145d10d664>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_explist_context_1a24e889f1b445ce8ab81590792dc7d495>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_explist_context_1aeb930c3b4fdb5dea2fb8d5e5ad4a0e76>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
