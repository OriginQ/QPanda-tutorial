.. index:: pair: class; QPanda::QProgDataParse
.. _doxid-class_q_panda_1_1_q_prog_data_parse:

class QPanda::QProgDataParse
============================

.. toctree::
	:hidden:

	class_QPanda_QProgDataParse_DataNode.rst

Overview
~~~~~~~~

parse binary file to quantum program :ref:`More...<details-class_q_panda_1_1_q_prog_data_parse>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgDataParse.h>
	
	class QProgDataParse
	{
	public:
		// classes
	
		class :ref:`DataNode<doxid-union_q_panda_1_1_q_prog_data_parse_1_1_data_node>`;

		// construction
	
		:target:`QProgDataParse<doxid-class_q_panda_1_1_q_prog_data_parse_1aeb2d97e617d4ce929993b5c211ed86d4>`(:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qm);

		// methods
	
		bool :ref:`load<doxid-class_q_panda_1_1_q_prog_data_parse_1a33974c45d604d915dc8361bdcb000900>`(const std::string& filename);
		bool :ref:`load<doxid-class_q_panda_1_1_q_prog_data_parse_1ab107d071a2ebb923abfc36bdc4b51332>`(const std::vector<uint8_t>& data);
		bool :ref:`parse<doxid-class_q_panda_1_1_q_prog_data_parse_1a5f252ad47a2ab7b52c41685587a63778>`(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog);
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>` :target:`getQubits<doxid-class_q_panda_1_1_q_prog_data_parse_1aab9d3875a9b83e6090918feb8a9a2596>`();
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :target:`getCbits<doxid-class_q_panda_1_1_q_prog_data_parse_1a364f3d634913cc8e58c1abe9c25d80b3>`();
	};
.. _details-class_q_panda_1_1_q_prog_data_parse:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

parse binary file to quantum program

Methods
-------

.. index:: pair: function; load
.. _doxid-class_q_panda_1_1_q_prog_data_parse_1a33974c45d604d915dc8361bdcb000900:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool load(const std::string& filename)

Load qprog data from file.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- filename



.. rubric:: Returns:

bool

.. index:: pair: function; load
.. _doxid-class_q_panda_1_1_q_prog_data_parse_1ab107d071a2ebb923abfc36bdc4b51332:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool load(const std::vector<uint8_t>& data)

Load qprog data from data vector.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<uint8_t>&

		- data



.. rubric:: Returns:

bool

.. index:: pair: function; parse
.. _doxid-class_q_panda_1_1_q_prog_data_parse_1a5f252ad47a2ab7b52c41685587a63778:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool parse(:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`& prog)

Parse binary file to :ref:`QProg <doxid-class_q_panda_1_1_q_prog>`.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QProg&

		- prog



.. rubric:: Returns:

bool

