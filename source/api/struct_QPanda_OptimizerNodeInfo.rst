.. index:: pair: struct; QPanda::OptimizerNodeInfo
.. _doxid-struct_q_panda_1_1_optimizer_node_info:

struct QPanda::OptimizerNodeInfo
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ProcessOnTraversing.h>
	
	struct OptimizerNodeInfo: public :ref:`QPanda::NodeInfo<doxid-class_q_panda_1_1_node_info>`
	{
		// fields
	
		size_t :target:`m_layer<doxid-struct_q_panda_1_1_optimizer_node_info_1a782f4c20e8cef0b22b5f00a5dfe32678>`;
		int :target:`m_type<doxid-struct_q_panda_1_1_optimizer_node_info_1a65eeb0a6b9596f589a11f206a10b56ac>`;
		std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> :target:`m_parent_node<doxid-struct_q_panda_1_1_optimizer_node_info_1a956b9992f76909dbde38ffa4a0b85fb0>`;
		int :target:`m_sub_graph_index<doxid-struct_q_panda_1_1_optimizer_node_info_1ac96e0ee8477f08596ba337aae831f5c8>`;

		// construction
	
		:target:`OptimizerNodeInfo<doxid-struct_q_panda_1_1_optimizer_node_info_1a64e7c8484c003d42801b7f50f99e29df>`(
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` iter,
			size_t layer,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` target_qubits,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` control_qubits,
			int type,
			std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> parent_node,
			const bool dagger
			);

		// methods
	
		virtual void :ref:`reset<doxid-struct_q_panda_1_1_optimizer_node_info_1ae682ce2cb97a8e6aecf4e8226be03b62>`();
		void :target:`insert_QNode<doxid-struct_q_panda_1_1_optimizer_node_info_1a3de082986e5597c71e961d3cfde14723>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`> node);
		bool :target:`operator ==<doxid-struct_q_panda_1_1_optimizer_node_info_1af0365669fc662903c532b31162fdfd7f>` (const OptimizerNodeInfo& other) const;
		bool :target:`is_empty<doxid-struct_q_panda_1_1_optimizer_node_info_1ab14f4e84ca9c04d3b20ef413b097635c>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// fields
	
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`m_iter<doxid-class_q_panda_1_1_node_info_1afa444e6c26c1a41b9a28f0facd2ccee5>`;
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`m_node_type<doxid-class_q_panda_1_1_node_info_1ae398dadff0afde22cabdd2ff5b20281f>`;
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :ref:`m_gate_type<doxid-class_q_panda_1_1_node_info_1a2d7e6060b4915dba45f7ce1c02209cb0>`;
		bool :ref:`m_is_dagger<doxid-class_q_panda_1_1_node_info_1a62423e74d282c57cd8ba8a7f7187dc59>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`m_target_qubits<doxid-class_q_panda_1_1_node_info_1ac3ae58a9891b21392e4e9097b4bbdd11>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`m_control_qubits<doxid-class_q_panda_1_1_node_info_1a6ee761642b78a94ed72b87d108ce7292>`;
		std::vector<int> :ref:`m_cbits<doxid-class_q_panda_1_1_node_info_1a830136b3fb9af063114aae936a1e8149>`;
		std::vector<double> :ref:`m_params<doxid-class_q_panda_1_1_node_info_1a7fdc85d7b53e1973849196a7953dd8ce>`;
		std::string :ref:`m_name<doxid-class_q_panda_1_1_node_info_1ae00ef38b4dda111f714fcad4cc48c636>`;

		// methods
	
		virtual void :ref:`reset<doxid-class_q_panda_1_1_node_info_1aaed379503096183ac530a01b41456e4b>`();

.. _details-struct_q_panda_1_1_optimizer_node_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; reset
.. _doxid-struct_q_panda_1_1_optimizer_node_info_1ae682ce2cb97a8e6aecf4e8226be03b62:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void reset()

reset the node information

