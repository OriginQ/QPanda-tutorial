.. index:: pair: struct; QPanda::SU4TopologyMatch::node
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node:

struct QPanda::SU4TopologyMatch::node
=====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

define struct for nodes in the A\* search; :ref:`More...<details-struct_q_panda_1_1_s_u4_topology_match_1_1node>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	struct node
	{
		// fields
	
		int :ref:`cost_fixed<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1af9a9f5065664e0e3ec3d300234741bf5>`;
		int :target:`cost_heur<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1a877a66f4d3c0a44350d45270c70cad41>`;
		std::vector<int> :ref:`locations<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1aec4b004f675a6235bbcdd341c4bc6bc4>`;
		std::vector<int> :ref:`qubits<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1a482dc3d7a92898076b7f41e83b122014>`;
		bool :ref:`is_goal<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1ac4bea8e1b01cd9222c7d401609e700c7>`;
		std::vector<std::pair<int, int>> :ref:`swaps<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1a335607e1fb7e6d29bf38d0ba2e74c2ec>`;
		std::vector<std::pair<int, int>> :ref:`remaining_gates<doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1a6e21f86b8d816c360366ad6fdc61bb8f>`;
	};
.. _details-struct_q_panda_1_1_s_u4_topology_match_1_1node:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

define struct for nodes in the A\* search;

Fields
------

.. index:: pair: variable; cost_fixed
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1af9a9f5065664e0e3ec3d300234741bf5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int cost_fixed

fixed cost of the current permutation

.. index:: pair: variable; locations
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1aec4b004f675a6235bbcdd341c4bc6bc4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int> locations

heuristic cost of the current permutation

.. index:: pair: variable; qubits
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1a482dc3d7a92898076b7f41e83b122014:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int> qubits

location (i.e. pysical qubit) of a logical qubit

.. index:: pair: variable; is_goal
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1ac4bea8e1b01cd9222c7d401609e700c7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool is_goal

logical qubits that are mapped to the physical ones

.. index:: pair: variable; swaps
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1a335607e1fb7e6d29bf38d0ba2e74c2ec:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::pair<int, int>> swaps

true if the node is a goal node;

.. index:: pair: variable; remaining_gates
.. _doxid-struct_q_panda_1_1_s_u4_topology_match_1_1node_1a6e21f86b8d816c360366ad6fdc61bb8f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::pair<int, int>> remaining_gates

a sequence of swap operations that have been applied

