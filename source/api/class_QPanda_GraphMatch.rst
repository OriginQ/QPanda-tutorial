.. index:: pair: class; QPanda::GraphMatch
.. _doxid-class_q_panda_1_1_graph_match:

class QPanda::GraphMatch
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Graph Match and Replace. :ref:`More...<details-class_q_panda_1_1_graph_match>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <GraphMatch.h>
	
	class GraphMatch
	{
	public:
		// methods
	
		template <typename _Ty>
		void :ref:`get_topological_sequence<doxid-class_q_panda_1_1_graph_match_1af7a3cdf7ebdf0edde69a871333ba418c>`(_Ty& node, :ref:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`& seq, :ref:`GraphType<doxid-namespace_q_panda_1a57710cc0949cf69a28d46e57bcc29f62>` graph_type = :ref:`MAIN_GRAPH<doxid-namespace_q_panda_1a57710cc0949cf69a28d46e57bcc29f62a2916d362819f49f706f686b93dc466d5>`);
	
		template <typename _Ty1, typename _Ty2>
		void :target:`replace<doxid-class_q_panda_1_1_graph_match_1a6afa332f570010e1d332422b59f59b38>`(
			_Ty1& query_node,
			_Ty2& replace_node,
			:ref:`ResultVector<doxid-namespace_q_panda_1a960ac3f5e928f3a42f4d2f2191320897>`& result,
			:ref:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`& graph_seq,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);
	
		bool :target:`query<doxid-class_q_panda_1_1_graph_match_1ab408eb997229b8ba60467aeb4b3dfb2a>`(
			:ref:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`&,
			:ref:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`&,
			:ref:`ResultVector<doxid-namespace_q_panda_1a960ac3f5e928f3a42f4d2f2191320897>`&
			);
	
		const :ref:`QProgDAG<doxid-class_q_panda_1_1_q_prog_d_a_g>`& :target:`getProgDAG<doxid-class_q_panda_1_1_graph_match_1ac8901a53c03e2d7bfd66d704a60b00e9>`();
	};
.. _details-class_q_panda_1_1_graph_match:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Graph Match and Replace.

Methods
-------

.. index:: pair: function; get_topological_sequence
.. _doxid-class_q_panda_1_1_graph_match_1af7a3cdf7ebdf0edde69a871333ba418c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename _Ty>
	void get_topological_sequence(
		_Ty& node,
		:ref:`TopologicalSequence<doxid-namespace_q_panda_1a20bbc03bbc4a7a217bc6d3b64414d328>`& seq,
		:ref:`GraphType<doxid-namespace_q_panda_1a57710cc0949cf69a28d46e57bcc29f62>` graph_type = :ref:`MAIN_GRAPH<doxid-namespace_q_panda_1a57710cc0949cf69a28d46e57bcc29f62a2916d362819f49f706f686b93dc466d5>`
		)

get topological sequence



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- _Ty

		- & node

	*
		- TopologicalSequence

		- & seq

	*
		- GraphType

		- graph_type



.. rubric:: Returns:

void

