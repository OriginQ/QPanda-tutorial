.. index:: pair: class; QPanda::PauliOp
.. _doxid-class_q_panda_1_1_pauli_op:

template class QPanda::PauliOp
==============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Pauli operator class. :ref:`More...<details-class_q_panda_1_1_pauli_op>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <PauliOperator.h>
	
	template <class T>
	class PauliOp
	{
	public:
		// typedefs
	
		typedef std::pair<:ref:`QPauliPair<doxid-namespace_q_panda_1a922b9a7c131f853272fc7115017e9bb8>`, :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> :target:`PauliItem<doxid-class_q_panda_1_1_pauli_op_1ace5238ddc3bf98197f24e72be57b1392>`;
		typedef std::vector<:ref:`PauliItem<doxid-class_q_panda_1_1_pauli_op_1ace5238ddc3bf98197f24e72be57b1392>`> :target:`PauliData<doxid-class_q_panda_1_1_pauli_op_1a2d0d61d1c03555513d5a092dfee4eef6>`;
		typedef std::map<std::string, :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> :target:`PauliMap<doxid-class_q_panda_1_1_pauli_op_1af42ad2b2eaf927a6278b97965fdb6d25>`;

		// construction
	
		:ref:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1a9815d5433225e566a21f3d19bcbe5d7c>`();
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1af685370cc1eeb172fe8a38e2bf621dff>`(const :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& value);
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1a671e2aef059d90a4925caae5f86f1733>`(double value);
	
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1aef7cfb20bc68d99a5915ea49160f74ed>`(
			const std::string& key,
			const :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& value
			);
	
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1a9724ff2d8e202dbcaa8dd9ad128d1b29>`(const :ref:`PauliMap<doxid-class_q_panda_1_1_pauli_op_1af42ad2b2eaf927a6278b97965fdb6d25>`& map);
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1aa6747af46f43304ce7ec0abf0e9ace7c>`(PauliOp&& op);
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1a3179589a71ece3091cb0933caee4121a>`(const PauliOp& op);
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1a0bae11c49fe1899c30cbba56c3952efb>`(:ref:`PauliData<doxid-class_q_panda_1_1_pauli_op_1a2d0d61d1c03555513d5a092dfee4eef6>`&& pauli);
		:target:`PauliOp<doxid-class_q_panda_1_1_pauli_op_1afbcc53d456781eab1f3a3aaacc0d32b6>`(const :ref:`PauliData<doxid-class_q_panda_1_1_pauli_op_1a2d0d61d1c03555513d5a092dfee4eef6>`& pauli);

		// methods
	
		PauliOp& :target:`operator =<doxid-class_q_panda_1_1_pauli_op_1adde36b924a6a5f323b2f30cd536dd038>` (const PauliOp& op);
		PauliOp& :target:`operator =<doxid-class_q_panda_1_1_pauli_op_1a3b99b66a06cebf5ee473ff2124fb1c37>` (PauliOp&& op);
		PauliOp :ref:`dagger<doxid-class_q_panda_1_1_pauli_op_1a499271559b14d78c63c4ef48b61c3f5a>`() const;
		PauliOp :ref:`remapQubitIndex<doxid-class_q_panda_1_1_pauli_op_1aca2197981a42eb94ddccf73c0467d5b1>`(std::map<size_t, size_t>& index_map);
		size_t :ref:`getMaxIndex<doxid-class_q_panda_1_1_pauli_op_1af4d431d9eed6f123a32b5203cc063027>`();
		bool :ref:`isEmpty<doxid-class_q_panda_1_1_pauli_op_1a31d6d3bb84aa3debcd85bbef231309fc>`();
		bool :ref:`isAllPauliZorI<doxid-class_q_panda_1_1_pauli_op_1aa0dd2e9cb815ed793c5eabf275b8c76d>`();
		void :ref:`setErrorThreshold<doxid-class_q_panda_1_1_pauli_op_1a8b95cdfc2791383ef37a3971951bfa6c>`(double threshold);
		double :ref:`error_threshold<doxid-class_q_panda_1_1_pauli_op_1a1f089bda4a44272deae129675396210f>`() const;
		std::string :ref:`toString<doxid-class_q_panda_1_1_pauli_op_1aefa7ba3179d1f1e1e228388ae19231f4>`() const;
		:ref:`PauliData<doxid-class_q_panda_1_1_pauli_op_1a2d0d61d1c03555513d5a092dfee4eef6>` :ref:`data<doxid-class_q_panda_1_1_pauli_op_1a409e2a18d8c04189f32d93662d471a83>`() const;
		:ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>` :ref:`toHamiltonian<doxid-class_q_panda_1_1_pauli_op_1af31c31945f396d0d3a55053b6128c63e>`(bool* ok = nullptr);
		PauliOp :ref:`operator +<doxid-class_q_panda_1_1_pauli_op_1aea667fb76deb422536b30a46d699d26a>` (const PauliOp& rhs) const;
		PauliOp :ref:`operator -<doxid-class_q_panda_1_1_pauli_op_1acabf9859cc7ec060674fe8e8ac0dd436>` (const PauliOp& rhs) const;
		PauliOp :ref:`operator *<doxid-class_q_panda_1_1_pauli_op_1afcc8b975f91a92c743a55f46a26a071d>` (const PauliOp& rhs) const;
		PauliOp& :ref:`operator +=<doxid-class_q_panda_1_1_pauli_op_1a27be3f087ea755a6f215362c5da07927>` (const PauliOp& rhs);
		PauliOp& :ref:`operator -=<doxid-class_q_panda_1_1_pauli_op_1ac708f5038b0de144ef7e769ef774dc57>` (const PauliOp& rhs);
		PauliOp& :ref:`operator *=<doxid-class_q_panda_1_1_pauli_op_1a8471110ff429d2a4b1b0f16064facc14>` (const PauliOp& rhs);
	};
