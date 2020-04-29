.. index:: pair: class; QPanda::Variational::MomentumOptimizer
.. _doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer:

class QPanda::Variational::MomentumOptimizer
============================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Optimizer.h>
	
	class MomentumOptimizer: public :ref:`QPanda::Variational::Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`
	{
	public:
		// construction
	
		:target:`MomentumOptimizer<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer_1a849f977ec5854a77d0b52fca090f17da>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lost,
			double learning_rate = 0.01,
			double momentum = 0.9
			);

		// methods
	
		virtual std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd> :target:`compute_gradients<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer_1a20941151f68912eb9b0e06aecbef4004>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& var_set);
		virtual std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`get_variables<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer_1a89461758c0ef2ece29844493847fd169>`();
		virtual double :target:`get_loss<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer_1a5031c191f8b27e0d3c0593349f93b402>`();
	
		virtual bool :target:`run<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer_1a8c6a65ca682c9ccba0823f7406a7dd72>`(
			std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves,
			size_t t = 0
			);
	
		static std::shared_ptr<:ref:`Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`> :target:`minimize<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer_1a1b5cd1a6b429f8d4e2d7f4a396e1c036>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& lost,
			double learning_rate = 0.01,
			double momentum = 0.9
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :ref:`get_variables<doxid-class_q_panda_1_1_variational_1_1_optimizer_1a2a86c7101b183404f8507119954b8142>`() = 0;
		virtual std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd> :ref:`compute_gradients<doxid-class_q_panda_1_1_variational_1_1_optimizer_1a956b08145e8efa6beb20eb6d6c062c07>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& var_set) = 0;
		virtual double :ref:`get_loss<doxid-class_q_panda_1_1_variational_1_1_optimizer_1a6717bbf6bfeda77780e08cd8cfef64a8>`() = 0;
		virtual bool :ref:`run<doxid-class_q_panda_1_1_variational_1_1_optimizer_1aa697607b501c4106c53c3fe9d0a8c3dc>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves, size_t t = 0) = 0;

