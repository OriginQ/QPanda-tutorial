.. index:: pair: class; qasmParser::Reg_declContext
.. _doxid-classqasm_parser_1_1_reg__decl_context:

class qasmParser::Reg_declContext
=================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class Reg_declContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context_1a594c0d4912907d790d01e21ce5c2e376>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_reg__decl_context_1a775350c64909d93d754c539b483c2c43>`() const;
		antlr4::tree::TerminalNode* :target:`QREG_KEY<doxid-classqasm_parser_1_1_reg__decl_context_1aed80cb36aef2698452f5b096b876a48a>`();
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1_1_reg__decl_context_1acd7594b8468fc385475099e929f86af0>`();
		antlr4::tree::TerminalNode* :target:`LBRACKET<doxid-classqasm_parser_1_1_reg__decl_context_1a2c1ab317b90e7eab6863bbc50cf2f91b>`();
		:ref:`IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* :target:`integer<doxid-classqasm_parser_1_1_reg__decl_context_1a24fb1b55f2bba3c8e5842da0707821cf>`();
		antlr4::tree::TerminalNode* :target:`RBRACKET<doxid-classqasm_parser_1_1_reg__decl_context_1a1f8d1b7e93777a0291505e12cf632821>`();
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_reg__decl_context_1a52f258e0aae4b9398a436d0c201b206a>`();
		antlr4::tree::TerminalNode* :target:`CREG_KEY<doxid-classqasm_parser_1_1_reg__decl_context_1a3fdbbfb27a8a31121f4eed2211df391e>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_reg__decl_context_1a3ef1cba0e140e271139b43ff91c45b78>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_reg__decl_context_1abd81581f111d7685ff606cf3685777ae>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_reg__decl_context_1a80b1edc4e2cf479820cf976131f3d243>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
