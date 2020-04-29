.. index:: pair: class; qasmParser::QopContext
.. _doxid-classqasm_parser_1_1_qop_context:

class qasmParser::QopContext
============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <qasmParser.h>
	
	class QopContext: public ParserRuleContext
	{
	public:
		// construction
	
		:target:`QopContext<doxid-classqasm_parser_1_1_qop_context_1ad0b8c79aafe8df637405284226c790d9>`(
			antlr4::ParserRuleContext* parent,
			size_t invokingState
			);

		// methods
	
		virtual size_t :target:`getRuleIndex<doxid-classqasm_parser_1_1_qop_context_1a095baa266945bc66e644bb17f01767d3>`() const;
		:ref:`UopContext<doxid-classqasm_parser_1_1_uop_context>`* :target:`uop<doxid-classqasm_parser_1_1_qop_context_1aa989fbb86119d223fa2274e555e11c84>`();
		antlr4::tree::TerminalNode* :target:`MEASURE_KEY<doxid-classqasm_parser_1_1_qop_context_1a4fcee578368e04e228382002c769e7be>`();
		std::vector<:ref:`ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`*> :target:`argument<doxid-classqasm_parser_1_1_qop_context_1a48ea6fd04a8cb71e50af1e6398597988>`();
		:ref:`ArgumentContext<doxid-classqasm_parser_1_1_argument_context>`* :target:`argument<doxid-classqasm_parser_1_1_qop_context_1a6c55764a859f1ac23da5fb5dd8a225ec>`(size_t i);
		antlr4::tree::TerminalNode* :target:`ARROW<doxid-classqasm_parser_1_1_qop_context_1a1e5c06a92c87bc4ddd14ff50b97abdef>`();
		antlr4::tree::TerminalNode* :target:`SEMI<doxid-classqasm_parser_1_1_qop_context_1a1bdd4e2ce890258eab3147beb51f06e6>`();
		antlr4::tree::TerminalNode* :target:`RESET_KEY<doxid-classqasm_parser_1_1_qop_context_1a69eb357966a788b90ca2b4a390096a05>`();
		virtual void :target:`enterRule<doxid-classqasm_parser_1_1_qop_context_1ae7e0d3d5b3c64b211879778bafc301ed>`(antlr4::tree::ParseTreeListener* listener);
		virtual void :target:`exitRule<doxid-classqasm_parser_1_1_qop_context_1ab5b8bcac4ab0c61b2c9fd8f9a8c8c3e5>`(antlr4::tree::ParseTreeListener* listener);
		virtual antlrcpp::Any :target:`accept<doxid-classqasm_parser_1_1_qop_context_1ad4094aac686e858f05baa8f5315c8d03>`(antlr4::tree::ParseTreeVisitor* visitor);
	};
