.. index:: pair: class; qasmListener
.. _doxid-classqasm_listener:

class qasmListener
==================

.. toctree::
	:hidden:

This interface defines an abstract listener for a parse tree produced by :ref:`qasmParser <doxid-classqasm_parser>`.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmListener.h>
	
	class qasmListener: public ParseTreeListener
	{
	public:
		// methods
	
		virtual void :target:`enterMainprogram<doxid-classqasm_listener_1a8a7064ee4a82b487affdfad83ac32742>`(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* ctx) = 0;
		virtual void :target:`exitMainprogram<doxid-classqasm_listener_1a3d5982f3aabf97429e510a7b2514d116>`(:ref:`qasmParser::MainprogramContext<doxid-classqasm_parser_1_1_mainprogram_context>`* ctx) = 0;
		virtual void :target:`enterHead_decl<doxid-classqasm_listener_1a328cc48655805f64939a7107b7760199>`(:ref:`qasmParser::Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* ctx) = 0;
		virtual void :target:`exitHead_decl<doxid-classqasm_listener_1ae5dfec8359dafa36f09f5730c8cdd4d2>`(:ref:`qasmParser::Head_declContext<doxid-classqasm_parser_1_1_head__decl_context>`* ctx) = 0;
		virtual void :target:`enterVersion_decl<doxid-classqasm_listener_1a2740f350b629f51b4bbb77749caf9796>`(:ref:`qasmParser::Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* ctx) = 0;
		virtual void :target:`exitVersion_decl<doxid-classqasm_listener_1a1f60ca878176adab690d7049a7721db8>`(:ref:`qasmParser::Version_declContext<doxid-classqasm_parser_1_1_version__decl_context>`* ctx) = 0;
		virtual void :target:`enterInclude_decl<doxid-classqasm_listener_1aca500fdc33ee50e3e4a5dfae26d14d92>`(:ref:`qasmParser::Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* ctx) = 0;
		virtual void :target:`exitInclude_decl<doxid-classqasm_listener_1a21b944953702652db423a6dd94f4c722>`(:ref:`qasmParser::Include_declContext<doxid-classqasm_parser_1_1_include__decl_context>`* ctx) = 0;
		virtual void :target:`enterStatement<doxid-classqasm_listener_1a47939a96cf0c110dbc244cd1a1482b10>`(:ref:`qasmParser::StatementContext<doxid-classqasm_parser_1_1_statement_context>`* ctx) = 0;
		virtual void :target:`exitStatement<doxid-classqasm_listener_1a6c93fbca068329a5099850396fc731bd>`(:ref:`qasmParser::StatementContext<doxid-classqasm_parser_1_1_statement_context>`* ctx) = 0;
		virtual void :target:`enterReg_decl<doxid-classqasm_listener_1a006f38554994a04fc7ad5bb77ab555ea>`(:ref:`qasmParser::Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* ctx) = 0;
		virtual void :target:`exitReg_decl<doxid-classqasm_listener_1a22f05177004347fefdb3aa1a0a86e1cc>`(:ref:`qasmParser::Reg_declContext<doxid-classqasm_parser_1_1_reg__decl_context>`* ctx) = 0;
		virtual void :target:`enterOpaque_decl<doxid-classqasm_listener_1ae3aa730f6cbdb0edb2264ee56bbb51f4>`(:ref:`qasmParser::Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* ctx) = 0;
		virtual void :target:`exitOpaque_decl<doxid-classqasm_listener_1ab8997900133503da875a0d0be7523df9>`(:ref:`qasmParser::Opaque_declContext<doxid-classqasm_parser_1_1_opaque__decl_context>`* ctx) = 0;
		virtual void :target:`enterIf_decl<doxid-classqasm_listener_1ae09f6d6f65ccfaddc6946ac338c85f91>`(:ref:`qasmParser::If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* ctx) = 0;
		virtual void :target:`exitIf_decl<doxid-classqasm_listener_1a3113a1ab827b3d5a5085424848735cf7>`(:ref:`qasmParser::If_declContext<doxid-classqasm_parser_1_1_if__decl_context>`* ctx) = 0;
		virtual void :target:`enterBarrier_decl<doxid-classqasm_listener_1a94b173d3c449b932c71eeedaaa291161>`(:ref:`qasmParser::Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* ctx) = 0;
		virtual void :target:`exitBarrier_decl<doxid-classqasm_listener_1a2bce72c0baba27432daf12aba2228178>`(:ref:`qasmParser::Barrier_declContext<doxid-classqasm_parser_1_1_barrier__decl_context>`* ctx) = 0;
		virtual void :target:`enterGate_decl<doxid-classqasm_listener_1abf500447ec5833b1ca2eb34fa7494dba>`(:ref:`qasmParser::Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* ctx) = 0;
		virtual void :target:`exitGate_decl<doxid-classqasm_listener_1ad7071773a128c470df7c272bd9eaa3a4>`(:ref:`qasmParser::Gate_declContext<doxid-classqasm_parser_1_1_gate__decl_context>`* ctx) = 0;
		virtual void :target:`enterGoplist<doxid-classqasm_listener_1af167e7e15fc8d90c3e54e789a27bd3bb>`(:ref:`qasmParser::GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* ctx) = 0;
		virtual void :target:`exitGoplist<doxid-classqasm_listener_1af3b395495d114ec7c6be725f607f6e43>`(:ref:`qasmParser::GoplistContext<doxid-classqasm_parser_1_1_goplist_context>`* ctx) = 0;
		virtual void :target:`enterBop<doxid-classqasm_listener_1a0628a95fd001cd9d72bef863d6a462ad>`(:ref:`qasmParser::BopContext<doxid-classqasm_parser_1_1_bop_context>`* ctx) = 0;
		virtual void :target:`exitBop<doxid-classqasm_listener_1aeac63e0a4a1376ba78b7f48c67946889>`(:ref:`qasmParser::BopContext<doxid-classqasm_parser_1_1_bop_context>`* ctx) = 0;
		virtual void :target:`enterQop<doxid-classqasm_listener_1ad227d7128570e99ec3cf22a60d44380e>`(:ref:`qasmParser::QopContext<doxid-classqasm_parser_1_1_qop_context>`* ctx) = 0;
		virtual void :target:`exitQop<doxid-classqasm_listener_1a8d6ea3ab83ce7012571cb318c7b4ebb2>`(:ref:`qasmParser::QopContext<doxid-classqasm_parser_1_1_qop_context>`* ctx) = 0;
		virtual void :target:`enterUop<doxid-classqasm_listener_1abe674c22e94719b80dd7ed9cb557bcc1>`(:ref:`qasmParser::UopContext<doxid-classqasm_parser_1_1_uop_context>`* ctx) = 0;
		virtual void :target:`exitUop<doxid-classqasm_listener_1a1384b5182cf304d96cb39881b3365eb5>`(:ref:`qasmParser::UopContext<doxid-classqasm_parser_1_1_uop_context>`* ctx) = 0;
		virtual void :target:`enterAnylist<doxid-classqasm_listener_1a94f892aacb55e301d85046615dd21d06>`(:ref:`qasmParser::AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* ctx) = 0;
		virtual void :target:`exitAnylist<doxid-classqasm_listener_1a49ecbc92545c2be62079518f04e8aa70>`(:ref:`qasmParser::AnylistContext<doxid-classqasm_parser_1_1_anylist_context>`* ctx) = 0;
		virtual void :target:`enterIdlist<doxid-classqasm_listener_1ac14052e6fa606aac398f3c4947750956>`(:ref:`qasmParser::IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* ctx) = 0;
		virtual void :target:`exitIdlist<doxid-classqasm_listener_1a67f7213c16a4a3a3c2d9ab824103b83e>`(:ref:`qasmParser::IdlistContext<doxid-classqasm_parser_1_1_idlist_context>`* ctx) = 0;
		virtual void :target:`enterId_index<doxid-classqasm_listener_1ac1b9f150360eb8bfb51c5fbc7cb7b018>`(:ref:`qasmParser::Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* ctx) = 0;
		virtual void :target:`exitId_index<doxid-classqasm_listener_1a1cf001e55c80a73f4ae0bc2307979932>`(:ref:`qasmParser::Id_indexContext<doxid-classqasm_parser_1_1_id__index_context>`* ctx) = 0;
		virtual void :target:`enterArgument<doxid-classqasm_listener_1a7af75d03f7c481e8f5d8b600ab64850c>`(:ref:`qasmParser::ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* ctx) = 0;
		virtual void :target:`exitArgument<doxid-classqasm_listener_1af8117cbab0d1629af44a02164a613425>`(:ref:`qasmParser::ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* ctx) = 0;
		virtual void :target:`enterExplist<doxid-classqasm_listener_1af5e4f4ae148a8a053ac0c95ce2bfbc7b>`(:ref:`qasmParser::ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* ctx) = 0;
		virtual void :target:`exitExplist<doxid-classqasm_listener_1aea3830faab24d270bd26b439ff574649>`(:ref:`qasmParser::ExplistContext<doxid-classqasm_parser_1_1_explist_context>`* ctx) = 0;
		virtual void :target:`enterExp<doxid-classqasm_listener_1a66a1e502f8c567712139ac6c93ca2871>`(:ref:`qasmParser::ExpContext<doxid-classqasm_parser_1_1_exp_context>`* ctx) = 0;
		virtual void :target:`exitExp<doxid-classqasm_listener_1a74d2cc777d6a6105b2848a2943536505>`(:ref:`qasmParser::ExpContext<doxid-classqasm_parser_1_1_exp_context>`* ctx) = 0;
		virtual void :target:`enterId<doxid-classqasm_listener_1adb4cab7ce3e9f238dc19c18f5d3b3b26>`(:ref:`qasmParser::IdContext<doxid-classqasm_parser_1_1_id_context>`* ctx) = 0;
		virtual void :target:`exitId<doxid-classqasm_listener_1a310d702cf38ea4433f4ffc8394ebc7b7>`(:ref:`qasmParser::IdContext<doxid-classqasm_parser_1_1_id_context>`* ctx) = 0;
		virtual void :target:`enterInteger<doxid-classqasm_listener_1af0555e4d9a99529fca4c9547e220e01e>`(:ref:`qasmParser::IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* ctx) = 0;
		virtual void :target:`exitInteger<doxid-classqasm_listener_1a9fa33ad127ed54fbaaf0f380d84e1cb9>`(:ref:`qasmParser::IntegerContext<doxid-classqasm_parser_1_1_integer_context>`* ctx) = 0;
		virtual void :target:`enterDecimal<doxid-classqasm_listener_1a50c9f9b3304915f420311835ecc46e4e>`(:ref:`qasmParser::DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* ctx) = 0;
		virtual void :target:`exitDecimal<doxid-classqasm_listener_1a199c6ecf2352b7d55db9cc47eef0dd61>`(:ref:`qasmParser::DecimalContext<doxid-classqasm_parser_1_1_decimal_context>`* ctx) = 0;
		virtual void :target:`enterFilename<doxid-classqasm_listener_1a34445b54a04b31e822434ce260804dd9>`(:ref:`qasmParser::FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* ctx) = 0;
		virtual void :target:`exitFilename<doxid-classqasm_listener_1abca7f7e66ff7a25304474853fe42a23d>`(:ref:`qasmParser::FilenameContext<doxid-classqasm_parser_1_1_filename_context>`* ctx) = 0;
	};
