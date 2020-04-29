.. index:: pair: class; originirParser::Pri_cstContext
.. _doxid-classoriginir_parser_1_1_pri__cst_context:

class originirParser::Pri_cstContext
====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Pri_cstContext: public :ref:`originirParser::Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`
	{
	public:
		// construction
	
		:target:`Pri_cstContext<doxid-classoriginir_parser_1_1_pri__cst_context_1a7c67dc099b5f15317a458d15d83bd088>`(:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* ctx);

		// methods
	
		:ref:`ConstantContext<doxid-classoriginir_parser_1_1_constant_context>`* :target:`constant<doxid-classoriginir_parser_1_1_pri__cst_context_1aee033435241602873ae344a5413927aa>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_pri__cst_context_1ac4be253365511f27a1a50e8162e954ad>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_pri__cst_context_1ac60a65b609b7f7cb0852b00c5704df59>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_pri__cst_context_1a83239d73c4e59caa09e107b435cba929>`(antlr4::tree::ParseTreeVisitor* visitor);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		void :ref:`copyFrom<doxid-classoriginir_parser_1_1_primary__expression_context_1aac335f00cc8b3a5c4f4831663e672850>`(:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* context);
		virtual size_t :ref:`getRuleIndex<doxid-classoriginir_parser_1_1_primary__expression_context_1a11fc39c65fe7cd7a38aacf26d18bddcc>`() const;

