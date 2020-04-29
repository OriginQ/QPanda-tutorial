.. index:: pair: class; originirLexer
.. _doxid-classoriginir_lexer:

class originirLexer
===================

.. toctree::
	:hidden:

	struct_originirLexer_Initializer.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirLexer.h>
	
	class originirLexer: public Lexer
	{
	public:
		// enums
	
		enum
		{
		    :target:`PI<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa76df33505b1b978eb528b2dd7441a171>`                = 1,
		    :target:`QINIT_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fad0298e93a7ab1d7e5bc3e3251c84e8d1>`         = 2,
		    :target:`CREG_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa51c2d58be6421538d54360dd1e152ac0>`          = 3,
		    :target:`Q_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa24be92f8c65adf5b977a80d1b3f97c36>`             = 4,
		    :target:`C_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa7c48a44ad2e025e848f65a8b7a9f961b>`             = 5,
		    :target:`H_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fac3952819afe167bb5295799879559c56>`            = 6,
		    :target:`X_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa063a28a2aff174d3631ddb220f7e5aa7>`            = 7,
		    :target:`NOT_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fac3247dd3781b3b92cd332f85f96a1ac3>`          = 8,
		    :target:`T_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faff2c3127f3692de8a949996918385289>`            = 9,
		    :target:`S_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa87d69da2209a710f7cbd9fcfaaf22529>`            = 10,
		    :target:`Y_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faaa4c8c9f97d9a4c1411f0a5687936e35>`            = 11,
		    :target:`Z_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fab50373eb63cc54d5080391f86b5c1478>`            = 12,
		    :target:`X1_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa180283b6202b0cf6b706bf7921b427af>`           = 13,
		    :target:`Y1_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fadb9c024a4a482101d23a86bc741d7637>`           = 14,
		    :target:`Z1_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa84d8a7fee1129d6e048536d3ff361508>`           = 15,
		    :target:`I_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faf68cb39a1917adf52ac08eeed1fa4321>`            = 16,
		    :target:`U2_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faff374be1e8342194a7aa2ce9ee6ed88f>`           = 17,
		    :target:`U3_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa64feb4640e6751debf5ee9aba2faa06b>`           = 18,
		    :target:`U4_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa9abd9348ae2c2ee200dbd176262ff33a>`           = 19,
		    :target:`RX_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa198b0b3c4e03bfc5891552c213368619>`           = 20,
		    :target:`RY_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fade9ba355b6f25a22237bcb7bcbe457ce>`           = 21,
		    :target:`RZ_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fafae13851df79a8e027cacc43c78df16b>`           = 22,
		    :target:`U1_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fae7567c55a250b387b2081f7e78ce2861>`           = 23,
		    :target:`CNOT_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faba563048679e232305755cd30e30aaa1>`         = 24,
		    :target:`CZ_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faa07b05bbbf6570b631a34cfcca82c676>`           = 25,
		    :target:`CU_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa90e9f80653d395268ed552a669ccb8e7>`           = 26,
		    :target:`ISWAP_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa6b0a6ac6d2c844b1a6eae92e6bb03bc1>`        = 27,
		    :target:`SQISWAP_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa01838f608cf8f8d6b3acd47115b0b186>`      = 28,
		    :target:`SWAPZ1_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fafe8b07741b44ae081617b0bbf9d04a02>`       = 29,
		    :target:`ISWAPTHETA_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa81165af85a28355933cdcd9fbb7b1b70>`   = 30,
		    :target:`CR_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faf81f743de77d6262750e8d138d3bdc5d>`           = 31,
		    :target:`TOFFOLI_GATE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa66aae6af4cafd9c984bedf1e966c65d6>`      = 32,
		    :target:`DAGGER_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa1fdf541047c72c8e6a1157daee5165cc>`        = 33,
		    :target:`ENDDAGGER_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa193fc7e24f7644361d4fc6d247d7a371>`     = 34,
		    :target:`CONTROL_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa13bcd63b43cd033893e28b6d52d50921>`       = 35,
		    :target:`ENDCONTROL_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa91ee35c0bb38a6013cbf318b4a91bec8>`    = 36,
		    :target:`QIF_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa0e3831ce83383889acbbc94c041d2067>`           = 37,
		    :target:`ELSE_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa13cff405b92435cfe0e41565420422bc>`          = 38,
		    :target:`ENDIF_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faaea000e714840c1a8a6270f612220090>`         = 39,
		    :target:`QWHILE_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa6534b5a84ba0a1dc0b82eafa1c60fbb9>`        = 40,
		    :target:`ENDQWHILE_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fab3a8ab69bcd88d364cbec86adece66b1>`     = 41,
		    :target:`MEASURE_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa56374c9e7ad19ed379ef27494dcac7b0>`       = 42,
		    :target:`RESET_KEY<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fab148ae4f16d813c976f1f0f17d5831e9>`         = 43,
		    :target:`ASSIGN<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fafdbcc75fea62240f9c983cab966b9cac>`            = 44,
		    :target:`GT<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa3ba647dbc0712855024fc3b36cc4b41f>`                = 45,
		    :target:`LT<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa2cdcaf582cf93687f6bf3abe186f9747>`                = 46,
		    :target:`NOT<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa43772dd65c4145550a3e0742c5605b74>`               = 47,
		    :target:`EQ<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fac32895732d5a78a71b57877ad2526c16>`                = 48,
		    :target:`LEQ<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa617b2e393c42fe1d28efbadc777d2114>`               = 49,
		    :target:`GEQ<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa30fa7ee8e7cd05e8a1c9b39a2daa73e0>`               = 50,
		    :target:`NE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa1bbf7e6ceef17531a7ba63fc156c151e>`                = 51,
		    :target:`AND<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa99202d1a4929771c53d22ad28fcdab0d>`               = 52,
		    :target:`OR<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa6f05611b88e0454c4c91376ed632e6ac>`                = 53,
		    :target:`PLUS<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa5b1755c42dfa89b04597349bb188f79a>`              = 54,
		    :target:`MINUS<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fabcfa9a70e7e8fad681ea9bc17bbc7938>`             = 55,
		    :target:`MUL<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faca66fde27fd2f41ed10cdfab6d95b7c1>`               = 56,
		    :target:`DIV<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faef180a63678736138bef4b3edd71c04c>`               = 57,
		    :target:`COMMA<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa2f14c685fd218c39e9ae7dc2944304e6>`             = 58,
		    :target:`LPAREN<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faf8f68c19182ea84810e19f902aaeb912>`            = 59,
		    :target:`RPAREN<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa1198d1cfdd36fbb5cc71aade61105718>`            = 60,
		    :target:`LBRACK<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa730df026681fcff7c2b4b0aa7b586ded>`            = 61,
		    :target:`RBRACK<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa801c5534b63bf74b33f92657a058a0cd>`            = 62,
		    :target:`NEWLINE<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa4a216d8ea86dd060827ff7e6b3f90525>`           = 63,
		    :target:`Identifier<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa49c4c11ad519179c5845a8667a6af845>`        = 64,
		    :target:`Integer_Literal<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa9d3141231fa8c114935d79613e9e3c74>`   = 65,
		    :target:`Double_Literal<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746faf2058a795446122e58c357d6add3dc43>`    = 66,
		    :target:`Digit_Sequence<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fab29af36a5d839098484802477776bd37>`    = 67,
		    :target:`WhiteSpace<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa38d41d77ce47c610f87f8d2924789851>`        = 68,
		    :target:`SingleLineComment<doxid-classoriginir_lexer_1a5362befd82d7ef5299a5cc3190ae746fa703302c781d7241f514524a4229b71df>` = 69,
		};

		// structs
	
		struct :ref:`Initializer<doxid-structoriginir_lexer_1_1_initializer>`;

		// construction
	
		:target:`originirLexer<doxid-classoriginir_lexer_1ad8d66940b72e98d001f427e74219d1ba>`(antlr4::CharStream* input);

		// methods
	
		virtual std::string :target:`getGrammarFileName<doxid-classoriginir_lexer_1a60b1167d52dcb67a2b81725993c8e51d>`() const;
		virtual const std::vector<std::string>& :target:`getRuleNames<doxid-classoriginir_lexer_1acc8c427fcc64f6ed1129cc3de48c1a03>`() const;
		virtual const std::vector<std::string>& :target:`getChannelNames<doxid-classoriginir_lexer_1a5bf6f458226824330ac52dc20d981239>`() const;
		virtual const std::vector<std::string>& :target:`getModeNames<doxid-classoriginir_lexer_1a79425e1f798de62a1e6e5cde95d74049>`() const;
		virtual const std::vector<std::string>& :target:`getTokenNames<doxid-classoriginir_lexer_1ab3041329c6a0612289ed03b12a4ba95d>`() const;
		virtual antlr4::dfa::Vocabulary& :target:`getVocabulary<doxid-classoriginir_lexer_1ab51a198e180ef23f52be814a399b3207>`() const;
		virtual const std::vector<uint16_t> :target:`getSerializedATN<doxid-classoriginir_lexer_1a154d4d4bc8c7b600122ab46c3ae23f6c>`() const;
		virtual const antlr4::atn::ATN& :target:`getATN<doxid-classoriginir_lexer_1aac8993d377e84ed22b9a514fce9651a1>`() const;
	};