.. _details-class_q_panda_1_1_pauli_op:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Pauli operator class.

Construction
------------

.. index:: pair: function; PauliOp
.. _doxid-class_q_panda_1_1_pauli_op_1a9815d5433225e566a21f3d19bcbe5d7c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp()

Constructor of :ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` class.

Methods
-------

.. index:: pair: function; dagger
.. _doxid-class_q_panda_1_1_pauli_op_1a499271559b14d78c63c4ef48b61c3f5a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp dagger() const

get the Transposed conjugate matrix



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return the Transposed conjugate matrix

.. index:: pair: function; remapQubitIndex
.. _doxid-class_q_panda_1_1_pauli_op_1aca2197981a42eb94ddccf73c0467d5b1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp remapQubitIndex(std::map<size_t, size_t>& index_map)

remap qubit index



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::map<size_t

		- 

	*
		- size_t>&

		- qubit index map



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return remapped qubit index map

.. index:: pair: function; getMaxIndex
.. _doxid-class_q_panda_1_1_pauli_op_1af4d431d9eed6f123a32b5203cc063027:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t getMaxIndex()

get the max index



.. rubric:: Returns:

size_t the max index

.. index:: pair: function; isEmpty
.. _doxid-class_q_panda_1_1_pauli_op_1a31d6d3bb84aa3debcd85bbef231309fc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isEmpty()

Judge whether it is empty.



.. rubric:: Returns:

bool if data is empty, return true, or else return false

.. index:: pair: function; isAllPauliZorI
.. _doxid-class_q_panda_1_1_pauli_op_1aa0dd2e9cb815ed793c5eabf275b8c76d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isAllPauliZorI()

Judge whether all of data is "Z".



.. rubric:: Returns:

bool if all data is "Z", return true, or else return false

.. index:: pair: function; setErrorThreshold
.. _doxid-class_q_panda_1_1_pauli_op_1a8b95cdfc2791383ef37a3971951bfa6c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setErrorThreshold(double threshold)

set error threshold



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- threshold val

.. index:: pair: function; error_threshold
.. _doxid-class_q_panda_1_1_pauli_op_1a1f089bda4a44272deae129675396210f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	double error_threshold() const

get error threshold



.. rubric:: Returns:

double return the error threshold val

.. index:: pair: function; toString
.. _doxid-class_q_panda_1_1_pauli_op_1aefa7ba3179d1f1e1e228388ae19231f4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string toString() const

data to string



.. rubric:: Returns:

std::string convert data val to string

.. index:: pair: function; data
.. _doxid-class_q_panda_1_1_pauli_op_1a409e2a18d8c04189f32d93662d471a83:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PauliData<doxid-class_q_panda_1_1_pauli_op_1a2d0d61d1c03555513d5a092dfee4eef6>` data() const

get data



.. rubric:: Returns:

PauliData return Pauli data

.. index:: pair: function; toHamiltonian
.. _doxid-class_q_panda_1_1_pauli_op_1af31c31945f396d0d3a55053b6128c63e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`QHamiltonian<doxid-namespace_q_panda_1ad608a1d24a69c36a298895b44c90a250>` toHamiltonian(bool* ok = nullptr)

convert data to Hamiltonian



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool\*

		- save the convert result, default is nullptr



.. rubric:: Returns:

QHamiltonian the convert result

.. index:: pair: function; operator+
.. _doxid-class_q_panda_1_1_pauli_op_1aea667fb76deb422536b30a46d699d26a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp operator + (const PauliOp& rhs) const

overload +



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return (PauliOp_left + PauliOp_right)

.. index:: pair: function; operator-
.. _doxid-class_q_panda_1_1_pauli_op_1acabf9859cc7ec060674fe8e8ac0dd436:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp operator - (const PauliOp& rhs) const

overload -



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return (PauliOp_left - PauliOp_right)

.. index:: pair: function; operator*
.. _doxid-class_q_panda_1_1_pauli_op_1afcc8b975f91a92c743a55f46a26a071d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp operator * (const PauliOp& rhs) const

overload \*



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return (PauliOp_left \* PauliOp_right)

.. index:: pair: function; operator+=
.. _doxid-class_q_panda_1_1_pauli_op_1a27be3f087ea755a6f215362c5da07927:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp& operator += (const PauliOp& rhs)

overload +=



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return (PauliOp_left += PauliOp_right)

.. index:: pair: function; operator-=
.. _doxid-class_q_panda_1_1_pauli_op_1ac708f5038b0de144ef7e769ef774dc57:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp& operator -= (const PauliOp& rhs)

overload -=



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return (PauliOp_left -= PauliOp_right)

.. index:: pair: function; operator*=
.. _doxid-class_q_panda_1_1_pauli_op_1a8471110ff429d2a4b1b0f16064facc14:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	PauliOp& operator *= (const PauliOp& rhs)

overload \*=



.. rubric:: Returns:

:ref:`PauliOp <doxid-class_q_panda_1_1_pauli_op>` return (PauliOp_left \*= PauliOp_right)

