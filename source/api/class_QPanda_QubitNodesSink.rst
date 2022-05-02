.. index:: pair: class; QPanda::QubitNodesSink
.. _doxid-class_q_panda_1_1_qubit_nodes_sink:

class QPanda::QubitNodesSink
============================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ProcessOnTraversing.h>
	
	class QubitNodesSink: public std::map< size_t, std::vector< pOptimizerNodeInfo > >
	{
	public:
		// typedefs
	
		typedef std::map<size_t, std::vector<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>>::iterator :target:`QubitNodesSinkItr<doxid-class_q_panda_1_1_qubit_nodes_sink_1a6d351e83c9e1a8646fb2116e579b42b9>`;
		typedef std::vector<:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>`>::iterator :target:`QubitNodesVecItr<doxid-class_q_panda_1_1_qubit_nodes_sink_1a9aa290d7c056f9c22e0e51077fab011e>`;

		// methods
	
		void :target:`append_data<doxid-class_q_panda_1_1_qubit_nodes_sink_1a5873107d35cfabe2ae5b9383e56b0900>`(
			:ref:`pOptimizerNodeInfo<doxid-namespace_q_panda_1a20ed06f9e8a95ce4bb6321863d9662b3>` p_node,
			const size_t qubit_i
			);
	
		void :target:`insert<doxid-class_q_panda_1_1_qubit_nodes_sink_1aa2f7ce06d79352b0af77c37ac6a48d1a>`(:ref:`GatesBufferType<doxid-namespace_q_panda_1a289faae09fffc3132aac4739008cdbd4>` qubit_nodes);
		const size_t& :target:`get_target_qubit_sink_size<doxid-class_q_panda_1_1_qubit_nodes_sink_1a02a2317e54deb71cdcc3b1ef7cd500b8>`(size_t q) const;
		size_t& :target:`get_target_qubit_sink_size<doxid-class_q_panda_1_1_qubit_nodes_sink_1ae2c442b8a3d16bfb85514dd34cad9964>`(size_t q);
		:ref:`SinkPos<doxid-namespace_q_panda_1abc2b1c5d350f40cf0a262e7bc6de8822>`& :target:`get_sink_pos<doxid-class_q_panda_1_1_qubit_nodes_sink_1ad672473b555c7c4883ece951e36aa3b6>`();
		void :ref:`remove<doxid-class_q_panda_1_1_qubit_nodes_sink_1a5ab46c82dde0a332c39e91f1bd813386>`(size_t qubit, :ref:`QubitNodesVecItr<doxid-class_q_panda_1_1_qubit_nodes_sink_1a9aa290d7c056f9c22e0e51077fab011e>` it_first, :ref:`QubitNodesVecItr<doxid-class_q_panda_1_1_qubit_nodes_sink_1a9aa290d7c056f9c22e0e51077fab011e>` it_end);
	
		void :target:`remove<doxid-class_q_panda_1_1_qubit_nodes_sink_1acff74bdd4bcca6a3b29354eb8aeaff88>`(
			size_t qubit,
			:ref:`QubitNodesVecItr<doxid-class_q_panda_1_1_qubit_nodes_sink_1a9aa290d7c056f9c22e0e51077fab011e>` it_first
			);
	};
.. _details-class_q_panda_1_1_qubit_nodes_sink:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; remove
.. _doxid-class_q_panda_1_1_qubit_nodes_sink_1a5ab46c82dde0a332c39e91f1bd813386:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void remove(size_t qubit, :ref:`QubitNodesVecItr<doxid-class_q_panda_1_1_qubit_nodes_sink_1a9aa290d7c056f9c22e0e51077fab011e>` it_first, :ref:`QubitNodesVecItr<doxid-class_q_panda_1_1_qubit_nodes_sink_1a9aa290d7c056f9c22e0e51077fab011e>` it_end)

note: not include it_end

