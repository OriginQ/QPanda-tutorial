.. index:: pair: enum; GateType
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c:

enum GateType
=============

Overview
~~~~~~~~



.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QGlobalVariable.h>

	enum GateType
	{
	    :target:`GATE_UNDEFINED<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca8fcafbaea63e2513bbe07c4ae7187241>`   = -1,
	    :ref:`P0_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca9f81b62953eac060d4355ce5dcc1027c>`,
	    :ref:`P1_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caace82a431cdaf85c7b8fc78772fb99c3>`,
	    :ref:`PAULI_X_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789cafb152c41b3549d50cd0571db2cbdc1a7>`,
	    :ref:`PAULI_Y_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca8f1a41f8ccd332993559842d9cdd0dfd>`,
	    :ref:`PAULI_Z_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca379c2274ff2d70570cdb99b8b09d955e>`,
	    :ref:`X_HALF_PI<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca30db3e742234efb579d15ac67572c4f5>`,
	    :ref:`Y_HALF_PI<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caed45a54ede9a1e561395a0adfe6d1385>`,
	    :ref:`Z_HALF_PI<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca56e96f26fcae472fce2068167844ab82>`,
	    :ref:`HADAMARD_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caaa4cba341d1db307df6414296a9970eb>`,
	    :ref:`T_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca614d07d597a8e320cc556bc0e652e4ab>`,
	    :ref:`S_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca06e60f80fa80cce271793d6d31bcc21f>`,
	    :ref:`RX_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca0ef81629f054170a8bb71f850820bc3f>`,
	    :ref:`RY_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca7dc7565fd56d69ad24931133d0374267>`,
	    :ref:`RZ_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca74648a1b57818d818c5f32770dde8fce>`,
	    :ref:`U1_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca2eef4d46e040ca6fa7a3fb68b375eb82>`,
	    :ref:`U2_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca73fe77fd9785befb60327a9fd5907ef1>`,
	    :ref:`U3_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca9d0bb91a1b44dbe212e7c2189218ad0a>`,
	    :ref:`U4_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca95c6d62e5f07d09a5e5d47c2d9851930>`,
	    :ref:`CU_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caeceaf10711a39ab0fa34eb20dfd005a0>`,
	    :ref:`CNOT_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca5491d896f56cb9f3f33c34dc439f02e9>`,
	    :ref:`CZ_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca7d657952ccdb6b66c5496943174949f1>`,
	    :ref:`CPHASE_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca278cc5eefc100feda48966b2ea53e3a4>`,
	    :ref:`ISWAP_THETA_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caa00b90d016f7a9568c638ccc662214bc>`,
	    :ref:`ISWAP_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca2c38454a0c4766da08c24760c9e4e692>`,
	    :ref:`SQISWAP_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caf1cae818e98e937a4a27c4ba7e9f4895>`,
	    :ref:`SWAP_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca3159c1145869a5e685a45a03c8547dce>`,
	    :ref:`TWO_QUBIT_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca195459bd4e46077892f9b3026746f2a9>`,
	    :target:`P00_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789cadc49148f955be978d902c8deeee4a2a3>`,
	    :target:`P11_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca7005ffc9530f1565c7724c994ac955af>`,
	    :target:`TOFFOLI_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca8ce7dee098598ba824f02c191965bfce>`,
	    :target:`ORACLE_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca2160ab94c945c11018504b5c0dc18cfc>`,
	    :target:`I_GATE<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789cac83eb4f6e43d98d3a864a3cbb327ceb0>`,
	};

.. _details-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Enum Values
-----------

.. index:: pair: enumvalue; P0_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca9f81b62953eac060d4355ce5dcc1027c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	P0_GATE

Quantum p0 gate

.. index:: pair: enumvalue; P1_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caace82a431cdaf85c7b8fc78772fb99c3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	P1_GATE

Quantum p1 gate

.. index:: pair: enumvalue; PAULI_X_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789cafb152c41b3549d50cd0571db2cbdc1a7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PAULI_X_GATE

