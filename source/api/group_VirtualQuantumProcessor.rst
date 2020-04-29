.. index:: pair: group; VirtualQuantumProcessor
.. _doxid-group___virtual_quantum_processor:

VirtualQuantumProcessor
=======================

.. toctree::
	:hidden:

	class_AbstractDistributedFullAmplitudeEngine.rst
	class_AbstractQuantumGates.rst
	class_CPUImplQPU.rst
	class_DefaultRandomEngine.rst
	class_DistributedFullAmplitudeEngine.rst
	class_DoubleGateNoiseModeMap.rst
	class_NoisyCPUImplQPU.rst
	class_QPanda_PartialAmplitudeGraph.rst
	class_QPUImpl.rst
	class_RandomEngine.rst
	class_SingleGateNoiseModeMap.rst
	class_XC_RandomEngine16807.rst

Overview
~~~~~~~~

QPanda2 virtual quantum processor. :ref:`More...<details-group___virtual_quantum_processor>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// classes

	class :ref:`AbstractDistributedFullAmplitudeEngine<doxid-class_abstract_distributed_full_amplitude_engine>`;
	class :ref:`AbstractQuantumGates<doxid-class_abstract_quantum_gates>`;
	class :ref:`CPUImplQPU<doxid-class_c_p_u_impl_q_p_u>`;
	class :ref:`DefaultRandomEngine<doxid-class_default_random_engine>`;
	class :ref:`DistributedFullAmplitudeEngine<doxid-class_distributed_full_amplitude_engine>`;
	class :ref:`DoubleGateNoiseModeMap<doxid-class_double_gate_noise_mode_map>`;
	class :ref:`NoisyCPUImplQPU<doxid-class_noisy_c_p_u_impl_q_p_u>`;
	class :ref:`QPanda::PartialAmplitudeGraph<doxid-class_q_panda_1_1_partial_amplitude_graph>`;
	class :ref:`QPUImpl<doxid-class_q_p_u_impl>`;
	class :ref:`RandomEngine<doxid-class_random_engine>`;
	class :ref:`SingleGateNoiseModeMap<doxid-class_single_gate_noise_mode_map>`;
	class :ref:`XC_RandomEngine16807<doxid-class_x_c___random_engine16807>`;

	// global functions

	bool :ref:`bit_phase_flip_operator<doxid-group___virtual_quantum_processor_1ga387b0f99344a6794da969d23de3a96b0>` (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);
	bool :ref:`phase_damping_oprator<doxid-group___virtual_quantum_processor_1gaec6e538178b20f1f902fcdf30ff9062d>`(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);
	bool :ref:`double_bit_phase_flip_operator<doxid-group___virtual_quantum_processor_1gacc4ff7b27f520f6fb21a41c8848cdc0d>` (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);
	bool :ref:`double_phase_damping_oprator<doxid-group___virtual_quantum_processor_1gaef3f3a9f7026dc7a790cb2e58448b5ae>`(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise);

.. _details-group___virtual_quantum_processor:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPanda2 virtual quantum processor.

Global Functions
----------------

.. index:: pair: function; bit_phase_flip_operator
.. _doxid-group___virtual_quantum_processor_1ga387b0f99344a6794da969d23de3a96b0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool bit_phase_flip_operator (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise)

Get Noise model bit-phase flip matrix.

Use this at the :ref:`SingleGateNoiseModeMap <doxid-class_single_gate_noise_mode_map>` constructor



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value

		- Noise model and probability

	*
		- NoiseOp

		- Noise model matrix: E1 = sqrt(1-p){1,0,0,1}, E2 = sqrt(p) {0,-i,i,0}



.. rubric:: Returns:

bool true:get matrix success, false:get matrix failed

.. index:: pair: function; phase_damping_oprator
.. _doxid-group___virtual_quantum_processor_1gaec6e538178b20f1f902fcdf30ff9062d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool phase_damping_oprator(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise)

Get Noise model bit-phase flip matrix.

Use this at the :ref:`SingleGateNoiseModeMap <doxid-class_single_gate_noise_mode_map>` constructor



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value

		- Noise model and probability

	*
		- NoiseOp

		- Noise model matrix: E1 = {1,0,0,sqrt(1-p)} , E2 = {0,0,0,sqrt(p)}



.. rubric:: Returns:

bool true:get matrix success, false:get matrix failed

.. index:: pair: function; double_bit_phase_flip_operator
.. _doxid-group___virtual_quantum_processor_1gacc4ff7b27f520f6fb21a41c8848cdc0d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool double_bit_phase_flip_operator (rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise)

Get Noise model bit-phase flip matrix.

Use this at the :ref:`DoubleGateNoiseModeMap <doxid-class_double_gate_noise_mode_map>` constructor



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value

		- Noise model and probability

	*
		- NoiseOp

		- Noise model matrix: E1 = sqrt(1-p){1,0,0,1}, E2 = sqrt(p) {0,-i,i,0}



.. rubric:: Returns:

bool true:get matrix success, false:get matrix failed

.. index:: pair: function; double_phase_damping_oprator
.. _doxid-group___virtual_quantum_processor_1gaef3f3a9f7026dc7a790cb2e58448b5ae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool double_phase_damping_oprator(rapidjson::Value& value, :ref:`NoiseOp<doxid-_noise_model_8h_1ad01e905fa484518e596588e907885a21>`& noise)

Get Noise model bit-phase flip matrix.

Use this at the :ref:`DoubleGateNoiseModeMap <doxid-class_double_gate_noise_mode_map>` constructor



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value

		- Noise model and probability

	*
		- NoiseOp

		- Noise model matrix: E1 = {1,0,0,sqrt(1-p)}, E2 = {0,0,0,sqrt(p)}



.. rubric:: Returns:

bool true:get matrix success, false:get matrix failed

