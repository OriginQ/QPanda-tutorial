.. index:: pair: class; originirParser::Id_listContext
.. _doxid-classoriginir_parser_1_1_id__list_context:

class originirParser::Id_listContext
====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Id_listContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Id_listContext<doxid-classoriginir_parser_1_1_id__list_context_1a2fdad94f2ed226095d594b5aed790dc7>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classoriginir_parser_1_1_id__list_context_1a260fae0cb8127acc8cfafc4509583af6>`() const;
		std::vector<:ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`*> :target:`id<doxid-classoriginir_parser_1_1_id__list_context_1a2647961e586b7ec9fef6760443b253cb>`();
		:ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`* :target:`id<doxid-classoriginir_parser_1_1_id__list_context_1a018554b14ca9e5d60c2d97fa3fc636ba>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classoriginir_parser_1_1_id__list_context_1a47f77d7170c5aabf567b2d9402274904>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classoriginir_parser_1_1_id__list_context_1a94397e280bfa767edaf8b8b5f0b13ee1>`(size_t i);
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_id__list_context_1a944692abc1a95d8784d595c9468fcbeb>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_id__list_context_1a184bef6da070d4d81a6b2406e9457d9c>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_id__list_context_1a33898be97c3b5d6711b7df133eee02c1>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