Quantum pauli x gate

.. index:: pair: enumvalue; PAULI_Y_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca8f1a41f8ccd332993559842d9cdd0dfd:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PAULI_Y_GATE

Quantum pauli y gate

.. index:: pair: enumvalue; PAULI_Z_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca379c2274ff2d70570cdb99b8b09d955e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PAULI_Z_GATE

Quantum pauli z gate

.. index:: pair: enumvalue; X_HALF_PI
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca30db3e742234efb579d15ac67572c4f5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	X_HALF_PI

Quantum x half gate

.. index:: pair: enumvalue; Y_HALF_PI
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caed45a54ede9a1e561395a0adfe6d1385:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Y_HALF_PI

Quantum y half gate

.. index:: pair: enumvalue; Z_HALF_PI
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca56e96f26fcae472fce2068167844ab82:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Z_HALF_PI

Quantum z half gate

.. index:: pair: enumvalue; HADAMARD_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caaa4cba341d1db307df6414296a9970eb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	HADAMARD_GATE

Quantum hadamard gate

.. index:: pair: enumvalue; T_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca614d07d597a8e320cc556bc0e652e4ab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	T_GATE

Quantum t gate

.. index:: pair: enumvalue; S_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca06e60f80fa80cce271793d6d31bcc21f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	S_GATE

Quantum s gate

.. index:: pair: enumvalue; RX_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca0ef81629f054170a8bb71f850820bc3f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RX_GATE

Quantum rotation x gate

.. index:: pair: enumvalue; RY_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca7dc7565fd56d69ad24931133d0374267:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RY_GATE

Quantum rotation y gate

.. index:: pair: enumvalue; RZ_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca74648a1b57818d818c5f32770dde8fce:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	RZ_GATE

Quantum rotation z gate

.. index:: pair: enumvalue; U1_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca2eef4d46e040ca6fa7a3fb68b375eb82:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U1_GATE

Quantum u1 gate

.. index:: pair: enumvalue; U2_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca73fe77fd9785befb60327a9fd5907ef1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U2_GATE

Quantum u2 gate

.. index:: pair: enumvalue; U3_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca9d0bb91a1b44dbe212e7c2189218ad0a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U3_GATE

Quantum u3 gate

.. index:: pair: enumvalue; U4_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca95c6d62e5f07d09a5e5d47c2d9851930:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	U4_GATE

Quantum u4 gate

.. index:: pair: enumvalue; CU_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caeceaf10711a39ab0fa34eb20dfd005a0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CU_GATE

Quantum control-u gate

.. index:: pair: enumvalue; CNOT_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca5491d896f56cb9f3f33c34dc439f02e9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CNOT_GATE

Quantum control-not gate

.. index:: pair: enumvalue; CZ_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca7d657952ccdb6b66c5496943174949f1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CZ_GATE

Quantum control-z gate

.. index:: pair: enumvalue; CPHASE_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca278cc5eefc100feda48966b2ea53e3a4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	CPHASE_GATE

Quantum control-rotation gate

.. index:: pair: enumvalue; ISWAP_THETA_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caa00b90d016f7a9568c638ccc662214bc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ISWAP_THETA_GATE

Quantum iswap-theta gate

.. index:: pair: enumvalue; ISWAP_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca2c38454a0c4766da08c24760c9e4e692:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	ISWAP_GATE

Quantum iswap gate

.. index:: pair: enumvalue; SQISWAP_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789caf1cae818e98e937a4a27c4ba7e9f4895:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SQISWAP_GATE

Quantum sqiswap gate

.. index:: pair: enumvalue; SWAP_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca3159c1145869a5e685a45a03c8547dce:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	SWAP_GATE

Quantum swap gate

.. index:: pair: enumvalue; TWO_QUBIT_GATE
.. _doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789ca195459bd4e46077892f9b3026746f2a9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	TWO_QUBIT_GATE

Quantum two-qubit gate

