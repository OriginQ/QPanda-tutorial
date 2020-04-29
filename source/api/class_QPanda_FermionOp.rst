.. index:: pair: class; QPanda::FermionOp
.. _doxid-class_q_panda_1_1_fermion_op:

template class QPanda::FermionOp
================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Fermion operator class. :ref:`More...<details-class_q_panda_1_1_fermion_op>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <FermionOperator.h>
	
	template <class T>
	class FermionOp
	{
	public:
		// typedefs
	
		typedef std::pair<:ref:`FermionPair<doxid-namespace_q_panda_1a4d9726c70eb40664ad8816323dc3420b>`, :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> :target:`FermionItem<doxid-class_q_panda_1_1_fermion_op_1a94692f04e649a20ab7ccd0c23fe5e80b>`;
		typedef std::vector<:ref:`FermionItem<doxid-class_q_panda_1_1_fermion_op_1a94692f04e649a20ab7ccd0c23fe5e80b>`> :target:`FermionData<doxid-class_q_panda_1_1_fermion_op_1a009e7a97ab23ac6a5c3e014ad0113ca2>`;
		typedef std::map<std::string, :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> :target:`FermionMap<doxid-class_q_panda_1_1_fermion_op_1a4f204ecb72a2fec10cb8cb94039fbb6c>`;

		// construction
	
		:ref:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1ae4710e465b52a1b56b1d0c97bd56929a>`();
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1a22cec575e183f26090a5fe32c2caedb3>`(double value);
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1a540257177508716a8f8460f1abb1b0fe>`(const :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& value);
	
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1a39211382211efdcad85efce6f666dc9a>`(
			const std::string& key,
			const :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& value
			);
	
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1a75d8682f8c381eaba25feeeff53f3aaa>`(const :ref:`FermionMap<doxid-class_q_panda_1_1_fermion_op_1a4f204ecb72a2fec10cb8cb94039fbb6c>`& map);
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1a5dec315e0e0ef48f9346c0eac16677a8>`(:ref:`FermionData<doxid-class_q_panda_1_1_fermion_op_1a009e7a97ab23ac6a5c3e014ad0113ca2>`&& fermion_data);
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1a57a04aa08013bf741ccd76408ebffb26>`(const :ref:`FermionData<doxid-class_q_panda_1_1_fermion_op_1a009e7a97ab23ac6a5c3e014ad0113ca2>`& fermion_data);
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1aa6aaafd935af1cab24487d41278008a8>`(FermionOp&& op);
		:target:`FermionOp<doxid-class_q_panda_1_1_fermion_op_1a4125e5b9bb3932a92f190ada7c94f255>`(const FermionOp& op);

		// methods
	
		FermionOp& :target:`operator =<doxid-class_q_panda_1_1_fermion_op_1a97a2ab2759613f2638f0fd7acb7eb865>` (const FermionOp& op);
		FermionOp& :target:`operator =<doxid-class_q_panda_1_1_fermion_op_1a41c1ecdd08f5007e64187081ce46114f>` (FermionOp&& op);
		FermionOp :ref:`normal_ordered<doxid-class_q_panda_1_1_fermion_op_1ad16f02b9ddbc3466c220fb7fd18ae7e5>`();
		size_t :ref:`getMaxIndex<doxid-class_q_panda_1_1_fermion_op_1aa467d13b89d78fd50fba699143e9a5c3>`() const;
		bool :ref:`isEmpty<doxid-class_q_panda_1_1_fermion_op_1aa846e43fb4bee4baba398e094ee7539b>`();
		std::string :ref:`toString<doxid-class_q_panda_1_1_fermion_op_1a11876f5e825a2b80d2c24f5a195c2198>`() const;
		void :ref:`setErrorThreshold<doxid-class_q_panda_1_1_fermion_op_1a093667b5c05e17c4ed7e5bf812b0c6ef>`(double threshold);
		double :ref:`error_threshold<doxid-class_q_panda_1_1_fermion_op_1a49b43264ad39bc65662a5fe815c51004>`() const;
		:ref:`FermionData<doxid-class_q_panda_1_1_fermion_op_1a009e7a97ab23ac6a5c3e014ad0113ca2>` :ref:`data<doxid-class_q_panda_1_1_fermion_op_1a0bcbe2d74af638c4de3cafaed6dcf9ec>`() const;
		FermionOp :ref:`operator +<doxid-class_q_panda_1_1_fermion_op_1a69938656824ec1eb840d3aaee7e1e4bf>` (const FermionOp& rhs) const;
		FermionOp :ref:`operator -<doxid-class_q_panda_1_1_fermion_op_1a64adcaf3a76d825a658c48b86394b235>` (const FermionOp& rhs) const;
		FermionOp :ref:`operator *<doxid-class_q_panda_1_1_fermion_op_1a42f03d0bc79b2a79670e5cf5541936cf>` (const FermionOp& rhs) const;
		FermionOp& :ref:`operator +=<doxid-class_q_panda_1_1_fermion_op_1af780055e063f8990f534d50339125200>` (const FermionOp& rhs);
		FermionOp& :ref:`operator -=<doxid-class_q_panda_1_1_fermion_op_1ad7e0dcdcf370dc4678dac2ba25d79108>` (const FermionOp& rhs);
		FermionOp& :ref:`operator *=<doxid-class_q_panda_1_1_fermion_op_1a6249d01799e8d3d24777f0c2954b2bf3>` (const FermionOp& rhs);
	};
.. _details-class_q_panda_1_1_fermion_op:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Fermion operator class.

Construction
------------

.. index:: pair: function; FermionOp
.. _doxid-class_q_panda_1_1_fermion_op_1ae4710e465b52a1b56b1d0c97bd56929a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp()

Constructor of :ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` class.

