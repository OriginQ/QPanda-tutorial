.. index:: pair: class; originirParser::Pri_ckeyContext
.. _doxid-classoriginir_parser_1_1_pri__ckey_context:

class originirParser::Pri_ckeyContext
=====================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class Pri_ckeyContext: public :ref:`originirParser::Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`
	{
	public:
		// construction
	
		:target:`Pri_ckeyContext<doxid-classoriginir_parser_1_1_pri__ckey_context_1a98a03c69b9d570ea3d12e9929243a36b>`(:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* ctx);

		// methods
	
		:ref:`C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`* :target:`c_KEY_declaration<doxid-classoriginir_parser_1_1_pri__ckey_context_1a27481495e9b5f2a3cc9740b5a6828790>`();
		virtual void :target:`enterRule<doxid-classoriginir_parser_1_1_pri__ckey_context_1a21afd46639deb5730807866ecbb4ea8e>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classoriginir_parser_1_1_pri__ckey_context_1ae31ef89891b3f2659c15bcc0b59ad7d4>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classoriginir_parser_1_1_pri__ckey_context_1a145a3ea2eeb84e6dcfcc16a098b1fcd8>`(antlr4::tree::ParseTreeVisitor* visitor);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		void :ref:`copyFrom<doxid-classoriginir_parser_1_1_primary__expression_context_1aac335f00cc8b3a5c4f4831663e672850>`(:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* context);
		virtual size_t :ref:`getRuleIndex<doxid-classoriginir_parser_1_1_primary__expression_context_1a11fc39c65fe7cd7a38aacf26d18bddcc>`() const;

