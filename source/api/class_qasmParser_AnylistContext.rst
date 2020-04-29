.. index:: pair: class; qasmParser::AnylistContext
.. _doxid-classqasm_parser_1_1_anylist_context:

class qasmParser::AnylistContext
================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class AnylistContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`AnylistContext<doxid-classqasm_parser_1_1_anylist_context_1a23ce1c731fdbe46766c36eecfe027f77>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_anylist_context_1ab79d217d78707ff300fa19db68a7f789>`() const;
		std::vector<:ref:`Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`*> :target:`id_index<doxid-classqasm_parser_1_1_anylist_context_1a3d27f879e8ce10a463c434872e0b5d80>`();
		:ref:`Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* :target:`id_index<doxid-classqasm_parser_1_1_anylist_context_1a90d45a8930deed68dfee47ce38c1c83b>`(size_t i);
		std::vector<:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`*> :target:`id<doxid-classqasm_parser_1_1_anylist_context_1a0116ff39256d856ca94d4504138b0471>`();
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_anylist_context_1afd19d2c399c9b74172f39d5671ae462f>`(size_t i);
		std::vector<antlr4::tree::TerminalNode*> :target:`COMMA<doxid-classqasm_parser_1_1_anylist_context_1a9ccebb5008253c984bb1c9c8941cf499>`();
		antlr4::tree::TerminalNode* :target:`COMMA<doxid-classqasm_parser_1_1_anylist_context_1a969bc7367311f9aed44bbfa56b368677>`(size_t i);
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_anylist_context_1a502d85c60489b0dabb51125afe4c72fd>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_anylist_context_1ab4d1aad959d3070522ad09d92a90ef55>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_anylist_context_1aede8d3b87e69f0f3bd8417c3e381026d>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
