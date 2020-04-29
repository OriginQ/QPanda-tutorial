.. index:: pair: class; qasmParser
.. _doxid-classqasm_parser:

class qasmParser
================

.. toctree::
	:hidden:

	struct_qasmParser_Initializer.rst
	class_qasmParser_AnylistContext.rst
	class_qasmParser_ArgumentContext.rst
	class_qasmParser_Barrier_declContext.rst
	class_qasmParser_BopContext.rst
	class_qasmParser_DecimalContext.rst
	class_qasmParser_ExpContext.rst
	class_qasmParser_ExplistContext.rst
	class_qasmParser_FilenameContext.rst
	class_qasmParser_Gate_declContext.rst
	class_qasmParser_GoplistContext.rst
	class_qasmParser_Head_declContext.rst
	class_qasmParser_IdContext.rst
	class_qasmParser_Id_indexContext.rst
	class_qasmParser_IdlistContext.rst
	class_qasmParser_If_declContext.rst
	class_qasmParser_Include_declContext.rst
	class_qasmParser_IntegerContext.rst
	class_qasmParser_MainprogramContext.rst
	class_qasmParser_Opaque_declContext.rst
	class_qasmParser_QopContext.rst
	class_qasmParser_Reg_declContext.rst
	class_qasmParser_StatementContext.rst
	class_qasmParser_UopContext.rst
	class_qasmParser_Version_declContext.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class qasmParser: public Parser
	{
	public:
		// enums
	
		enum
		{
		    :target:`OPENQASM_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa77534b341663aee0bdd9d24490f86949>` = 1,
		    :target:`INCLUDE_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fabf484d1aab98d5b9cb223af7ef121d67>`  = 2,
		    :target:`OPAQUE_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa5218ce5715d287eefd7ea65fc2ac45db>`   = 3,
		    :target:`QREG_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa181e7ac307926c90b0bcf1b267bc5096>`     = 4,
		    :target:`CREG_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa38d4243eba82ad472565afc249f5006a>`     = 5,
		    :target:`BARRIER_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa1d61a1f23bcd5f54515b22c5306031da>`  = 6,
		    :target:`IF_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa33b88c1c6b9cb0dbac16d7565a179258>`       = 7,
		    :target:`MEASURE_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa871af88dee35582fe4e1161ac61c9410>`  = 8,
		    :target:`RESET_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fac134ba184b15eb28c9934a354db0600c>`    = 9,
		    :target:`GATE_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa4b12cba440cbb8324508b5b22a50d51f>`     = 10,
		    :target:`PI_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa75a33c4a831aa4ed0e634637f172df4c>`       = 11,
		    :target:`U_GATE_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa698861ea850ffc40b4c0cd79f64d1434>`   = 12,
		    :target:`CX_GATE_KEY<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1faad7db155a68d3faff8e1efe665fe26ce>`  = 13,
		    :target:`ARROW<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa5a07fb7d82d58485c995aa9a57171bcf>`        = 14,
		    :target:`EQ<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fac0251d14015f3aeae2ffb21ad8aa4054>`           = 15,
		    :target:`PLUS<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fab14cf4775a180e5928c1ee051ded67c3>`         = 16,
		    :target:`MINUS<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa4a430efddbac4bfebfc5b3162fa8f1d9>`        = 17,
		    :target:`MUL<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa1ede41d6e77a035a8617a7c0ea073a06>`          = 18,
		    :target:`DIV<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa4a2d08f78775a6a70dba9401848d2318>`          = 19,
		    :target:`COMMA<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1facdbd3d6315b8428ca40785fe2a48264b>`        = 20,
		    :target:`SEMI<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa02b53baa56994930360237471b78cc71>`         = 21,
		    :target:`LPAREN<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa779b787f69774561e1f97ff5635a44c5>`       = 22,
		    :target:`RPAREN<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fad35c4137ae528bdcfa101cb14a6485f3>`       = 23,
		    :target:`LBRACKET<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa1692833f371e97511954223ac797a5c8>`     = 24,
		    :target:`RBRACKET<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1faf7717d70ffcb08e0c172291377616b0b>`     = 25,
		    :target:`LBRACE<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fad8e5083b1ba9ade0ac04e7c07140f5a5>`       = 26,
		    :target:`RBRACE<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fab80eb7778ec8dcf4ed02dd7f6b400f13>`       = 27,
		    :target:`DQM<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa477fa1ee731229d0b906a2495e48185f>`          = 28,
		    :target:`IDENTIFIER<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fae5b3d489d87a453be7be7b1482c9854c>`   = 29,
		    :target:`INTEGER<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa21907463a1bd490a2bb4a22b29947330>`      = 30,
		    :target:`DECIMAL<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa71d1323c56852f255d342747151c80bb>`      = 31,
		    :target:`FILENAME<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa448cee3cc687dc8e823c74d87c847858>`     = 32,
		    :target:`NL<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa8c2ddf15815a9817f453eb9c70919307>`           = 33,
		    :target:`WS<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa2265be47858dd34322efa8ed75fb3310>`           = 34,
		    :target:`LC<doxid-classqasm_parser_1a6e021634a0631aad1536425810528b1fa130f2c69d46d44cde26c624922599711>`           = 35,
		};
	
		enum
		{
		    :target:`RuleMainprogram<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea4a4d5ea5a6c17e7b3c2a6eb6e8035981>`  = 0,
		    :target:`RuleHead_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eaa2cdb2aed4b08892ed52434b79bf9e6b>`    = 1,
		    :target:`RuleVersion_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea85f20a117178f049d9042d4c406abb63>` = 2,
		    :target:`RuleInclude_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea44d9063748f8fd46535cb264f2b253d7>` = 3,
		    :target:`RuleStatement<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eabe3495b2f1558aa114c10d36649abd14>`    = 4,
		    :target:`RuleReg_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eaf96344aac1ffb1bd07b21d21df255b3c>`     = 5,
		    :target:`RuleOpaque_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eaffec0b908d7ff846007e9f4d0c4ee6e9>`  = 6,
		    :target:`RuleIf_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea7d92bf51bcf3ad000fb1951c813b7955>`      = 7,
		    :target:`RuleBarrier_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea9dd903523cbd44ce0b752db291c45797>` = 8,
		    :target:`RuleGate_decl<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eafd90475e1ea19e722ae9fb8f009d3120>`    = 9,
		    :target:`RuleGoplist<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea5605a23eb3d34536195768215f363b9e>`      = 10,
		    :target:`RuleBop<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea51deb09ae782d650bb4a57a638af2226>`          = 11,
		    :target:`RuleQop<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea040a1ec20e97bb0707c0f8120d990c84>`          = 12,
		    :target:`RuleUop<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eaac94c82e0868fb077f993ff7d2d9ea60>`          = 13,
		    :target:`RuleAnylist<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eadffdfe51b6bcdb8b48d2cf6926414b3c>`      = 14,
		    :target:`RuleIdlist<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ead6550e16f1c921394098f4b15111bdb4>`       = 15,
		    :target:`RuleId_index<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea6f81adde377cab730de54abfc1ea8b0c>`     = 16,
		    :target:`RuleArgument<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea48a1da364322fff68aa60630e7872b60>`     = 17,
		    :target:`RuleExplist<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eaad794fb8ea33e7ad10ed78067ab5b6f0>`      = 18,
		    :target:`RuleExp<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eadaea9372b69bd1877efd9df3bcfae603>`          = 19,
		    :target:`RuleId<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea5b247d393568987d7d041d1185779f62>`           = 20,
		    :target:`RuleInteger<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852eafe1fbec3c4eb49d3b27f2bcb8215562b>`      = 21,
		    :target:`RuleDecimal<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea61dae5a8045cf1e933c62fdad6190687>`      = 22,
		    :target:`RuleFilename<doxid-classqasm_parser_1affe8f6d0f38cbab8896593a8208d852ea0e795af98f4632367611df9ec783c377>`     = 23,
		};

		// structs
	
		struct :ref:`Initializer<doxid-structqasm_parser_1_1_initializer>`;

		// classes
	
		class :ref:`AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`;
		class :ref:`ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`;
		class :ref:`Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`;
		class :ref:`BopContext<doxid-classqasm_parser_1_1_bop_context>`;
		class :ref:`DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`;
		class :ref:`ExpContext<doxid-classqasm_parser_1_1_exp_context>`;
		class :ref:`ExplistContext<doxid-classqasm_parser_1_1_explist_context>`;
		class :ref:`FilenameContext<doxid-classqasm_parser_1_1_filename_context>`;
		class :ref:`Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`;
		class :ref:`GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`;
		class :ref:`Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`;
		class :ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`;
		class :ref:`Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`;
		class :ref:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`;
		class :ref:`If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`;
		class :ref:`Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`;
		class :ref:`IntegerContext<doxid-classqasm_parser_1_1_integer_context>`;
		class :ref:`MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`;
		class :ref:`Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`;
		class :ref:`QopContext<doxid-classqasm_parser_1_1_qop_context>`;
		class :ref:`Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`;
		class :ref:`StatementContext<doxid-classqasm_parser_1_1_statement_context>`;
		class :ref:`UopContext<doxid-classqasm_parser_1_1_uop_context>`;
		class :ref:`Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`;

		// construction
	
		:target:`qasmParser<doxid-classqasm_parser_1a7e3f192ebb73834a6819e2c8836f6374>`(antlr4::TokenStream* input);

		// methods
	
		virtual std::string :target:`getGrammarFileName<doxid-classqasm_parser_1a8fd47a8ca4d268e8ee549a680cb7de30>`() const;
		virtual const antlr4::atn::ATN& :target:`getATN<doxid-classqasm_parser_1a869871daafbdf9b0d460b47486c704aa>`() const;
		virtual const std::vector<std::string>& :target:`getTokenNames<doxid-classqasm_parser_1a379f027e15f3f15b9c21f7b7d5ea7c71>`() const;
		virtual const std::vector<std::string>& :target:`getRuleNames<doxid-classqasm_parser_1ac633fa1ae3c2f461738f62352a849bc4>`() const;
		virtual antlr4::dfa::Vocabulary& :target:`getVocabulary<doxid-classqasm_parser_1a01794943417523657f07ae1334752b8e>`() const;
		:ref:`MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* :target:`mainprogram<doxid-classqasm_parser_1a202c04b1a88acf94ab12b90da413e9e5>`();
		:ref:`Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* :target:`head_decl<doxid-classqasm_parser_1a3127f4569d93bbe99a1e918d802325b2>`();
		:ref:`Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* :target:`version_decl<doxid-classqasm_parser_1afba865c85400a5dbf68abedfc5a3b0e2>`();
		:ref:`Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* :target:`include_decl<doxid-classqasm_parser_1adde7cdb9cf043ca59c039885844fa2a3>`();
		:ref:`StatementContext<doxid-classqasm_parser_1_1_statement_context>`* :target:`statement<doxid-classqasm_parser_1aedb6726fd3f5971cca8080944639fed1>`();
		:ref:`Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* :target:`reg_decl<doxid-classqasm_parser_1acfa25a366dedd9f5e0edb0911bcd1880>`();
		:ref:`Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* :target:`opaque_decl<doxid-classqasm_parser_1aa6837a6bb657a5b7beb34db36e806087>`();
		:ref:`If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* :target:`if_decl<doxid-classqasm_parser_1aa467866dea830a96413a077c6b5d391d>`();
		:ref:`Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* :target:`barrier_decl<doxid-classqasm_parser_1aa1a8a75fcee56656d992cb5d5a6f1ae0>`();
		:ref:`Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* :target:`gate_decl<doxid-classqasm_parser_1a573c474d20b415bdd74192de197b4eac>`();
		:ref:`GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* :target:`goplist<doxid-classqasm_parser_1a771310b1e7b19e909c26fe8a4cc84dcf>`();
		:ref:`BopContext<doxid-classqasm_parser_1_1_bop_context>`* :target:`bop<doxid-classqasm_parser_1a8783286e528188ca8256dd938b7e22d3>`();
		:ref:`QopContext<doxid-classqasm_parser_1_1_qop_context>`* :target:`qop<doxid-classqasm_parser_1a83680ba1b52238efe88aa0be9849bf2b>`();
		:ref:`UopContext<doxid-classqasm_parser_1_1_uop_context>`* :target:`uop<doxid-classqasm_parser_1a6a736b4a8fc044e666a9e636fbd8731f>`();
		:ref:`AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* :target:`anylist<doxid-classqasm_parser_1a36d34adc0eb73623ca59276923e10e18>`();
		:ref:`IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* :target:`idlist<doxid-classqasm_parser_1acf0c7770d40baa03e401d609399fede0>`();
		:ref:`Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* :target:`id_index<doxid-classqasm_parser_1ae9f527f58857f55af4102e90ff26ea84>`();
		:ref:`ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* :target:`argument<doxid-classqasm_parser_1a5348f99c9c8598898da316c67b286f39>`();
		:ref:`ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* :target:`explist<doxid-classqasm_parser_1aa8e1dfcc15e22f68d35f71b3ab2e0581>`();
		:ref:`ExpContext<doxid-classqasm_parser_1_1_exp_context>`* :target:`exp<doxid-classqasm_parser_1af2f2617c29b040158222beb0217552f8>`();
		:ref:`ExpContext<doxid-classqasm_parser_1_1_exp_context>`* :target:`exp<doxid-classqasm_parser_1a4c8abf922ac2b7fb7600c46e3cb81cf5>`(int precedence);
		:ref:`IdContext<doxid-classqasm_parser_1_1_id_context>`* :target:`id<doxid-classqasm_parser_1aeda5ffb37f7b38673e85c1440ca2b56c>`();
		:ref:`IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* :target:`integer<doxid-classqasm_parser_1acb0e8b17287b23b354512152916e081f>`();
		:ref:`DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* :target:`decimal<doxid-classqasm_parser_1ad2e97e7f634da7da99ec19209a535d7e>`();
		:ref:`FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* :target:`filename<doxid-classqasm_parser_1a954b6e04d08e7156ec155f226f612963>`();
	
		virtual bool :target:`sempred<doxid-classqasm_parser_1ad8ebb9a3235ed5562ead1d8d09642802>`(
			antlr4::RuleContext* _localctx,
			size_t ruleIndex,
			size_t predicateIndex
			);
	
		bool :target:`expSempred<doxid-classqasm_parser_1a0568adb43dc1c1efdc6aecf0f4719631>`(
			:ref:`ExpContext<doxid-classqasm_parser_1_1_exp_context>`* _localctx,
			size_t predicateIndex
			);
	};
