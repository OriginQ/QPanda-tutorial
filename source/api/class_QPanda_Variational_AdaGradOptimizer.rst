.. index:: pair: class; QPanda::Variational::AdaGradOptimizer
.. _doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer:

class QPanda::Variational::AdaGradOptimizer
===========================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Optimizer.h>
	
	class AdaGradOptimizer: public :ref:`QPanda::Variational::Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`
	{
	public:
		// construction
	
		:target:`AdaGradOptimizer<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer_1a8787f200f71b79d42d81cb8db846ddb4>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lost,
			double learning_rate = 0.01,
			double initial_accumulator_value = 0.0,
			double epsilon = 1e-10
			);

		// methods
	
		virtual std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd> :target:`compute_gradients<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer_1ac442e9a6624501638ff77242f2746c31>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& var_set);
		virtual std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`get_variables<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer_1a3c79e0481e05831bdad3ba627b3a0bc3>`();
		virtual double :target:`get_loss<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer_1a69ed7cc6897cff1f5fc25449b43dca86>`();
	
		virtual bool :target:`run<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer_1a96b1a883e835bb47da379222e5f442b9>`(
			std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves,
			size_t t = 0
			);
	
		static std::shared_ptr<:ref:`Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`> :target:`minimize<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer_1a6ebdf9d2919db29749a4c9d91947e47d>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& lost,
			double learning_rate = 0.01,
			double initial_accumulator_value = 0.0,
			double epsilon = 1e-10
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

