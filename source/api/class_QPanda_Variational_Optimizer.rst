.. index:: pair: class; QPanda::Variational::Optimizer
.. _doxid-class_q_panda_1_1_variational_1_1_optimizer:

class QPanda::Variational::Optimizer
====================================

.. toctree::
	:hidden:

:ref:`Optimizer <doxid-class_q_panda_1_1_variational_1_1_optimizer>` base class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Optimizer.h>
	
	class Optimizer
	{
	public:
		// construction
	
		:target:`Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer_1addd794b0bb91a5330735dc9e44366f51>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lost_function,
			double learning_rate = 0.01
			);

		// methods
	
		virtual std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`get_variables<doxid-class_q_panda_1_1_variational_1_1_optimizer_1a2a86c7101b183404f8507119954b8142>`() = 0;
		virtual std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd> :target:`compute_gradients<doxid-class_q_panda_1_1_variational_1_1_optimizer_1a956b08145e8efa6beb20eb6d6c062c07>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& var_set) = 0;
		virtual double :target:`get_loss<doxid-class_q_panda_1_1_variational_1_1_optimizer_1a6717bbf6bfeda77780e08cd8cfef64a8>`() = 0;
	
		virtual bool :target:`run<doxid-class_q_panda_1_1_variational_1_1_optimizer_1aa697607b501c4106c53c3fe9d0a8c3dc>`(
			std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves,
			size_t t = 0
			) = 0;
	};

	// direct descendants

	class :ref:`AdaGradOptimizer<doxid-class_q_panda_1_1_variational_1_1_ada_grad_optimizer>`;
	class :ref:`AdamOptimizer<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer>`;
	class :ref:`MomentumOptimizer<doxid-class_q_panda_1_1_variational_1_1_momentum_optimizer>`;
	class :ref:`RMSPropOptimizer<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer>`;
	class :ref:`VanillaGradientDescentOptimizer<doxid-class_q_panda_1_1_variational_1_1_vanilla_gradient_descent_optimizer>`;
