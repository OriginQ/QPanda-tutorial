.. index:: pair: class; QPanda::Variational::AdamOptimizer
.. _doxid-class_q_panda_1_1_variational_1_1_adam_optimizer:

class QPanda::Variational::AdamOptimizer
========================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Optimizer.h>
	
	class AdamOptimizer: public :ref:`QPanda::Variational::Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`
	{
	public:
		// construction
	
		:target:`AdamOptimizer<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer_1aa21f74697c1f36bc07587559cba36d52>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lost,
			double learning_rate = 0.001,
			double beta1 = 0.9,
			double beta2 = 0.999,
			double epsilon = 1e-8
			);

		// methods
	
		virtual std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd> :target:`compute_gradients<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer_1afd998c590fc4a544d1b918e8327e858e>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& var_set);
		virtual std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`get_variables<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer_1a79131068ca20bc859764960305b6b89e>`();
		virtual double :target:`get_loss<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer_1a08506d09e691a1cac325951696005586>`();
	
		virtual bool :target:`run<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer_1a2adaa5525945887048ef60e752039165>`(
			std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves,
			size_t t = 0
			);
	
		static std::shared_ptr<:ref:`Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`> :target:`minimize<doxid-class_q_panda_1_1_variational_1_1_adam_optimizer_1a9a10ec27b9338eef4069a011bfe3b502>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& lost,
			double learning_rate = 0.001,
			double beta1 = 0.9,
			double beta2 = 0.999,
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

