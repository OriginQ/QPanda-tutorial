.. index:: pair: class; QPUImpl
.. _doxid-class_q_p_u_impl:

class QPUImpl
=============

.. toctree::
	:hidden:

Overview
~~~~~~~~

QPU implementation base class. :ref:`More...<details-class_q_p_u_impl>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPUImpl.h>
	
	class QPUImpl
	{
	public:
		// methods
	
		virtual bool :target:`qubitMeasure<doxid-class_q_p_u_impl_1a8231dac2a0406c20032c871de6f45df3>`(size_t qn) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`pMeasure<doxid-class_q_p_u_impl_1a7b81f6f6dd6e1d3e56b812335cd26e5f>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`initState<doxid-class_q_p_u_impl_1a2fb637028cde700f9b415a9f0770eb02>`(
			size_t head_rank,
			size_t rank_size,
			size_t qubit_num
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_q_p_u_impl_1a5d4651b69e9ddcf7f3180b577a80ea22>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_q_p_u_impl_1ad1d0629c91a42e06e079d6d6c215c0a9>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ad5f00e8ccf36ca66f48f4c63b3650e61>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ac164d4305076d2d34f61997ef63a1f34>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_p_u_impl_1aa4152648b4001296305ee546a1136abc>`() = 0;
		virtual void :target:`set_random_engine<doxid-class_q_p_u_impl_1ae8d102f1acac09f453c26f096d0e62ea>`(:ref:`RandomEngine<doxid-class_random_engine>`* rng);
		virtual double :target:`get_random_double<doxid-class_q_p_u_impl_1a25c1af43b633e913810831a5bfd7c90d>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_q_p_u_impl_1a9087cb5109b90f3215093165b11b4218>`(size_t qn) = 0;
	};

	// direct descendants

	class :ref:`CPUImplQPU<doxid-class_c_p_u_impl_q_p_u>`;
	class :ref:`CPUImplQPUSingleThread<doxid-class_c_p_u_impl_q_p_u_single_thread>`;
	class :ref:`DistributedFullAmplitudeEngine<doxid-class_distributed_full_amplitude_engine>`;
	class :ref:`NoisyCPUImplQPU<doxid-class_noisy_c_p_u_impl_q_p_u>`;
.. _details-class_q_p_u_impl:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

QPU implementation base class.

Methods
-------

.. index:: pair: function; unitarySingleQubitGate
.. _doxid-class_q_p_u_impl_1a5d4651b69e9ddcf7f3180b577a80ea22:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitarySingleQubitGate(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0

unitary single qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

	*
		- QStat&

		- matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; controlunitarySingleQubitGate
.. _doxid-class_q_p_u_impl_1ad1d0629c91a42e06e079d6d6c215c0a9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitarySingleQubitGate(
		size_t qn,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		) = 0

controlunitary single qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

	*
		- Qnum&

		- control qubit addresses

	*
		- QStat

		- & matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; unitaryDoubleQubitGate
.. _doxid-class_q_p_u_impl_1ad5f00e8ccf36ca66f48f4c63b3650e61:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		) = 0

unitary double qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- first qubit address

	*
		- size_t

		- second qubit address

	*
		- QStat&

		- matrix

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; controlunitaryDoubleQubitGate
.. _doxid-class_q_p_u_impl_1ac164d4305076d2d34f61997ef63a1f34:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		) = 0

controlunitary double qubit gate



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- first qubit address

	*
		- size_t

		- second qubit address

	*
		- Qnum&

		- control qubit addresses

	*
		- QStat&

		- quantum states

	*
		- bool

		- state of conjugate

	*
		- GateType

		- gate type



.. rubric:: Returns:

QError

.. index:: pair: function; getQState
.. _doxid-class_q_p_u_impl_1aa4152648b4001296305ee546a1136abc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getQState() = 0

get quantum states

.. index:: pair: function; Reset
.. _doxid-class_q_p_u_impl_1a9087cb5109b90f3215093165b11b4218:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` Reset(size_t qn) = 0

reset qubit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

