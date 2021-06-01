.. index:: pair: class; QPanda::ApproxTSFinder
.. _doxid-class_q_panda_1_1_approx_t_s_finder:

class QPanda::ApproxTSFinder
============================

.. toctree::
	:hidden:

4-Approximative polynomial algorithm. Miltzow et al. DOI: 10.4230/LIPIcs.ESA.2016.66


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TokenSwapFinder.h>
	
	class ApproxTSFinder: public :ref:`QPanda::TokenSwapFinder<doxid-class_q_panda_1_1_token_swap_finder>`
	{
	public:
		// typedefs
	
		typedef ApproxTSFinder* :target:`Ref<doxid-class_q_panda_1_1_approx_t_s_finder_1a228b710e53dbc6682efe7bb2fc758e5a>`;
		typedef std::unique_ptr<ApproxTSFinder> :target:`uRef<doxid-class_q_panda_1_1_approx_t_s_finder_1a2a8f6fde72eecdd6493eb8821557d9c7>`;

		// methods
	
		static :ref:`uRef<doxid-class_q_panda_1_1_token_swap_finder_1af779e294c4fc3c393a17c2288e86c0d5>` :target:`Create<doxid-class_q_panda_1_1_approx_t_s_finder_1a64d78d7784a499ea155f66f0bf4954ef>`();
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

