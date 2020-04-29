.. index:: pair: class; QPanda::Variational::RMSPropOptimizer
.. _doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer:

class QPanda::Variational::RMSPropOptimizer
===========================================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Optimizer.h>
	
	class RMSPropOptimizer: public :ref:`QPanda::Variational::Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`
	{
	public:
		// construction
	
		:target:`RMSPropOptimizer<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer_1a500582d52289e8b1743acbd3cd1be3eb>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` lost,
			double learning_rate = 0.001,
			double decay = 0.9,
			double epsilon = 1e-10
			);

		// methods
	
		virtual std::unordered_map<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`, MatrixXd> :target:`compute_gradients<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer_1a580132a3b6c6aae115120e09e601122f>`(std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& var_set);
		virtual std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`> :target:`get_variables<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer_1a835f7b17051f6bc25c79dfc4e8074c1c>`();
		virtual double :target:`get_loss<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer_1a13ad0a7cec4bc91f478bb4823bf253eb>`();
	
		virtual bool :target:`run<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer_1a66e7c99dda78075d4faaafd257b88661>`(
			std::unordered_set<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& leaves,
			size_t t = 0
			);
	
		static std::shared_ptr<:ref:`Optimizer<doxid-class_q_panda_1_1_variational_1_1_optimizer>`> :target:`minimize<doxid-class_q_panda_1_1_variational_1_1_r_m_s_prop_optimizer_1af05a742af27fb846b905d3fb88d64ebd>`(
			:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& lost,
			double learning_rate = 0.001,
			double decay = 0.9,
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

