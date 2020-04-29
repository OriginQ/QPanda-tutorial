.. index:: pair: enum; NodeType
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16:

enum NodeType
=============

Overview
~~~~~~~~



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QGlobalVariable.h>

	enum NodeType
	{
	    :ref:`NODE_UNDEFINED<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a05c91dffe75997979a5b78ca6c66ccee>`   = -1,
	    :ref:`GATE_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16af346ed6d3c24d457bd5d91eabffd5ff3>`,
	    :ref:`CIRCUIT_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16aec541c7fdb9cc4b30c34ada82e95a345>`,
	    :ref:`PROG_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a46bdc5568925dfbb4b13d338b15dce53>`,
	    :ref:`MEASURE_GATE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a998408e15cfb551f3deeb010c6ff893b>`,
	    :ref:`WHILE_START_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a9b8b8a37e3f2681482c1db84ebfc5109>`,
	    :ref:`QIF_START_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a6b4d2bdc2081ddacd0820e6a947a9cf4>`,
	    :ref:`CLASS_COND_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16aef40d0ad5bc7b63ca664aed53b21ca31>`,
	    :ref:`QWAIT_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16aa06d7a1c5e05710e133fdcab5d090cb4>`,
	    :ref:`RESET_NODE<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a0e3eb9b858e08167a827730587a1747d>`,
	};

.. _details-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Enum Values
-----------

.. index:: pair: enumvalue; NODE_UNDEFINED
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a05c91dffe75997979a5b78ca6c66ccee:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	NODE_UNDEFINED

Undefined node

.. index:: pair: enumvalue; GATE_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16af346ed6d3c24d457bd5d91eabffd5ff3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	GATE_NODE

Quantum gate node

.. index:: pair: enumvalue; CIRCUIT_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16aec541c7fdb9cc4b30c34ada82e95a345:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CIRCUIT_NODE

Quantum circuit node

.. index:: pair: enumvalue; PROG_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a46bdc5568925dfbb4b13d338b15dce53:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PROG_NODE

Quantum program node

.. index:: pair: enumvalue; MEASURE_GATE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a998408e15cfb551f3deeb010c6ff893b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	MEASURE_GATE

Quantum measure node

.. index:: pair: enumvalue; WHILE_START_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a9b8b8a37e3f2681482c1db84ebfc5109:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	WHILE_START_NODE

Quantum while controlflow start node

.. index:: pair: enumvalue; QIF_START_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a6b4d2bdc2081ddacd0820e6a947a9cf4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QIF_START_NODE

Quantum if controlflow start node

.. index:: pair: enumvalue; CLASS_COND_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16aef40d0ad5bc7b63ca664aed53b21ca31:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CLASS_COND_NODE

Quantum classical condition node

.. index:: pair: enumvalue; QWAIT_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16aa06d7a1c5e05710e133fdcab5d090cb4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	QWAIT_NODE

QWait node

.. index:: pair: enumvalue; RESET_NODE
.. _doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16a0e3eb9b858e08167a827730587a1747d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RESET_NODE

QReset node

