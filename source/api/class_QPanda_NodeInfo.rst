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
	
		:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`m_itr<doxid-class_q_panda_1_1_node_info_1aa4c6dfe23682f1e20cf1af42661ae67d>`;
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`m_node_type<doxid-class_q_panda_1_1_node_info_1ae398dadff0afde22cabdd2ff5b20281f>`;
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>` :ref:`m_gate_type<doxid-class_q_panda_1_1_node_info_1a2d7e6060b4915dba45f7ce1c02209cb0>`;
		bool :ref:`m_is_dagger<doxid-class_q_panda_1_1_node_info_1a62423e74d282c57cd8ba8a7f7187dc59>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`m_qubits<doxid-class_q_panda_1_1_node_info_1a02849d9a169eae9ad1beed3ccb269993>`;
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :ref:`m_control_qubits<doxid-class_q_panda_1_1_node_info_1a6ee761642b78a94ed72b87d108ce7292>`;

		// methods
	
		void :ref:`clear<doxid-class_q_panda_1_1_node_info_1a2ee2d85738c0328ebc0d0759dee001ef>`();
	};
.. _details-class_q_panda_1_1_node_info:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Detailed information of a :ref:`QProg <doxid-class_q_panda_1_1_q_prog>` node.

Fields
------

.. index:: pair: variable; m_itr
.. _doxid-class_q_panda_1_1_node_info_1aa4c6dfe23682f1e20cf1af42661ae67d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` m_itr

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

.. index:: pair: variable; m_qubits
.. _doxid-class_q_panda_1_1_node_info_1a02849d9a169eae9ad1beed3ccb269993:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` m_qubits

Quantum bits of current node

.. index:: pair: variable; m_control_qubits
.. _doxid-class_q_panda_1_1_node_info_1a6ee761642b78a94ed72b87d108ce7292:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` m_control_qubits

control Quantum bits

Methods
-------

.. index:: pair: function; clear
.. _doxid-class_q_panda_1_1_node_info_1a2ee2d85738c0328ebc0d0759dee001ef:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void clear()

clear the node information

