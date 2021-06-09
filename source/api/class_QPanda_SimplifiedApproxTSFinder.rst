.. index:: pair: class; QPanda::SimplifiedApproxTSFinder
.. _doxid-class_q_panda_1_1_simplified_approx_t_s_finder:

class QPanda::SimplifiedApproxTSFinder
======================================

.. toctree::
	:hidden:

Simplified 4-Approximative polynomial algorithm. Miltzow et al. DOI: 10.4230/LIPIcs.ESA.2016.66.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TokenSwapFinder.h>
	
	class SimplifiedApproxTSFinder: public :ref:`QPanda::TokenSwapFinder<doxid-class_q_panda_1_1_token_swap_finder>`
	{
	public:
		// typedefs
	
		typedef SimplifiedApproxTSFinder* :target:`Ref<doxid-class_q_panda_1_1_simplified_approx_t_s_finder_1a956fb35a25eeaa7d47a4a2d51d527960>`;
		typedef std::unique_ptr<SimplifiedApproxTSFinder> :target:`uRef<doxid-class_q_panda_1_1_simplified_approx_t_s_finder_1a60d20f615095373ebc67c86fc0f18ed0>`;

		// methods
	
		static :ref:`uRef<doxid-class_q_panda_1_1_token_swap_finder_1af779e294c4fc3c393a17c2288e86c0d5>` :target:`Create<doxid-class_q_panda_1_1_simplified_approx_t_s_finder_1abaa25df7b3a167dbac0da35f883fc7e6>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// typedefs
	
		typedef :ref:`TokenSwapFinder<doxid-class_q_panda_1_1_token_swap_finder>`* :ref:`Ref<doxid-class_q_panda_1_1_token_swap_finder_1a47a575ff2d770bea5bc6fdeeae50c67f>`;
		typedef std::unique_ptr<:ref:`TokenSwapFinder<doxid-class_q_panda_1_1_token_swap_finder>`> :ref:`uRef<doxid-class_q_panda_1_1_token_swap_finder_1af779e294c4fc3c393a17c2288e86c0d5>`;

		// methods
	
		void :ref:`set_graph<doxid-class_q_panda_1_1_token_swap_finder_1a2f28904c7f71504c7b787372f53d0e1f>`(:ref:`QPanda::Graph::Ref<doxid-class_q_panda_1_1_graph_1ac91477f35144fe2bbf3e5ec898bd96e3>` graph);
		:ref:`SwapSeq<doxid-namespace_q_panda_1a4e66c639211525c3cf74a597216fb6a3>` :ref:`find<doxid-class_q_panda_1_1_token_swap_finder_1a5d1fced8fdc887ecc85945086a27b0cf>`(const :ref:`InverseMap<doxid-namespace_q_panda_1a5b0be2998e856af17dafff4568c52cb0>`& from, const :ref:`InverseMap<doxid-namespace_q_panda_1a5b0be2998e856af17dafff4568c52cb0>`& to);

