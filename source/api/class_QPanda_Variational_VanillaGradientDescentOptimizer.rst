.. index:: pair: class; QPanda::Variational::VanillaGradientDescentOptimizer
.. _doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer:

class QPanda::Variational::VanillaGradientDescentOptimizer
==========================================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Optimizer.h>
	
	class VanillaGradientDescentOptimizer: public :ref:`QPanda::Variational::Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`
	{
	public:
		// construction
	
		:target:`VanillaGradientDescentOptimizer<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer_1a6b083b4b2a931c97474dabeddae99fc7>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lost_function,
			double learning_rate = 0.01,
			double stop_condition = 1.e-6,
			:ref:`OptimizerMode<doxid-namespace_q_panda_1_1_variational_1a71962dc3e476a494d016aaee332062c1>` mode = :ref:`OptimizerMode::MINIMIZE<doxid-namespace_q_panda_1_1_variational_1a71962dc3e476a494d016aaee332062c1a704bfa6c1ed5e479c8cfb5bdfc8cccda>`
			);

		// methods
	
		virtual std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`get_variables<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer_1a859b33fc2f5f365af9b319a94c62b96c>`();
		virtual std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd> :target:`compute_gradients<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer_1aaa911a8ca85bcb1d542b6318b23f4b2e>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& var_set);
		virtual double :target:`get_loss<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer_1a549f1c8b87764dba6116c8e1f1c8e5c2>`();
	
		virtual bool :target:`run<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer_1a1c28fa73d912c9726a1e2cd498f0eea3>`(
			std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves,
			size_t t = 0
			);
	
		static std::shared_ptr<:ref:`Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`> :target:`minimize<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer_1abdc800ac748a373608c83e62a39a5588>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`,
			double,
			double
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

