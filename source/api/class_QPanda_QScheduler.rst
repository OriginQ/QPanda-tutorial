.. index:: pair: class; QPanda::QScheduler
.. _doxid-class_q_panda_1_1_q_scheduler:

class QPanda::QScheduler
========================

.. toctree::
	:hidden:

	struct_QPanda_QScheduler_LogicalGate.rst
	struct_QPanda_QScheduler_PhysicsGate.rst

Overview
~~~~~~~~

CODAR algorithm, used for mapping calculations. :ref:`More...<details-class_q_panda_1_1_q_scheduler>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QScheduler.h>
	
	class QScheduler
	{
	public:
		// structs
	
		struct :ref:`LogicalGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate>`;
		struct :ref:`PhysicsGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_physics_gate>`;

		// fields
	
		std::vector<int> :ref:`map_list<doxid-class_q_panda_1_1_q_scheduler_1a8dcaba53a0dbd0b846fda96b38463489>`;
		:ref:`BasicGridDevice<doxid-class_q_panda_1_1_basic_grid_device>`* :ref:`device<doxid-class_q_panda_1_1_q_scheduler_1a1689c7b4d5c7b044b20917e108e08c32>`;
		std::vector<:ref:`GateInfo<doxid-struct_q_panda_1_1_gate_info>`> :ref:`mapped_result_gates<doxid-class_q_panda_1_1_q_scheduler_1a02fd510d48729710ab4f02040c6173dd>`;
		std::list<:ref:`LogicalGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate>`> :ref:`logical_gate_list<doxid-class_q_panda_1_1_q_scheduler_1ad6d185dd094703d55a41bcf9c0d096b9>`;
		std::list<:ref:`LogicalGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate>`> :ref:`candidate_gates<doxid-class_q_panda_1_1_q_scheduler_1a70677ceb94fc36a60e2f52cf2e42da7f>`;
		int :ref:`gate_count<doxid-class_q_panda_1_1_q_scheduler_1ac9b5cc32867719148579263a2fc00923>` = 0;
		int :target:`swap_gate_count<doxid-class_q_panda_1_1_q_scheduler_1a391cbff2044057979a5facd54c62a808>` = 0;
		std::map<std::pair<int, int>, std::pair<int, double>> :ref:`candidate_swaps<doxid-class_q_panda_1_1_q_scheduler_1a9098d7ee39d2d01c105eef1b3a7bf4cb>`;
		std::map<int, int> :target:`logical_qubit_apply_degree<doxid-class_q_panda_1_1_q_scheduler_1a74e1098c707240c9cf9cece732d7ac7b>`;
		std::vector<double> :target:`physics_gate_fidelity<doxid-class_q_panda_1_1_q_scheduler_1ad8f36ebe3a8c7fef79924e63a29f38eb>`;
		std::vector<std::vector<double>> :target:`physics_qubit_error<doxid-class_q_panda_1_1_q_scheduler_1afaa09191868f5cf535b2474acb639b49>`;
		double :target:`double_gate_error_rate<doxid-class_q_panda_1_1_q_scheduler_1a2c4ddde9ac660f58e85b9358406dec01>` = 0;

		// construction
	
		:target:`QScheduler<doxid-class_q_panda_1_1_q_scheduler_1a04b3a140c8413501c6279be86d98614f>`(:ref:`BasicGridDevice<doxid-class_q_panda_1_1_basic_grid_device>`* device);

		// methods
	
		void :target:`loadCommutingTable<doxid-class_q_panda_1_1_q_scheduler_1ad49a259e390c0f19db49053fc767786c>`();
		size_t :ref:`getLogicalQubitCount<doxid-class_q_panda_1_1_q_scheduler_1ae1951391cdb1911727827f61d929319d>`();
		int :ref:`addLogicalQubit<doxid-class_q_panda_1_1_q_scheduler_1a6df8a94718b02a6cf374ec6a6f527ee0>`(int i, int j);
		bool :ref:`addLogicalQubits<doxid-class_q_panda_1_1_q_scheduler_1a543cb1ddfa27bb09648e6f0150ce8df0>`(int count, bool is_order = false);
	
		void :ref:`addSingleQubitGate<doxid-class_q_panda_1_1_q_scheduler_1aa54308e2bd9f628c570da40a08891f42>`(
			std::string gate,
			int gate_type,
			int t,
			std::vector<double> param,
			int barrier_id = -1,
			bool is_dagger = false
			);
	
		void :ref:`addDoubleQubitGate<doxid-class_q_panda_1_1_q_scheduler_1aeee3f16eb766eabd8fdaa17c6a11e988>`(
			std::string gate,
			int gate_type,
			int c,
			int t,
			std::vector<double> param,
			bool is_dagger = false
			);
	
		void :ref:`start<doxid-class_q_panda_1_1_q_scheduler_1a29c034281f4160c109396ed75346c497>`();
	
		void :target:`setQubitFidelity<doxid-class_q_panda_1_1_q_scheduler_1ae03ad4066ada03b57d8025f7bd9a180c>`(
			std::map<int, int> degree,
			std::vector<double> fidelity,
			std::vector<std::vector<double>> error_rate
			);
	};
.. _details-class_q_panda_1_1_q_scheduler:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

CODAR algorithm, used for mapping calculations.

Fields
------

.. index:: pair: variable; map_list
.. _doxid-class_q_panda_1_1_q_scheduler_1a8dcaba53a0dbd0b846fda96b38463489:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<int> map_list

the mapping table from logical qubits to physical qubits, see getMappedPosition

.. index:: pair: variable; device
.. _doxid-class_q_panda_1_1_q_scheduler_1a1689c7b4d5c7b044b20917e108e08c32:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`BasicGridDevice<doxid-class_q_panda_1_1_basic_grid_device>`* device

the device

.. index:: pair: variable; mapped_result_gates
.. _doxid-class_q_panda_1_1_q_scheduler_1a02fd510d48729710ab4f02040c6173dd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<:ref:`GateInfo<doxid-struct_q_panda_1_1_gate_info>`> mapped_result_gates

the output

.. index:: pair: variable; logical_gate_list
.. _doxid-class_q_panda_1_1_q_scheduler_1ad6d185dd094703d55a41bcf9c0d096b9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::list<:ref:`LogicalGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate>`> logical_gate_list

the list of logical gates (the whole circuit)

.. index:: pair: variable; candidate_gates
.. _doxid-class_q_panda_1_1_q_scheduler_1a70677ceb94fc36a60e2f52cf2e42da7f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::list<:ref:`LogicalGate<doxid-struct_q_panda_1_1_q_scheduler_1_1_logical_gate>`> candidate_gates

the set of Commutative Forward gates

.. index:: pair: variable; gate_count
.. _doxid-class_q_panda_1_1_q_scheduler_1ac9b5cc32867719148579263a2fc00923:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int gate_count = 0

count of gates launched

.. index:: pair: variable; candidate_swaps
.. _doxid-class_q_panda_1_1_q_scheduler_1a9098d7ee39d2d01c105eef1b3a7bf4cb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::pair<int, int>, std::pair<int, double>> candidate_swaps

maps from candidate swaps to their heuristic costs

Methods
-------

.. index:: pair: function; getLogicalQubitCount
.. _doxid-class_q_panda_1_1_q_scheduler_1ae1951391cdb1911727827f61d929319d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t getLogicalQubitCount()

get count of logical qubits

.. index:: pair: function; addLogicalQubit
.. _doxid-class_q_panda_1_1_q_scheduler_1a6df8a94718b02a6cf374ec6a6f527ee0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int addLogicalQubit(int i, int j)

add a logical qubit by its position return the index of the logical qubit

.. index:: pair: function; addLogicalQubits
.. _doxid-class_q_panda_1_1_q_scheduler_1a543cb1ddfa27bb09648e6f0150ce8df0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool addLogicalQubits(int count, bool is_order = false)

add several logical qubits and make initial mapping automaticly

MUST ENSURE YOU HAVEN"T MAPPED ANY QUBIT BEFORE CALLING



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- count of qubits



.. rubric:: Returns:

bool true if success

.. index:: pair: function; addSingleQubitGate
.. _doxid-class_q_panda_1_1_q_scheduler_1aa54308e2bd9f628c570da40a08891f42:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void addSingleQubitGate(
		std::string gate,
		int gate_type,
		int t,
		std::vector<double> param,
		int barrier_id = -1,
		bool is_dagger = false
		)

add a (logical) single qubit gate

.. index:: pair: function; addDoubleQubitGate
.. _doxid-class_q_panda_1_1_q_scheduler_1aeee3f16eb766eabd8fdaa17c6a11e988:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void addDoubleQubitGate(
		std::string gate,
		int gate_type,
		int c,
		int t,
		std::vector<double> param,
		bool is_dagger = false
		)

add a logical double qubit gate

.. index:: pair: function; start
.. _doxid-class_q_panda_1_1_q_scheduler_1a29c034281f4160c109396ed75346c497:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void start()

start remapping (call it after intialization) , The main entry of the CODAR remapper

