.. index:: pair: class; DistributedFullAmplitudeEngine
.. _doxid-class_distributed_full_amplitude_engine:

class DistributedFullAmplitudeEngine
====================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Distributed full amplitude engine. :ref:`More...<details-class_distributed_full_amplitude_engine>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <AbstractFullAmplitudeEngine.h>
	
	class DistributedFullAmplitudeEngine: public :ref:`QPUImpl<doxid-class_q_p_u_impl>`
	{
	public:
		// methods
	
		virtual bool :target:`qubitMeasure<doxid-class_distributed_full_amplitude_engine_1a97420abd2e1571928183fc1efdc5166d>`(size_t qn);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`pMeasure<doxid-class_distributed_full_amplitude_engine_1a84402ee005a3a45f9cc70526b04c12ac>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`initState<doxid-class_distributed_full_amplitude_engine_1a4db677c07322c89923622921c53ecaf9>`(
			size_t head_rank,
			size_t rank_size,
			size_t qubit_num
			);
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_distributed_full_amplitude_engine_1a6367bec1c13c56aec09ed06db7b39cb2>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_distributed_full_amplitude_engine_1a8d758ea0c376ec57d12e88a66ee71f60>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_distributed_full_amplitude_engine_1a7ac8ba8bfbf9acacb3e9b2d766197781>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_distributed_full_amplitude_engine_1acc8d367903a3a8c1f4d01bb11c2a41cf>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`);
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_distributed_full_amplitude_engine_1af272bb852c94330a581933930215986f>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_distributed_full_amplitude_engine_1a27a91284c53e6bc48edec06756e763e7>`(size_t qn);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual bool :ref:`qubitMeasure<doxid-class_q_p_u_impl_1a8231dac2a0406c20032c871de6f45df3>`(size_t qn) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`pMeasure<doxid-class_q_p_u_impl_1a7b81f6f6dd6e1d3e56b812335cd26e5f>`(:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`initState<doxid-class_q_p_u_impl_1a2fb637028cde700f9b415a9f0770eb02>`(size_t head_rank, size_t rank_size, size_t qubit_num) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitarySingleQubitGate<doxid-class_q_p_u_impl_1a5d4651b69e9ddcf7f3180b577a80ea22>`(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitarySingleQubitGate<doxid-class_q_p_u_impl_1ad1d0629c91a42e06e079d6d6c215c0a9>`(size_t qn, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`unitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ad5f00e8ccf36ca66f48f4c63b3650e61>`(size_t qn_0, size_t qn_1, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`controlunitaryDoubleQubitGate<doxid-class_q_p_u_impl_1ac164d4305076d2d34f61997ef63a1f34>`(size_t qn_0, size_t qn_1, :ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`) = 0;
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :ref:`getQState<doxid-class_q_p_u_impl_1aa4152648b4001296305ee546a1136abc>`() = 0;
		virtual void :ref:`set_random_engine<doxid-class_q_p_u_impl_1ae8d102f1acac09f453c26f096d0e62ea>`(:ref:`RandomEngine<doxid-class_random_engine>`* rng);
		virtual double :ref:`get_random_double<doxid-class_q_p_u_impl_1a25c1af43b633e913810831a5bfd7c90d>`();
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :ref:`Reset<doxid-class_q_p_u_impl_1a9087cb5109b90f3215093165b11b4218>`(size_t qn) = 0;

.. _details-class_distributed_full_amplitude_engine:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Distributed full amplitude engine.

Methods
-------

.. index:: pair: function; unitarySingleQubitGate
.. _doxid-class_distributed_full_amplitude_engine_1a6367bec1c13c56aec09ed06db7b39cb2:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitarySingleQubitGate(size_t qn, :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix, bool isConjugate, :ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`)

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
.. _doxid-class_distributed_full_amplitude_engine_1a8d758ea0c376ec57d12e88a66ee71f60:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitarySingleQubitGate(
		size_t qn,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

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
.. _doxid-class_distributed_full_amplitude_engine_1a7ac8ba8bfbf9acacb3e9b2d766197781:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` unitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

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
.. _doxid-class_distributed_full_amplitude_engine_1acc8d367903a3a8c1f4d01bb11c2a41cf:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` controlunitaryDoubleQubitGate(
		size_t qn_0,
		size_t qn_1,
		:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
		:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
		bool isConjugate,
		:ref:`GateType<doxid-_q_global_variable_8h_1a842ca6790f315b3f79faf3cda6d6789c>`
		)

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
.. _doxid-class_distributed_full_amplitude_engine_1af272bb852c94330a581933930215986f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` getQState()

get quantum states

.. index:: pair: function; Reset
.. _doxid-class_distributed_full_amplitude_engine_1a27a91284c53e6bc48edec06756e763e7:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` Reset(size_t qn)

reset qubit



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qubit address

