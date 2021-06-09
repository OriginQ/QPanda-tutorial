.. index:: pair: class; QPanda::HHLAlg
.. _doxid-class_q_panda_1_1_h_h_l_alg:

class QPanda::HHLAlg
====================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <HHL.h>
	
	class HHLAlg
	{
	public:
		// construction
	
		:target:`HHLAlg<doxid-class_q_panda_1_1_h_h_l_alg_1ae9132544577a0d888dff591017b2ceda>`(
			const :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& A,
			const std::vector<double>& b,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* qvm
			);

		// methods
	
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`get_hhl_circuit<doxid-class_q_panda_1_1_h_h_l_alg_1ab8548e130527112872dd74bb3478b4f6>`(uint32_t precision_cnt = 0);
		std::string :target:`check_QPE_result<doxid-class_q_panda_1_1_h_h_l_alg_1a927c0b7cb3caf40ce0f1a3a81519f0ca>`();
		const double& :target:`get_amplification_factor<doxid-class_q_panda_1_1_h_h_l_alg_1af5d326d2f913d1c0faf3604a3dcd5a40>`() const;
		static void :ref:`expand_linear_equations<doxid-group___q_alg_1ga15071b137401e7721541cff22eddc9c8>`(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& A, std::vector<double>& b);
	};
.. _details-class_q_panda_1_1_h_h_l_alg:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; expand_linear_equations
.. _doxid-group___q_alg_1ga15071b137401e7721541cff22eddc9c8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static void expand_linear_equations(:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& A, std::vector<double>& b)

Extending linear equations to N dimension, N=2^n.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QStat&

		- the source matrix, which will be extend to N\*N, N=2^n

	*
		- std::vector<double>&

		- the source vector b, which will be extend to 2^n



.. rubric:: Returns:

