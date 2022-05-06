.. index:: pair: class; originirParser
.. _doxid-classoriginir_parser:

class originirParser
====================

.. toctree::
	:hidden:

	struct_originirParser_Initializer.rst
	class_originirParser_Addtive_expressionContext.rst
	class_originirParser_Assignment_expressionContext.rst
	class_originirParser_Barrier_statementContext.rst
	class_originirParser_C_KEY_declarationContext.rst
	class_originirParser_Cinit_declarationContext.rst
	class_originirParser_ConstantContext.rst
	class_originirParser_Control_statementContext.rst
	class_originirParser_Controlbit_listContext.rst
	class_originirParser_Dagger_statementContext.rst
	class_originirParser_DeclarationContext.rst
	class_originirParser_Define_gate_declarationContext.rst
	class_originirParser_Define_gate_statementContext.rst
	class_originirParser_Double_gate_with_four_parameter_declarationContext.rst
	class_originirParser_Double_gate_with_four_parameter_typeContext.rst
	class_originirParser_Double_gate_with_one_parameter_declarationContext.rst
	class_originirParser_Double_gate_with_one_parameter_typeContext.rst
	class_originirParser_Double_gate_without_parameter_declarationContext.rst
	class_originirParser_Double_gate_without_parameter_typeContext.rst
	class_originirParser_Equality_expressionContext.rst
	class_originirParser_ExpContext.rst
	class_originirParser_ExplistContext.rst
	class_originirParser_ExpressionContext.rst
	class_originirParser_Expression_statementContext.rst
	class_originirParser_Gate_func_statementContext.rst
	class_originirParser_Gate_nameContext.rst
	class_originirParser_IdContext.rst
	class_originirParser_Id_listContext.rst
	class_originirParser_IndexContext.rst
	class_originirParser_Logical_and_expressionContext.rst
	class_originirParser_Logical_or_expressionContext.rst
	class_originirParser_Measure_statementContext.rst
	class_originirParser_Multiplicative_expressionContext.rst
	class_originirParser_Pri_ckeyContext.rst
	class_originirParser_Pri_cstContext.rst
	class_originirParser_Pri_exprContext.rst
	class_originirParser_Primary_expressionContext.rst
	class_originirParser_Q_KEY_declarationContext.rst
	class_originirParser_Qelse_statement_fragmentContext.rst
	class_originirParser_Qif_ifContext.rst
	class_originirParser_Qif_ifelseContext.rst
	class_originirParser_Qif_statementContext.rst
	class_originirParser_Qinit_declarationContext.rst
	class_originirParser_Quantum_gate_declarationContext.rst
	class_originirParser_Qwhile_statementContext.rst
	class_originirParser_Relational_expressionContext.rst
	class_originirParser_Reset_statementContext.rst
	class_originirParser_Single_gate_with_four_parameter_declarationContext.rst
	class_originirParser_Single_gate_with_four_parameter_typeContext.rst
	class_originirParser_Single_gate_with_one_parameter_declarationContext.rst
	class_originirParser_Single_gate_with_one_parameter_typeContext.rst
	class_originirParser_Single_gate_with_three_parameter_declarationContext.rst
	class_originirParser_Single_gate_with_three_parameter_typeContext.rst
	class_originirParser_Single_gate_with_two_parameter_declarationContext.rst
	class_originirParser_Single_gate_with_two_parameter_typeContext.rst
	class_originirParser_Single_gate_without_parameter_declarationContext.rst
	class_originirParser_Single_gate_without_parameter_typeContext.rst
	class_originirParser_StatementContext.rst
	class_originirParser_TranslationunitContext.rst
	class_originirParser_Triple_gate_without_parameter_declarationContext.rst
	class_originirParser_Triple_gate_without_parameter_typeContext.rst
	class_originirParser_Unary_expressionContext.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <originirParser.h>
	
	class originirParser: public Parser
	{
	public:
		// enums
	
		enum
		{
		    :target:`PI<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aaf8a00d3676daf16a236fab78157b531>`                = 1,
		    :target:`QINIT_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a8fade9ccc9234e3a5cc0fd5d8f3a90dc>`         = 2,
		    :target:`CREG_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a82f2ec68e4b9b7383bd570799836f916>`          = 3,
		    :target:`Q_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ab0875cde5d9a46411f4f52a7fa42140f>`             = 4,
		    :target:`C_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aed3a2fc8b258da0d05f01c7810e999e1>`             = 5,
		    :target:`BARRIER_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ad9e625dcb2cfbd2874593c5aab124985>`       = 6,
		    :target:`QGATE_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a8d496ac93136c53f25c1ae4a6bc5d58d>`         = 7,
		    :target:`ENDQGATE_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a54deaf3c31789769ef099719e9453e9f>`      = 8,
		    :target:`ECHO_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aaec990b3c0773e6d5a3de42a868add98>`         = 9,
		    :target:`H_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a251250b0ebd89ea82ff3d1841cb2dd84>`            = 10,
		    :target:`X_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ac54e52343c1812f0e2e76d45227bd55f>`            = 11,
		    :target:`NOT_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a8bf24b976f8e4ff4028546fdb0c94268>`          = 12,
		    :target:`T_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a4bae47a9171a233e0f72e20401c0f921>`            = 13,
		    :target:`S_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a2ea0e1d59de60a1129f455c3fa9b42ad>`            = 14,
		    :target:`Y_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aa5750af5148ff9c822617eec523514f5>`            = 15,
		    :target:`Z_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a2043e21a4b3bc35f5bd8eb052b0869cf>`            = 16,
		    :target:`X1_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ad7250cbfd30470a182fc38ea5d8d9c35>`           = 17,
		    :target:`Y1_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a34c6ecdcfc807373f224c218cfba9a5a>`           = 18,
		    :target:`Z1_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aad317797683c40710c4270206fae6fe2>`           = 19,
		    :target:`I_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a01a0edc71d836bba892c73a66ebdd6ad>`            = 20,
		    :target:`U2_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a9952932eaa502389c2b7d30ecfa6e8d6>`           = 21,
		    :target:`RPHI_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a3629c0724dca116aadf8ef39846eb29c>`         = 22,
		    :target:`U3_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7adb77091bc0ab5e9f9e95e7640818f360>`           = 23,
		    :target:`U4_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a859d819d8929c513cc57720993d5d9c5>`           = 24,
		    :target:`RX_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7af30895b0d239cfa27db723065d79abe7>`           = 25,
		    :target:`RY_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aa43df8d075b0ae295d747df6a4e34f23>`           = 26,
		    :target:`RZ_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aa92da7351e5fa9003f94fc6b0481a077>`           = 27,
		    :target:`U1_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ae33e0f4af2711a9cbd2772780c8117c9>`           = 28,
		    :target:`CNOT_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a173af6fed1153ad4016e1874fb648708>`         = 29,
		    :target:`CZ_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a8972980e6aa195d19bf32b6e083d4798>`           = 30,
		    :target:`CU_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a33e9d77786ffb5cec5ee51ae6cb82308>`           = 31,
		    :target:`ISWAP_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a82c8bd7540afa601d8db7c3350e6fee5>`        = 32,
		    :target:`SQISWAP_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a14384749a9eb9104bd036f94e189e8d5>`      = 33,
		    :target:`SWAPZ1_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ae7d89a5febabcdaf63e58fc49b493a79>`       = 34,
		    :target:`ISWAPTHETA_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ad504059c4fd96f0be7f9886506fbeeaf>`   = 35,
		    :target:`CR_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a8d4f6b71708263807798527ceacf6e75>`           = 36,
		    :target:`TOFFOLI_GATE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a7a6358697440055c7de38fbc49b5eff6>`      = 37,
		    :target:`DAGGER_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ae6a50a3055094a45450f1587d04b8201>`        = 38,
		    :target:`ENDDAGGER_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a4b361d83d1c284ed95e681c1b335dbc9>`     = 39,
		    :target:`CONTROL_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a674f391c179f972b2c26dba06a4fbc12>`       = 40,
		    :target:`ENDCONTROL_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a6df501cd440fb28d0aba849fe67d1a9d>`    = 41,
		    :target:`QIF_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a0f8d4a16126b93bc961f7f142a45aa11>`           = 42,
		    :target:`ELSE_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ab451f0ea001babaeec0e54b3cfce9c82>`          = 43,
		    :target:`ENDIF_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a3afe4c7d31c5575fdd379224eaed9865>`         = 44,
		    :target:`QWHILE_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7adeaecce5499d8ab2c46b813755b84919>`        = 45,
		    :target:`ENDQWHILE_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a7113dbe33ecb60d401bf9de150b75f2c>`     = 46,
		    :target:`MEASURE_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7afa507c1d058d6b3a78b97a109a7e34b3>`       = 47,
		    :target:`RESET_KEY<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ab4b40c7b0c8c39f638d4cb59cd23a9aa>`         = 48,
		    :target:`ASSIGN<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a949291fed779cdb530ea700a089d94d0>`            = 49,
		    :target:`GT<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a12935acb510d95c213afe1e6db2edc49>`                = 50,
		    :target:`LT<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a8a76183a5f81da1c9a9a27695cad897e>`                = 51,
		    :target:`NOT<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a4548a01d1b6b997f60339d580f3a8ed1>`               = 52,
		    :target:`EQ<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a458b73b129b017b35110a71c597ceace>`                = 53,
		    :target:`LEQ<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a0f61b27efdb09de4beb14b62c0953b34>`               = 54,
		    :target:`GEQ<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a930456262322985ec7d25a2ee3bba46a>`               = 55,
		    :target:`NE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a7766fb8bbe23069783e60f9a09ec974b>`                = 56,
		    :target:`AND<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aadc38bd26ea275535bfee4eb7c27f1e5>`               = 57,
		    :target:`OR<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a0cb47f894e8f82591727aab3638c343f>`                = 58,
		    :target:`PLUS<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ac933de53213b39a89715a9b64a801c70>`              = 59,
		    :target:`MINUS<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ab91c303cced206d7d1543e5c0158ab27>`             = 60,
		    :target:`MUL<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a107656e0e9632db1a5d00d7ff94730f9>`               = 61,
		    :target:`DIV<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a36df984e2d06b6ef89d6c9c053839e1f>`               = 62,
		    :target:`COMMA<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a870a332931d41201b1e6ebb324be0852>`             = 63,
		    :target:`LPAREN<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a065dd236020be81b8e74d8dd2f9d59bd>`            = 64,
		    :target:`RPAREN<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a9445bc3663c4bbc4b0e19743c05c0a2c>`            = 65,
		    :target:`LBRACK<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a1dcf24b2013b64310359ac09a4e9d349>`            = 66,
		    :target:`RBRACK<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a89c23004aa19f708d843fd64dc7a4382>`            = 67,
		    :target:`NEWLINE<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a91d11145a1821c4ee60c1f34fbc1b8ed>`           = 68,
		    :target:`Identifier<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7aec43a85e70e3c9622892b96114a71c59>`        = 69,
		    :target:`Integer_Literal<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a7ac349271ee2c457786cb96ffcf37b99>`   = 70,
		    :target:`Double_Literal<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a4bb0d794bf5e4464785fd8ea8dd9553c>`    = 71,
		    :target:`Digit_Sequence<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a20cfe95be5a94f294acdc9a338d4c211>`    = 72,
		    :target:`REALEXP<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7afe7f9b6841252011f1c89b2cd266da9d>`           = 73,
		    :target:`WhiteSpace<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7ab0e6b8da2516d76cf523b17cf1ea28e1>`        = 74,
		    :target:`SingleLineComment<doxid-classoriginir_parser_1a6c63a76912a68b9e1407c71f8d6733f7a805e4c6de62bee5c7053abde6d91cbc8>` = 75,
		};
	
		enum
		{
		    :target:`RuleTranslationunit<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675afb396ee73ef7af83b79149557be095d4>`                              = 0,
		    :target:`RuleDeclaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675aa94e9bf182ba9056797a306275d65063>`                                  = 1,
		    :target:`RuleQinit_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a3e97b49cbd5d4d4bbe7b623bb5616712>`                            = 2,
		    :target:`RuleCinit_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a72ac8c8db5915608584cfb4a1f7162ab>`                            = 3,
		    :target:`RuleQuantum_gate_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ae784d7541a00c7fe11dbee9ab3bdff45>`                     = 4,
		    :target:`RuleIndex<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a6df3d40016dbc2133229e55d8f5540e3>`                                        = 5,
		    :target:`RuleC_KEY_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675afdc26faccb951d22c47c18ab4b1032dd>`                            = 6,
		    :target:`RuleQ_KEY_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a69e289ed47a6600eaadfbdf0e1b48958>`                            = 7,
		    :target:`RuleSingle_gate_without_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a08596fe0f6bf8f4f52f2e9976db57812>`    = 8,
		    :target:`RuleSingle_gate_with_one_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a3b079a9602a272864148165c321c26bd>`   = 9,
		    :target:`RuleSingle_gate_with_two_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675aefd78d2f6f87e0189036fce65f0f915c>`   = 10,
		    :target:`RuleSingle_gate_with_three_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a4bb07e69c97e509711a01e1dd872f113>` = 11,
		    :target:`RuleSingle_gate_with_four_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a68dbd55aa308b35df8c5c960ab6dc4f4>`  = 12,
		    :target:`RuleDouble_gate_without_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a802755e7d4106cf23f6617a824c118ad>`    = 13,
		    :target:`RuleDouble_gate_with_one_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a512c5c9910daac802ae977fa73c22107>`   = 14,
		    :target:`RuleDouble_gate_with_four_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a9de93c4732717f81aa92d0d9ddcbd10b>`  = 15,
		    :target:`RuleTriple_gate_without_parameter_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a6a8e1b29f4931518a43bbe41bad6eaec>`    = 16,
		    :target:`RuleDefine_gate_declaration<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a4948945352e26e72930b5652aeb5dfce>`                      = 17,
		    :target:`RuleSingle_gate_without_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a92cb81423008de35ec669930c328255f>`           = 18,
		    :target:`RuleSingle_gate_with_one_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a885145a23aa3e27c08e46fdd5d5d7172>`          = 19,
		    :target:`RuleSingle_gate_with_two_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a51294a3ccd2818e1a62d5de07d263dda>`          = 20,
		    :target:`RuleSingle_gate_with_three_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a9890fc438fd57e2f5439bda215097429>`        = 21,
		    :target:`RuleSingle_gate_with_four_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a669067a61331bae73dde916a58a4178a>`         = 22,
		    :target:`RuleDouble_gate_without_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a14d2fb5ab1b629eb996b26f3ef146a28>`           = 23,
		    :target:`RuleDouble_gate_with_one_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675af95c66b51ddbcb0c4d017dcc77290a0d>`          = 24,
		    :target:`RuleDouble_gate_with_four_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ac89c729822c0c9780029cf6ada983a64>`         = 25,
		    :target:`RuleTriple_gate_without_parameter_type<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a8f4f83445f61a3e0338cd12fafa041a7>`           = 26,
		    :target:`RulePrimary_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675aee09171ab15819959689f33dc266bdba>`                           = 27,
		    :target:`RuleUnary_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a13725ac263d7b3181bde0e02bac65ea8>`                             = 28,
		    :target:`RuleMultiplicative_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a49b1a4d4ecf70e629fc086e2d7efc7fc>`                    = 29,
		    :target:`RuleAddtive_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ab9378e1c57520fb92681f9f389e34b91>`                           = 30,
		    :target:`RuleRelational_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a1449db28e2842bc8c31db1a310bfd5cd>`                        = 31,
		    :target:`RuleEquality_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675acd51a34e1880c6d43aa3b6fd0a4cc074>`                          = 32,
		    :target:`RuleLogical_and_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ad91eee2252f2f1afdf9f7b08047271e1>`                       = 33,
		    :target:`RuleLogical_or_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675af61c55551da060dc4e3007db10929dd8>`                        = 34,
		    :target:`RuleAssignment_expression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675abcc81cf7366131e9dac80ccbcdbf240f>`                        = 35,
		    :target:`RuleExpression<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a7586369067b1fc21b9507a6211f8706f>`                                   = 36,
		    :target:`RuleControlbit_list<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675abf9abe16195d862b197b82b36a6755d5>`                              = 37,
		    :target:`RuleStatement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675abc950e50903afa9cfdd4dc1f2aaeaa19>`                                    = 38,
		    :target:`RuleDagger_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a1c44da9f08679eaf0e7a7ab794f939c7>`                             = 39,
		    :target:`RuleControl_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a39e9f2d8cac144fe0debef61e22809a2>`                            = 40,
		    :target:`RuleQelse_statement_fragment<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ac782594c153ae4baca9cea37fb60b950>`                     = 41,
		    :target:`RuleQif_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ab496b9ab9ee3a7b4ef10821f966dee7c>`                                = 42,
		    :target:`RuleQwhile_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ad2fcbcb0a29e0cd7ff13ca6ed7f1856f>`                             = 43,
		    :target:`RuleMeasure_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675aeab05a6e01ee4ee28e85a7709f5b1754>`                            = 44,
		    :target:`RuleReset_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a250e3fe98f1bbd17c0e946f7053d3b76>`                              = 45,
		    :target:`RuleBarrier_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ab07fa13fae49f91309e455028fd02a36>`                            = 46,
		    :target:`RuleExpression_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ab45446a044897eefa16affd1304dc811>`                         = 47,
		    :target:`RuleDefine_gate_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a512ae56e1708479f8705856c91dc5df7>`                        = 48,
		    :target:`RuleExplist<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675abed1284582670724740b4e8264309dd2>`                                      = 49,
		    :target:`RuleExp<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a185d75cc8c12952f50d5a0f0ed6727b2>`                                          = 50,
		    :target:`RuleGate_func_statement<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a1e3a0ef0ab76e9ba7d6db230f9fbbe95>`                          = 51,
		    :target:`RuleId<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a9529cc956524b862b140a4dbcfa695f3>`                                           = 52,
		    :target:`RuleId_list<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a9c322e8df599dc5713899915cc10eb46>`                                      = 53,
		    :target:`RuleGate_name<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675a2f9afc4663bf13c68f00d64a16d638f7>`                                    = 54,
		    :target:`RuleConstant<doxid-classoriginir_parser_1ad7515bc4a2971425b5da6fd295e47675ae108ecdc365430b16f177ed004a06491>`                                     = 55,
		};

		// structs
	
		struct :ref:`Initializer<doxid-structoriginir_parser_1_1_initializer>`;

		// classes
	
		class :ref:`Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`;
		class :ref:`Assignment_expressionContext<doxid-classoriginir_parser_1_1_assignment__expression_context>`;
		class :ref:`Barrier_statementContext<doxid-classoriginir_parser_1_1_barrier__statement_context>`;
		class :ref:`C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`;
		class :ref:`Cinit_declarationContext<doxid-classoriginir_parser_1_1_cinit__declaration_context>`;
		class :ref:`ConstantContext<doxid-classoriginir_parser_1_1_constant_context>`;
		class :ref:`Control_statementContext<doxid-classoriginir_parser_1_1_control__statement_context>`;
		class :ref:`Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context>`;
		class :ref:`Dagger_statementContext<doxid-classoriginir_parser_1_1_dagger__statement_context>`;
		class :ref:`DeclarationContext<doxid-classoriginir_parser_1_1_declaration_context>`;
		class :ref:`Define_gate_declarationContext<doxid-classoriginir_parser_1_1_define__gate__declaration_context>`;
		class :ref:`Define_gate_statementContext<doxid-classoriginir_parser_1_1_define__gate__statement_context>`;
		class :ref:`Double_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context>`;
		class :ref:`Double_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__type_context>`;
		class :ref:`Double_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context>`;
		class :ref:`Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context>`;
		class :ref:`Double_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context>`;
		class :ref:`Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context>`;
		class :ref:`Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`;
		class :ref:`ExpContext<doxid-classoriginir_parser_1_1_exp_context>`;
		class :ref:`ExplistContext<doxid-classoriginir_parser_1_1_explist_context>`;
		class :ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`;
		class :ref:`Expression_statementContext<doxid-classoriginir_parser_1_1_expression__statement_context>`;
		class :ref:`Gate_func_statementContext<doxid-classoriginir_parser_1_1_gate__func__statement_context>`;
		class :ref:`Gate_nameContext<doxid-classoriginir_parser_1_1_gate__name_context>`;
		class :ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`;
		class :ref:`Id_listContext<doxid-classoriginir_parser_1_1_id__list_context>`;
		class :ref:`IndexContext<doxid-classoriginir_parser_1_1_index_context>`;
		class :ref:`Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`;
		class :ref:`Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`;
		class :ref:`Measure_statementContext<doxid-classoriginir_parser_1_1_measure__statement_context>`;
		class :ref:`Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`;
		class :ref:`Pri_ckeyContext<doxid-classoriginir_parser_1_1_pri__ckey_context>`;
		class :ref:`Pri_cstContext<doxid-classoriginir_parser_1_1_pri__cst_context>`;
		class :ref:`Pri_exprContext<doxid-classoriginir_parser_1_1_pri__expr_context>`;
		class :ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`;
		class :ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`;
		class :ref:`Qelse_statement_fragmentContext<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context>`;
		class :ref:`Qif_ifContext<doxid-classoriginir_parser_1_1_qif__if_context>`;
		class :ref:`Qif_ifelseContext<doxid-classoriginir_parser_1_1_qif__ifelse_context>`;
		class :ref:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`;
		class :ref:`Qinit_declarationContext<doxid-classoriginir_parser_1_1_qinit__declaration_context>`;
		class :ref:`Quantum_gate_declarationContext<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context>`;
		class :ref:`Qwhile_statementContext<doxid-classoriginir_parser_1_1_qwhile__statement_context>`;
		class :ref:`Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`;
		class :ref:`Reset_statementContext<doxid-classoriginir_parser_1_1_reset__statement_context>`;
		class :ref:`Single_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context>`;
		class :ref:`Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context>`;
		class :ref:`Single_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context>`;
		class :ref:`Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context>`;
		class :ref:`Single_gate_with_three_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context>`;
		class :ref:`Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context>`;
		class :ref:`Single_gate_with_two_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context>`;
		class :ref:`Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context>`;
		class :ref:`Single_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context>`;
		class :ref:`Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context>`;
		class :ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`;
		class :ref:`TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context>`;
		class :ref:`Triple_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context>`;
		class :ref:`Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context>`;
		class :ref:`Unary_expressionContext<doxid-classoriginir_parser_1_1_unary__expression_context>`;

		// construction
	
		:target:`originirParser<doxid-classoriginir_parser_1a3763a88ee61d6260a74fabde3ee08d23>`(antlr4::TokenStream* input);

		// methods
	
		virtual std::string :target:`getGrammarFileName<doxid-classoriginir_parser_1afb996cd7d6ea6162687ed06730252b1c>`() const;
		virtual const antlr4::atn::ATN& :target:`getATN<doxid-classoriginir_parser_1a8db7e9bdab3cf0a1cf8771061896b9a7>`() const;
		virtual const std::vector<std::string>& :target:`getTokenNames<doxid-classoriginir_parser_1aeb76e2f92d92ec74758c855ae2af6546>`() const;
		virtual const std::vector<std::string>& :target:`getRuleNames<doxid-classoriginir_parser_1a0916335c912fbd772aac7ec2c4e2e99b>`() const;
		virtual antlr4::dfa::Vocabulary& :target:`getVocabulary<doxid-classoriginir_parser_1a982a7b2a969840838239f0ac5a28da12>`() const;
		:ref:`TranslationunitContext<doxid-classoriginir_parser_1_1_translationunit_context>`* :target:`translationunit<doxid-classoriginir_parser_1af57569ab832f3f312e7c02aab2df7bae>`();
		:ref:`DeclarationContext<doxid-classoriginir_parser_1_1_declaration_context>`* :target:`declaration<doxid-classoriginir_parser_1aad295d5d0b31a912538245d07b2aec84>`();
		:ref:`Qinit_declarationContext<doxid-classoriginir_parser_1_1_qinit__declaration_context>`* :target:`qinit_declaration<doxid-classoriginir_parser_1a7d5d6716b694dabb40db9c1b6187ceff>`();
		:ref:`Cinit_declarationContext<doxid-classoriginir_parser_1_1_cinit__declaration_context>`* :target:`cinit_declaration<doxid-classoriginir_parser_1ab1a6b765b121b87dc51fc88df7aac38f>`();
		:ref:`Quantum_gate_declarationContext<doxid-classoriginir_parser_1_1_quantum__gate__declaration_context>`* :target:`quantum_gate_declaration<doxid-classoriginir_parser_1ae0a91bbd7593a04b8af4dfe8eb6d74a1>`();
		:ref:`IndexContext<doxid-classoriginir_parser_1_1_index_context>`* :target:`index<doxid-classoriginir_parser_1a0880bf7b9f42755c6c351606c0a6c183>`();
		:ref:`C_KEY_declarationContext<doxid-classoriginir_parser_1_1_c___k_e_y__declaration_context>`* :target:`c_KEY_declaration<doxid-classoriginir_parser_1aad89877ff2b81481f17b482c99fc547d>`();
		:ref:`Q_KEY_declarationContext<doxid-classoriginir_parser_1_1_q___k_e_y__declaration_context>`* :target:`q_KEY_declaration<doxid-classoriginir_parser_1a9206d511414710cce87605115da1528c>`();
		:ref:`Single_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__declaration_context>`* :target:`single_gate_without_parameter_declaration<doxid-classoriginir_parser_1acd6d5991ed51f07b07c790912d0c54ac>`();
		:ref:`Single_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__declaration_context>`* :target:`single_gate_with_one_parameter_declaration<doxid-classoriginir_parser_1a8d273347a8fefc1c13d13fbb5ac523b9>`();
		:ref:`Single_gate_with_two_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__declaration_context>`* :target:`single_gate_with_two_parameter_declaration<doxid-classoriginir_parser_1a0b7376736ddd832ad5dcece695182a0b>`();
		:ref:`Single_gate_with_three_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__declaration_context>`* :target:`single_gate_with_three_parameter_declaration<doxid-classoriginir_parser_1af112b4d3b4372e33b198467eb907d5a1>`();
		:ref:`Single_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__declaration_context>`* :target:`single_gate_with_four_parameter_declaration<doxid-classoriginir_parser_1aa8153db84a38ccf56418faa861d48e2a>`();
		:ref:`Double_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__declaration_context>`* :target:`double_gate_without_parameter_declaration<doxid-classoriginir_parser_1a39121cea1176f97590dff7e240ea23dc>`();
		:ref:`Double_gate_with_one_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__declaration_context>`* :target:`double_gate_with_one_parameter_declaration<doxid-classoriginir_parser_1a0cb620af428f88f3906351f1cf9d0ed2>`();
		:ref:`Double_gate_with_four_parameter_declarationContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__declaration_context>`* :target:`double_gate_with_four_parameter_declaration<doxid-classoriginir_parser_1acdf955a2d1c259302041f6ff947e23a3>`();
		:ref:`Triple_gate_without_parameter_declarationContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__declaration_context>`* :target:`triple_gate_without_parameter_declaration<doxid-classoriginir_parser_1a02e12fb71ccaa9456b13508d8afd2bb5>`();
		:ref:`Define_gate_declarationContext<doxid-classoriginir_parser_1_1_define__gate__declaration_context>`* :target:`define_gate_declaration<doxid-classoriginir_parser_1ae054a6610e6f55e9783a76a130f6029e>`();
		:ref:`Single_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__without__parameter__type_context>`* :target:`single_gate_without_parameter_type<doxid-classoriginir_parser_1ae71622361ab4b3923a971089df47ea73>`();
		:ref:`Single_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__one__parameter__type_context>`* :target:`single_gate_with_one_parameter_type<doxid-classoriginir_parser_1a1780d077e99e9974aa2a9d148fd91ff6>`();
		:ref:`Single_gate_with_two_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__two__parameter__type_context>`* :target:`single_gate_with_two_parameter_type<doxid-classoriginir_parser_1a192559b029553d0630dcd28692e6b43a>`();
		:ref:`Single_gate_with_three_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__three__parameter__type_context>`* :target:`single_gate_with_three_parameter_type<doxid-classoriginir_parser_1a02825cb18ea4425d1ac69e7738f9c638>`();
		:ref:`Single_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_single__gate__with__four__parameter__type_context>`* :target:`single_gate_with_four_parameter_type<doxid-classoriginir_parser_1a67dbe2921992ae65245057186bde5445>`();
		:ref:`Double_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__without__parameter__type_context>`* :target:`double_gate_without_parameter_type<doxid-classoriginir_parser_1af2254fb53bfca16ff2515683918cbe3e>`();
		:ref:`Double_gate_with_one_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__one__parameter__type_context>`* :target:`double_gate_with_one_parameter_type<doxid-classoriginir_parser_1a2a1ca22ccfa3f98f10526b27aa2b5abc>`();
		:ref:`Double_gate_with_four_parameter_typeContext<doxid-classoriginir_parser_1_1_double__gate__with__four__parameter__type_context>`* :target:`double_gate_with_four_parameter_type<doxid-classoriginir_parser_1a0d729fe41a2f5fbb4f97fc9d7c4ecb91>`();
		:ref:`Triple_gate_without_parameter_typeContext<doxid-classoriginir_parser_1_1_triple__gate__without__parameter__type_context>`* :target:`triple_gate_without_parameter_type<doxid-classoriginir_parser_1a0fd351818ca5b7a3d6fb10249279fc6e>`();
		:ref:`Primary_expressionContext<doxid-classoriginir_parser_1_1_primary__expression_context>`* :target:`primary_expression<doxid-classoriginir_parser_1ac66b9c0b3f421f280d22b0b2dc57ee3e>`();
		:ref:`Unary_expressionContext<doxid-classoriginir_parser_1_1_unary__expression_context>`* :target:`unary_expression<doxid-classoriginir_parser_1ad6c02f202e3f94cbd1a031936c9eee35>`();
		:ref:`Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`* :target:`multiplicative_expression<doxid-classoriginir_parser_1a4c071c2c7304e6bd63c42ec75ab7038c>`();
		:ref:`Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`* :target:`multiplicative_expression<doxid-classoriginir_parser_1ac476c86cf337a0473c5ea02f1ffd7b59>`(int precedence);
		:ref:`Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`* :target:`addtive_expression<doxid-classoriginir_parser_1aff6a36962bef69606e495e43fed53a07>`();
		:ref:`Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`* :target:`addtive_expression<doxid-classoriginir_parser_1ae83b267c635928f64cbe1772ec29b390>`(int precedence);
		:ref:`Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`* :target:`relational_expression<doxid-classoriginir_parser_1a1aa9d4f058002e213f7ebab823484c7a>`();
		:ref:`Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`* :target:`relational_expression<doxid-classoriginir_parser_1a5a2df29265dc56de34d11b3b3315c4c6>`(int precedence);
		:ref:`Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`* :target:`equality_expression<doxid-classoriginir_parser_1a3c7d196fa2e1ec66fb1e85a6a37151fd>`();
		:ref:`Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`* :target:`equality_expression<doxid-classoriginir_parser_1a9c475594440e9db6eb5ae1a88bcd139f>`(int precedence);
		:ref:`Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`* :target:`logical_and_expression<doxid-classoriginir_parser_1aa614f1c0839641ffcc7ed586d4aa4da2>`();
		:ref:`Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`* :target:`logical_and_expression<doxid-classoriginir_parser_1a4faf3b6a6941878fa355b1fd125d50d2>`(int precedence);
		:ref:`Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`* :target:`logical_or_expression<doxid-classoriginir_parser_1a3f2a560498f038bc2b7b12919986dde2>`();
		:ref:`Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`* :target:`logical_or_expression<doxid-classoriginir_parser_1a45e8d98b6162e72f269a9ec0bbeb4125>`(int precedence);
		:ref:`Assignment_expressionContext<doxid-classoriginir_parser_1_1_assignment__expression_context>`* :target:`assignment_expression<doxid-classoriginir_parser_1a04ba568b25dccb0904e7f15877a1549c>`();
		:ref:`ExpressionContext<doxid-classoriginir_parser_1_1_expression_context>`* :target:`expression<doxid-classoriginir_parser_1a0f7832c7e7c7281faca2ba5aedf11b2d>`();
		:ref:`Controlbit_listContext<doxid-classoriginir_parser_1_1_controlbit__list_context>`* :target:`controlbit_list<doxid-classoriginir_parser_1a1561fc59efd1e9571fb82650f92a3a66>`();
		:ref:`StatementContext<doxid-classoriginir_parser_1_1_statement_context>`* :target:`statement<doxid-classoriginir_parser_1a326c9fbd3cd9658ee7ac781e1cc1e3d2>`();
		:ref:`Dagger_statementContext<doxid-classoriginir_parser_1_1_dagger__statement_context>`* :target:`dagger_statement<doxid-classoriginir_parser_1a1bf15a3e6cb724f5c05f290899389b2c>`();
		:ref:`Control_statementContext<doxid-classoriginir_parser_1_1_control__statement_context>`* :target:`control_statement<doxid-classoriginir_parser_1a597d874d1749db88b9778227d59fe0da>`();
		:ref:`Qelse_statement_fragmentContext<doxid-classoriginir_parser_1_1_qelse__statement__fragment_context>`* :target:`qelse_statement_fragment<doxid-classoriginir_parser_1abec919dfee9fc255ae4e634ed2fd8f02>`();
		:ref:`Qif_statementContext<doxid-classoriginir_parser_1_1_qif__statement_context>`* :target:`qif_statement<doxid-classoriginir_parser_1aaba5d3ff0794bd18489a9a886ed3298e>`();
		:ref:`Qwhile_statementContext<doxid-classoriginir_parser_1_1_qwhile__statement_context>`* :target:`qwhile_statement<doxid-classoriginir_parser_1afe7ec99d711afaade806a76871eed418>`();
		:ref:`Measure_statementContext<doxid-classoriginir_parser_1_1_measure__statement_context>`* :target:`measure_statement<doxid-classoriginir_parser_1ad6024207cc63cff0dcd683ad5f2901c8>`();
		:ref:`Reset_statementContext<doxid-classoriginir_parser_1_1_reset__statement_context>`* :target:`reset_statement<doxid-classoriginir_parser_1ad82a9b00d5681e89f5b0d354ebafb530>`();
		:ref:`Barrier_statementContext<doxid-classoriginir_parser_1_1_barrier__statement_context>`* :target:`barrier_statement<doxid-classoriginir_parser_1aafd0b198fef84562af2e206a360f8b52>`();
		:ref:`Expression_statementContext<doxid-classoriginir_parser_1_1_expression__statement_context>`* :target:`expression_statement<doxid-classoriginir_parser_1ae71a2a813a064a8d445fa6c3bffd69e4>`();
		:ref:`Define_gate_statementContext<doxid-classoriginir_parser_1_1_define__gate__statement_context>`* :target:`define_gate_statement<doxid-classoriginir_parser_1aa5c8d7570252fb98cdb56ea736441a6a>`();
		:ref:`ExplistContext<doxid-classoriginir_parser_1_1_explist_context>`* :target:`explist<doxid-classoriginir_parser_1a303e5320fedad9abcf3cc1d4348e17ee>`();
		:ref:`ExpContext<doxid-classoriginir_parser_1_1_exp_context>`* :target:`exp<doxid-classoriginir_parser_1a7613e306b95ecc25aaf352b74668aee2>`();
		:ref:`ExpContext<doxid-classoriginir_parser_1_1_exp_context>`* :target:`exp<doxid-classoriginir_parser_1a5d7a3784778bac4f86755cfdaf8ad0dd>`(int precedence);
		:ref:`Gate_func_statementContext<doxid-classoriginir_parser_1_1_gate__func__statement_context>`* :target:`gate_func_statement<doxid-classoriginir_parser_1ada8d9b16c674317c868b25cf2d0faf8b>`();
		:ref:`IdContext<doxid-classoriginir_parser_1_1_id_context>`* :target:`id<doxid-classoriginir_parser_1a30c76076924ecc9a3271627cba9596e7>`();
		:ref:`Id_listContext<doxid-classoriginir_parser_1_1_id__list_context>`* :target:`id_list<doxid-classoriginir_parser_1a600a6ff00474f6e4fe42e0a41679b03e>`();
		:ref:`Gate_nameContext<doxid-classoriginir_parser_1_1_gate__name_context>`* :target:`gate_name<doxid-classoriginir_parser_1a06680dd1dff7f924dda93e9cab2dcbad>`();
		:ref:`ConstantContext<doxid-classoriginir_parser_1_1_constant_context>`* :target:`constant<doxid-classoriginir_parser_1a5eb4ad9974bd8c6ad66a28205ad3e105>`();
	
		virtual bool :target:`sempred<doxid-classoriginir_parser_1a1a16ec58036b4dc2572b71ab69c19572>`(
			antlr4::RuleContext* _localctx,
			size_t ruleIndex,
			size_t predicateIndex
			);
	
		bool :target:`multiplicative_expressionSempred<doxid-classoriginir_parser_1a4dff639aa9bf609d5507595a1c6da803>`(
			:ref:`Multiplicative_expressionContext<doxid-classoriginir_parser_1_1_multiplicative__expression_context>`* _localctx,
			size_t predicateIndex
			);
	
		bool :target:`addtive_expressionSempred<doxid-classoriginir_parser_1ac0d52bb8e5c9ad40c5cf5a99e07a6d31>`(
			:ref:`Addtive_expressionContext<doxid-classoriginir_parser_1_1_addtive__expression_context>`* _localctx,
			size_t predicateIndex
			);
	
		bool :target:`relational_expressionSempred<doxid-classoriginir_parser_1a9d3a5ff75680c5985619033622533c6b>`(
			:ref:`Relational_expressionContext<doxid-classoriginir_parser_1_1_relational__expression_context>`* _localctx,
			size_t predicateIndex
			);
	
		bool :target:`equality_expressionSempred<doxid-classoriginir_parser_1a8434d009eefde9d438e41cc9d625151d>`(
			:ref:`Equality_expressionContext<doxid-classoriginir_parser_1_1_equality__expression_context>`* _localctx,
			size_t predicateIndex
			);
	
		bool :target:`logical_and_expressionSempred<doxid-classoriginir_parser_1a7e449660f6a3b0217be28ee11a33cdfe>`(
			:ref:`Logical_and_expressionContext<doxid-classoriginir_parser_1_1_logical__and__expression_context>`* _localctx,
			size_t predicateIndex
			);
	
		bool :target:`logical_or_expressionSempred<doxid-classoriginir_parser_1a6a10717a75b5099ea8124bdeb94ddeb2>`(
			:ref:`Logical_or_expressionContext<doxid-classoriginir_parser_1_1_logical__or__expression_context>`* _localctx,
			size_t predicateIndex
			);
	
		bool :target:`expSempred<doxid-classoriginir_parser_1a14545b8bc7a2fef460936de254a318ba>`(
			:ref:`ExpContext<doxid-classoriginir_parser_1_1_exp_context>`* _localctx,
			size_t predicateIndex
			);
	};
