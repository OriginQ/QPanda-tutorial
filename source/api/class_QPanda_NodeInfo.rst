.. index:: pair: class; QPanda::NodeInfo
.. _doxid-class_q_panda_1_1_node_info:

class QPanda::NodeInfo
======================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Detailed information of a :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` node. :ref:`More...<details-class_q_panda_1_1_node_info>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitInfo.h>
	
	class NodeInfo
	{
	public:
		// fields
	
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`m_iter<doxid-class_q_panda_1_1_node_info_1afa444e6c26c1a41b9a28f0facd2ccee5>`;
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`m_node_type<doxid-class_q_panda_1_1_node_info_1ae398dadff0afde22cabdd2ff5b20281f>`;
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :ref:`m_gate_type<doxid-class_q_panda_1_1_node_info_1a2d7e6060b4915dba45f7ce1c02209cb0>`;
		bool :ref:`m_is_dagger<doxid-class_q_panda_1_1_node_info_1a62423e74d282c57cd8ba8a7f7187dc59>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`m_target_qubits<doxid-class_q_panda_1_1_node_info_1ac3ae58a9891b21392e4e9097b4bbdd11>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`m_control_qubits<doxid-class_q_panda_1_1_node_info_1a6ee761642b78a94ed72b87d108ce7292>`;
		std::vector<int> :target:`m_cbits<doxid-class_q_panda_1_1_node_info_1a830136b3fb9af063114aae936a1e8149>`;
		std::vector<double> :target:`m_params<doxid-class_q_panda_1_1_node_info_1a7fdc85d7b53e1973849196a7953dd8ce>`;
		std::string :target:`m_name<doxid-class_q_panda_1_1_node_info_1ae00ef38b4dda111f714fcad4cc48c636>`;

		// construction
	
		:ref:`NodeInfo<doxid-class_q_panda_1_1_node_info_1a3fc75a0b573bf763c62f99961c4e9f9f>`();
	
		:target:`NodeInfo<doxid-class_q_panda_1_1_node_info_1ab74c056e471805a7fb98179554a673c9>`(
			const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` iter,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` target_qubits,
			:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` control_qubits,
			int type,
			const bool dagger
			);

		// methods
	
		virtual void :ref:`reset<doxid-class_q_panda_1_1_node_info_1aaed379503096183ac530a01b41456e4b>`();
	};

	// direct descendants

	struct :ref:`OptimizerNodeInfo<doxid-struct_q_panda_1_1_optimizer_node_info>`;
.. _details-class_q_panda_1_1_node_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Detailed information of a :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` node.

Fields
------

.. index:: pair: variable; m_iter
.. _doxid-class_q_panda_1_1_node_info_1afa444e6c26c1a41b9a28f0facd2ccee5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` m_iter

the :ref:`NodeIter <doxid-class_q_panda_1_1_node_iter>` of the node

.. index:: pair: variable; m_node_type
.. _doxid-class_q_panda_1_1_node_info_1ae398dadff0afde22cabdd2ff5b20281f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` m_node_type

the node type

.. index:: pair: variable; m_gate_type
.. _doxid-class_q_panda_1_1_node_info_1a2d7e6060b4915dba45f7ce1c02209cb0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` m_gate_type

the gate type (if the node type is gate_node)

.. index:: pair: variable; m_is_dagger
.. _doxid-class_q_panda_1_1_node_info_1a62423e74d282c57cd8ba8a7f7187dc59:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool m_is_dagger

dagger information

.. index:: pair: variable; m_target_qubits
.. _doxid-class_q_panda_1_1_node_info_1ac3ae58a9891b21392e4e9097b4bbdd11:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` m_target_qubits

Quantum bits of current node.

.. index:: pair: variable; m_control_qubits
.. _doxid-class_q_panda_1_1_node_info_1a6ee761642b78a94ed72b87d108ce7292:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` m_control_qubits

control Quantum bits.

Construction
------------

.. index:: pair: function; NodeInfo
.. _doxid-class_q_panda_1_1_node_info_1a3fc75a0b573bf763c62f99961c4e9f9f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NodeInfo()

Constructor of :ref:`NodeInfo <doxid-class_q_panda_1_1_node_info>`.

Methods
-------

.. index:: pair: function; reset
.. _doxid-class_q_panda_1_1_node_info_1aaed379503096183ac530a01b41456e4b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual void reset()

reset the node information

