.. index:: pair: enum; QProgStoredNodeType
.. _doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8a:

enum QPanda::QProgStoredNodeType
================================

Quantum Program Stored Node Type.

.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QProgStored.h>

	enum QProgStoredNodeType
	{
	    :target:`QPROG_PAULI_X_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaefbf2bd930b8ee7c21a1f9852fec2786>`     = 1u,
	    :target:`QPROG_PAULI_Y_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aab75dcfb20f9b1cbe58eb5cb59298f7e2>`,
	    :target:`QPROG_PAULI_Z_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa031cbc0deb79befb6a40807bf88864e6>`,
	    :target:`QPROG_X_HALF_PI<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa32672baa137f64057855cc89379d7752>`,
	    :target:`QPROG_Y_HALF_PI<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa4a05c2675e40b1c148faea2275b5a548>`,
	    :target:`QPROG_Z_HALF_PI<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa952ba5edb674bbe71234e4daec060dde>`,
	    :target:`QPROG_HADAMARD_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa9e8c6023837c7e7b43bf6fdddc68c5b4>`,
	    :target:`QPROG_T_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaa2ff366f5947d4ed1a0153a3dd5d02de>`,
	    :target:`QPROG_S_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aae08eaf0989e81fa7edb09e1f87c9e88d>`,
	    :target:`QPROG_RX_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa4aa04075c18d25d3ce1975efcc2a7259>`,
	    :target:`QPROG_RY_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaf6494779f421528e145558640c59ed99>`,
	    :target:`QPROG_RZ_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa7e0eee2d7d41c86b3756724f4667385e>`,
	    :target:`QPROG_U1_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa72121bb71d113706f51c547bcb6a5fe6>`,
	    :target:`QPROG_U2_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aad79dc68be2378eb96635becc60840e17>`,
	    :target:`QPROG_U3_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa03f043d72c2f4cdc8a64082e2ba9fbf6>`,
	    :target:`QPROG_U4_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa1b202e2fd11dcbd25104ef0789bb4fb7>`,
	    :target:`QPROG_CU_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa01b6a78523872c1940c243db9a2a6bd6>`,
	    :target:`QPROG_CNOT_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa8b8fc3dc61bb80bd3ad5542e3cf2ff63>`,
	    :target:`QPROG_CZ_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aadcf9c4704748c1830ea82f64a11c7dcb>`,
	    :target:`QPROG_CPHASE_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aac868fc988fed03b7420f4979000ba3b2>`,
	    :target:`QPROG_ISWAP_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa16fce75425e427b2c267d8eb2023f830>`,
	    :target:`QPROG_ISWAP_THETA_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aacd913dd7c4cc327dff106892c484c90c>`,
	    :target:`QPROG_SQISWAP_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aae79f50c70cfd30a5c3be9b04a3d40ea7>`,
	    :target:`QPROG_SWAP_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa0e6fdd0bbce992689b9befc62b04553e>`,
	    :target:`QPROG_GATE_ANGLE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa98b9589c6c56970707094fa640df1c40>`,
	    :target:`QPROG_MEASURE_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa1abc387886ce70d840d408c1604b34cd>`,
	    :target:`QPROG_QIF_NODE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aae384ca3d47507fd75207ba7a570b919c>`,
	    :target:`QPROG_QWHILE_NODE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa4fa62e42b4c276dada7168521553020a>`,
	    :target:`QPROG_CEXPR_CBIT<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaed8579ac97312a08d6220886618123f9>`,
	    :target:`QPROG_CEXPR_OPERATOR<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaa619c165041f1c5c8a1921c55fa0075d>`,
	    :target:`QPROG_CEXPR_CONSTVALUE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaa10d342bdc727e5a16146456cc7cf1d3>`,
	    :target:`QPROG_CEXPR_EVAL<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa05808ca5e7b061ea0dd7c9ab69125122>`,
	    :target:`QPROG_CEXPR_NODE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaa86c65afc8f091192fd7c99a943ecae1>`,
	    :target:`QPROG_CONTROL<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aaa5526bdd088ad59268362f74a639e5ab>`,
	    :target:`QPROG_CIRCUIT_NODE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa94757e4eadd6d067697a69a8ec2ef05a>`,
	    :target:`QPROG_RESET_NODE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa736ee0e51568810b4e98457843660802>`,
	    :target:`QPROG_I_GATE<doxid-namespace_q_panda_1a1eacec5d97776cdc8084cbb6131fed8aa106588c10acccd80d13d7e211030b4ba>`,
	};

