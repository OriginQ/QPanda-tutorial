.. index:: pair: class; qasmLexer
.. _doxid-classqasm_lexer:

class qasmLexer
===============

.. toctree::
	:hidden:

	struct_qasmLexer_Initializer.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmLexer.h>
	
	class qasmLexer: public Lexer
	{
	public:
		// enums
	
		enum
		{
		    :target:`OPENQASM_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa0016a50595647aba249b1862f95c1a7a>` = 1,
		    :target:`INCLUDE_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6faa54ac604d5f478fe08abecca4ba9d47e>`  = 2,
		    :target:`OPAQUE_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fac3fdbf7ea91bbc5d966e6b61c96a108f>`   = 3,
		    :target:`QREG_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa5dc85a75b280d88318a6a4db529d8c10>`     = 4,
		    :target:`CREG_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa037b093407af996c1123ceb724a154a7>`     = 5,
		    :target:`BARRIER_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa85b61c560d06249814cb30cd52ed675a>`  = 6,
		    :target:`IF_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa714892fc38770ca96d198db06963416e>`       = 7,
		    :target:`MEASURE_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa9136a1ea900eb2404196309c3e8334b1>`  = 8,
		    :target:`RESET_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fab0d1b1a532fb23ff429b590448ee0e99>`    = 9,
		    :target:`GATE_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fabbc588202700211d6cb1c1a4198e6a43>`     = 10,
		    :target:`PI_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa6dfda548db212f94a2f09ca33e6b44e9>`       = 11,
		    :target:`U_GATE_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fae7cf2d96621846f2734d6012a41d649f>`   = 12,
		    :target:`CX_GATE_KEY<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa1ee616fba771b08fe23f0fef7e9d3962>`  = 13,
		    :target:`ARROW<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fafe5b479c2effa6bab86935cd493dc010>`        = 14,
		    :target:`EQ<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa0e0b8280c6d30c1103599c52137f25ad>`           = 15,
		    :target:`PLUS<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa33688e86d9f0a2b44d4144a588889f0b>`         = 16,
		    :target:`MINUS<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6faf0cd006ad82b194a44b43bc6745bdbec>`        = 17,
		    :target:`MUL<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa3c1201c752a6bec9b10db7872bab301b>`          = 18,
		    :target:`DIV<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa72178ff5e5b2681ab37cbff4aaa0045b>`          = 19,
		    :target:`COMMA<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa981d847d4855382c5fcc8ca00119f476>`        = 20,
		    :target:`SEMI<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6faa4c8654b94f8b7ca9107594bc2e65726>`         = 21,
		    :target:`LPAREN<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa3e73c24a9fc8ce5b9ee3576ad4730657>`       = 22,
		    :target:`RPAREN<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6faa4106bc3a4e791d5b0916f58713960a5>`       = 23,
		    :target:`LBRACKET<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa8afe4d99f99554c1dc06ef13619d18df>`     = 24,
		    :target:`RBRACKET<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa82977acec2d329a433e8d00532e008a5>`     = 25,
		    :target:`LBRACE<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa76cd051af2ffc2c344aef34a34ee8ce3>`       = 26,
		    :target:`RBRACE<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa53b0bcd78d411204d8f658497cd31c05>`       = 27,
		    :target:`DQM<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fadc75d0dcf873e00ad7098f6621680927>`          = 28,
		    :target:`IDENTIFIER<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa1ea3a61aeb743746489598f370b515ec>`   = 29,
		    :target:`INTEGER<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6faaefb59da1f6f940b05d8ca6d391fa3e1>`      = 30,
		    :target:`DECIMAL<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa85b7535138437cf4b1fbcd78fcffb5af>`      = 31,
		    :target:`FILENAME<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6faffcb26642180a524eb7d8a09409da927>`     = 32,
		    :target:`NL<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fab18bfecba0b0b20eb8f7e8803d9c98f5>`           = 33,
		    :target:`WS<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa1ece7e89058c3fa34dfbe5a382f82f89>`           = 34,
		    :target:`LC<doxid-classqasm_lexer_1ab6b346c32395d9cb157b9d23509d9b6fa63cf97a4241ef0b7308f3a6aaf714008>`           = 35,
		};

		// structs
	
		struct :ref:`Initializer<doxid-structqasm_lexer_1_1_initializer>`;

		// construction
	
		:target:`qasmLexer<doxid-classqasm_lexer_1a20fd53c777aaf326b7fd709f963465d0>`(antlr4::CharStream* input);

		// methods
	
		virtual std::string :target:`getGrammarFileName<doxid-classqasm_lexer_1a1268b9c9287e0e0d0dfd469d3bd6e8a3>`() const;
		virtual const std::vector<std::string>& :target:`getRuleNames<doxid-classqasm_lexer_1a9424bc24b1d35e4cbf583342d72a4e5a>`() const;
		virtual const std::vector<std::string>& :target:`getChannelNames<doxid-classqasm_lexer_1a36c6d04f5ce29bd8e8c5014e40731949>`() const;
		virtual const std::vector<std::string>& :target:`getModeNames<doxid-classqasm_lexer_1a292de6a966183151d07b1f2938a67816>`() const;
		virtual const std::vector<std::string>& :target:`getTokenNames<doxid-classqasm_lexer_1aa1ff2fd0784867b1689686fe2dd02019>`() const;
		virtual antlr4::dfa::Vocabulary& :target:`getVocabulary<doxid-classqasm_lexer_1ab99808522be309a4ba2768ce4f428647>`() const;
		virtual const std::vector<uint16_t> :target:`getSerializedATN<doxid-classqasm_lexer_1a7c6693c84832eeae4ee9bd28ca4bb2d7>`() const;
		virtual const antlr4::atn::ATN& :target:`getATN<doxid-classqasm_lexer_1a618da4227b3f9d4aedb5bfe8e799688f>`() const;
	};
