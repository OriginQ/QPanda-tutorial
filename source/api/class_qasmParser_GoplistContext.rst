.. index:: pair: class; qasmParser::GoplistContext
.. _doxid-classqasm_parser_1_1_goplist_context:

class qasmParser::GoplistContext
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class GoplistContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`GoplistContext<doxid-classqasm_parser_1_1_goplist_context_1a7ab49122a992a147f6c77d7deb0285a4>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_goplist_context_1a326acd34ccf948325458abcfc1993b60>`() const;
		std::vector<:ref:`UopContext<doxid-classqasm_parser_1_1_uop_context>`*> :target:`uop<doxid-classqasm_parser_1_1_goplist_context_1ac1692a68dbdb4d2091debbf6bad4a120>`();
		:ref:`UopContext<doxid-classqasm_parser_1_1_uop_context>`* :target:`uop<doxid-classqasm_parser_1_1_goplist_context_1abd5a814edea32ae850978ce8107226bc>`(size_t i);
		std::vector<:ref:`BopContext<doxid-classqasm_parser_1_1_bop_context>`*> :target:`bop<doxid-classqasm_parser_1_1_goplist_context_1af7b2bb13b907e16422ad1fd7dfa0faf1>`();
		:ref:`BopContext<doxid-classqasm_parser_1_1_bop_context>`* :target:`bop<doxid-classqasm_parser_1_1_goplist_context_1ad1788aea83057c5d7dea08cb6080650b>`(size_t i);
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_goplist_context_1a75ef37f72b992fefbc9f9032c38ccfa0>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_goplist_context_1ac096989b04ee94b90f459d7e8a0e62c6>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_goplist_context_1a516c7c94c07935ac34b41a03330be7a9>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