Methods
-------

.. index:: pair: function; normal_ordered
.. _doxid-class_q_panda_1_1_fermion_op_1ad16f02b9ddbc3466c220fb7fd18ae7e5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp normal_ordered()

Compute and return the normal ordered form of a FermionOperator.

In our convention, normal ordering implies terms are ordered from highest tensor factor (on left) to lowest (on right). In addition: a^\dagger comes before a



.. rubric:: Returns:

:ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` the normal ordered form of a FermionOperator

.. index:: pair: function; getMaxIndex
.. _doxid-class_q_panda_1_1_fermion_op_1aa467d13b89d78fd50fba699143e9a5c3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t getMaxIndex() const

get the max index



.. rubric:: Returns:

size_t the max index

.. index:: pair: function; isEmpty
.. _doxid-class_q_panda_1_1_fermion_op_1aa846e43fb4bee4baba398e094ee7539b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool isEmpty()

Judge whether it is empty.



.. rubric:: Returns:

bool if data is empty, return true, or else return false

.. index:: pair: function; toString
.. _doxid-class_q_panda_1_1_fermion_op_1a11876f5e825a2b80d2c24f5a195c2198:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string toString() const

data to string



.. rubric:: Returns:

std::string convert data val to string

.. index:: pair: function; setErrorThreshold
.. _doxid-class_q_panda_1_1_fermion_op_1a093667b5c05e17c4ed7e5bf812b0c6ef:

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
.. _doxid-class_q_panda_1_1_fermion_op_1a49b43264ad39bc65662a5fe815c51004:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	double error_threshold() const

get error threshold



.. rubric:: Returns:

double return the error threshold val

.. index:: pair: function; data
.. _doxid-class_q_panda_1_1_fermion_op_1a0bcbe2d74af638c4de3cafaed6dcf9ec:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`FermionData<doxid-class_q_panda_1_1_fermion_op_1a009e7a97ab23ac6a5c3e014ad0113ca2>` data() const

get data



.. rubric:: Returns:

FermionData return fermion data

.. index:: pair: function; operator+
.. _doxid-class_q_panda_1_1_fermion_op_1a69938656824ec1eb840d3aaee7e1e4bf:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp operator + (const FermionOp& rhs) const

overload +



.. rubric:: Returns:

:ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` return (FermionOp_1 + FermionOp_2)

.. index:: pair: function; operator-
.. _doxid-class_q_panda_1_1_fermion_op_1a64adcaf3a76d825a658c48b86394b235:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp operator - (const FermionOp& rhs) const

overload -



.. rubric:: Returns:

:ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` return (FermionOp_1 - FermionOp_2)

.. index:: pair: function; operator*
.. _doxid-class_q_panda_1_1_fermion_op_1a42f03d0bc79b2a79670e5cf5541936cf:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp operator * (const FermionOp& rhs) const

overload \*



.. rubric:: Returns:

:ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` return (FermionOp_1 \* FermionOp_2)

.. index:: pair: function; operator+=
.. _doxid-class_q_panda_1_1_fermion_op_1af780055e063f8990f534d50339125200:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp& operator += (const FermionOp& rhs)

overload +=



.. rubric:: Returns:

:ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` & return (FermionOp_1 += FermionOp_2)

.. index:: pair: function; operator-=
.. _doxid-class_q_panda_1_1_fermion_op_1ad7e0dcdcf370dc4678dac2ba25d79108:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp& operator -= (const FermionOp& rhs)

overload -=



.. rubric:: Returns:

:ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` & return (FermionOp_1 -= FermionOp_2)

.. index:: pair: function; operator*=
.. _doxid-class_q_panda_1_1_fermion_op_1a6249d01799e8d3d24777f0c2954b2bf3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	FermionOp& operator *= (const FermionOp& rhs)

overload \*=



.. rubric:: Returns:

:ref:`FermionOp <doxid-class_q_panda_1_1_fermion_op>` & return (FermionOp_1 \*= FermionOp_2)

