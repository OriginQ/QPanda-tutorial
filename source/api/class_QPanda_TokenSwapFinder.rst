.. index:: pair: class; QPanda::TokenSwapFinder
.. _doxid-class_q_panda_1_1_token_swap_finder:

class QPanda::TokenSwapFinder
=============================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TokenSwapFinder.h>
	
	class TokenSwapFinder
	{
	public:
		// typedefs
	
		typedef TokenSwapFinder* :target:`Ref<doxid-class_q_panda_1_1_token_swap_finder_1a47a575ff2d770bea5bc6fdeeae50c67f>`;
		typedef std::unique_ptr<TokenSwapFinder> :target:`uRef<doxid-class_q_panda_1_1_token_swap_finder_1af779e294c4fc3c393a17c2288e86c0d5>`;

		// methods
	
		void :target:`set_graph<doxid-class_q_panda_1_1_token_swap_finder_1a2f28904c7f71504c7b787372f53d0e1f>`(:ref:`QPanda::Graph::Ref<doxid-class_q_panda_1_1_graph_1ac91477f35144fe2bbf3e5ec898bd96e3>` graph);
	
		:ref:`SwapSeq<doxid-namespace_q_panda_1a4e66c639211525c3cf74a597216fb6a3>` :target:`find<doxid-class_q_panda_1_1_token_swap_finder_1a5d1fced8fdc887ecc85945086a27b0cf>`(
			const :ref:`InverseMap<doxid-namespace_q_panda_1a5b0be2998e856af17dafff4568c52cb0>`& from,
			const :ref:`InverseMap<doxid-namespace_q_panda_1a5b0be2998e856af17dafff4568c52cb0>`& to
			);
	};

	// direct descendants

	class :ref:`ApproxTSFinder<doxid-class_q_panda_1_1_approx_t_s_finder>`;
	class :ref:`SimplifiedApproxTSFinder<doxid-class_q_panda_1_1_simplified_approx_t_s_finder>`;
