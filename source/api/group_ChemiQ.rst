.. index:: pair: group; ChemiQ
.. _doxid-group___chemi_q:

ChemiQ
======

.. toctree::
	:hidden:

	class_QPanda_Psi4Wrapper.rst

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// classes

	class :ref:`QPanda::Psi4Wrapper<doxid-class_q_panda_1_1_psi4_wrapper>`;

	// global functions

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t :ref:`QPanda::getElectronNum<doxid-group___chemi_q_1ga02b35349588cbecff66ed7b11df23836>`(const std::string& atom);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`QPanda::JordanWignerTransform<doxid-group___chemi_q_1gabe3d00970e6051f8fa3b1723ce700625>`(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`QPanda::JordanWignerTransform<doxid-group___chemi_q_1gaa35e415e385783eec78f5b8f0b6bc70b>`(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermion);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`QPanda::JordanWignerTransform<doxid-group___chemi_q_1ga380e66e8e43918dbf73a0690bef5e9f5>`(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`QPanda::ParityTransform<doxid-group___chemi_q_1gaf59314f2325b2fcde54820e67c5da280>`(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item, size_t maxqubit);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`QPanda::ParityTransform<doxid-group___chemi_q_1gaff1de62492b7cc268d8781bd53209cd3>`(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermio);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`QPanda::ParityTransform<doxid-group___chemi_q_1gaa4e7311a00586689562edc4d0078cb8b>`(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` std::vector<Eigen::MatrixXi> :ref:`QPanda::BKMatrix<doxid-group___chemi_q_1ga91de3b2612b1bbacc6b33ac13466632b>`(size_t qn);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`QPanda::BravyiKitaevTransform<doxid-group___chemi_q_1ga1ce91fc2dab3957e73c6aa3f7b327885>`(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item, size_t maxqubit, std::vector<Eigen::MatrixXi> BK);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`QPanda::BravyiKitaevTransform<doxid-group___chemi_q_1ga4bc6e42d8e1587c1b99c85218e79b0df>`(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion, std::vector<Eigen::MatrixXi> BK);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t :ref:`QPanda::getCCS_N_Trem<doxid-group___chemi_q_1ga1e525807937cc2fb95224ba97872c6ec>`(size_t qn, size_t en);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t :ref:`QPanda::getCCSD_N_Trem<doxid-group___chemi_q_1gabe33b2e96c7837abf24a9026d3fb9476>`(size_t qn, size_t en);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` :ref:`QPanda::getCCS<doxid-group___chemi_q_1ga2dee7304bfeecd7a50d85a2e6c7c910c>`(size_t qn, size_t en, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para_vec);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`QPanda::getCCS<doxid-group___chemi_q_1ga24061dcef88f99903c778485d0b79e0e>`(size_t qn, size_t en, :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`QPanda::getCCS<doxid-group___chemi_q_1ga14ad05ec8598381b3ae4719810e279f1>`(size_t qn, size_t en, std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` :ref:`QPanda::getCCSD<doxid-group___chemi_q_1ga4eace51dd20fd3c5878174e6e3c95a59>`(size_t qn, size_t en, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para_vec);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`QPanda::getCCSD<doxid-group___chemi_q_1ga5fd9958db5f1b82d4e10de9298b1a340>`(size_t qn, size_t en, :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` :ref:`QPanda::getCCSD<doxid-group___chemi_q_1ga05b705ee2069c55b9c13781634f2b0f6>`(size_t qn, size_t en, std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& para);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`QPanda::transCC2UCC<doxid-group___chemi_q_1ga59ff6451901ac75cfce2308a8c9becc6>`(const :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`& cc);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` :ref:`QPanda::transCC2UCC<doxid-group___chemi_q_1gaae2511f96ce8c475dd606b1dbe279c82>`(const :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`& cc);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` :ref:`QPanda::simulateHamiltonian<doxid-group___chemi_q_1gac65531ce19de3b5766bc33b1dca2c014>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`& pauli, double t, size_t slices);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` :ref:`QPanda::simulateOneTerm<doxid-group___chemi_q_1ga97962c33b3af98a7a1e25d9ba716e82e>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, const :ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`& hamiltonian_term, const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& coef, double t);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` :ref:`QPanda::simulateZTerm<doxid-group___chemi_q_1gadf8fdd11093b481f74988c0330591a63>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& coef, double t);
	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` :ref:`QPanda::parsePsi4DataToFermion<doxid-group___chemi_q_1ga4995c648e2dc98bbb2344483ac2b31ab>`(const std::string& data);

.. _details-group___chemi_q:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. index:: pair: function; getElectronNum
.. _doxid-group___chemi_q_1ga02b35349588cbecff66ed7b11df23836:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t QPanda::getElectronNum(const std::string& atom)

get the electron number of the atom.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- atom



.. rubric:: Returns:

size_t atom's electorn number

.. index:: pair: function; JordanWignerTransform
.. _doxid-group___chemi_q_1gabe3d00970e6051f8fa3b1723ce700625:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` QPanda::JordanWignerTransform(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item)

Jordan-Wigner transform of one fermion term, like "3+ 1 2+ 0".



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- OrbitalActVec&

		- fermion term



.. rubric:: Returns:

PauliOperator



.. rubric:: See also:

:ref:`OrbitalActVec <doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; JordanWignerTransform
.. _doxid-group___chemi_q_1gaa35e415e385783eec78f5b8f0b6bc70b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` QPanda::JordanWignerTransform(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermion)

Jordan-Wigner transform from FermionOperator to PauliOperator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- FermionOperator&

		- fermion operator



.. rubric:: Returns:

PauliOperator



.. rubric:: See also:

:ref:`FermionOperator <doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; JordanWignerTransform
.. _doxid-group___chemi_q_1ga380e66e8e43918dbf73a0690bef5e9f5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` QPanda::JordanWignerTransform(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion)

Jordan-Wigner transform from VarFermionOperator to VarPauliOperator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- VarFermionOperator&

		- variational fermion operator



.. rubric:: Returns:

VarPauliOperator



.. rubric:: See also:

:ref:`VarFermionOperator <doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`

:ref:`VarPauliOperator <doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`

.. index:: pair: function; ParityTransform
.. _doxid-group___chemi_q_1gaf59314f2325b2fcde54820e67c5da280:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` QPanda::ParityTransform(const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item, size_t maxqubit)

Parity transform of one fermion term, like "3+ 1 2+ 0".



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- OrbitalActVec&

		- fermion term

	*
		- size_t

		- maxqubit



.. rubric:: Returns:

PauliOperator



.. rubric:: See also:

:ref:`OrbitalActVec <doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; ParityTransform
.. _doxid-group___chemi_q_1gaff1de62492b7cc268d8781bd53209cd3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` QPanda::ParityTransform(const :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`& fermio)

Parity transform from FermionOperator to PauliOperator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- FermionOperator&

		- fermion operator



.. rubric:: Returns:

PauliOperator



.. rubric:: See also:

:ref:`FermionOperator <doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; ParityTransform
.. _doxid-group___chemi_q_1gaa4e7311a00586689562edc4d0078cb8b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` QPanda::ParityTransform(const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion)

Parity transform from VarFermionOperator to VarPauliOperator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- VarFermionOperator&

		- variational fermion operator



.. rubric:: Returns:

VarPauliOperator



.. rubric:: See also:

:ref:`VarFermionOperator <doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`

:ref:`VarPauliOperator <doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`

.. index:: pair: function; BKMatrix
.. _doxid-group___chemi_q_1ga91de3b2612b1bbacc6b33ac13466632b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` std::vector<Eigen::MatrixXi> QPanda::BKMatrix(size_t qn)

BKMatrix required by BravyiKitaev transform.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- qn quantum number

.. index:: pair: function; BravyiKitaevTransform
.. _doxid-group___chemi_q_1ga1ce91fc2dab3957e73c6aa3f7b327885:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` QPanda::BravyiKitaevTransform(
		const :ref:`OrbitalActVec<doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`& fermion_item,
		size_t maxqubit,
		std::vector<Eigen::MatrixXi> BK
		)

BravyiKitaev transform of one fermion term, like "3+ 1 2+ 0".



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- OrbitalActVec&

		- fermion term

	*
		- size_t

		- maxqubit

	*
		- std::vector<Eigen::MatrixXi>

		- BK



.. rubric:: Returns:

PauliOperator



.. rubric:: See also:

:ref:`OrbitalActVec <doxid-namespace_q_panda_1ab0dc65ba7e826d5d8a74e1660ff2db0f>`

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; BravyiKitaevTransform
.. _doxid-group___chemi_q_1ga4bc6e42d8e1587c1b99c85218e79b0df:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` QPanda::BravyiKitaevTransform(
		const :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`& fermion,
		std::vector<Eigen::MatrixXi> BK
		)

BravyiKitaev transform from VarFermionOperator to VarPauliOperator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- VarFermionOperator&

		- variational fermion operator

	*
		- std::vector<Eigen::MatrixXi>

		- BK



.. rubric:: Returns:

VarPauliOperator



.. rubric:: See also:

:ref:`VarFermionOperator <doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>`

:ref:`VarPauliOperator <doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`

.. index:: pair: function; getCCS_N_Trem
.. _doxid-group___chemi_q_1ga1e525807937cc2fb95224ba97872c6ec:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t QPanda::getCCS_N_Trem(size_t qn, size_t en)

get CCS term number.

Coupled cluster single model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number



.. rubric:: Returns:

size_t CCS term number

.. index:: pair: function; getCCSD_N_Trem
.. _doxid-group___chemi_q_1gabe33b2e96c7837abf24a9026d3fb9476:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` size_t QPanda::getCCSD_N_Trem(size_t qn, size_t en)

get CCSD term number.

Coupled cluster single and double model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3,01->23



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number



.. rubric:: Returns:

size_t CCSD term number

.. index:: pair: function; getCCS
.. _doxid-group___chemi_q_1ga2dee7304bfeecd7a50d85a2e6c7c910c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` QPanda::getCCS(size_t qn, size_t en, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para_vec)

get Coupled cluster single model.

Coupled cluster single model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3. returned FermionOperator like this: {{"2+ 0":para0},{"3+ 0":para1},{"2+ 1":para2},{"3+ 1":para3}}



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number

	*
		- vector_d&

		- parameters



.. rubric:: Returns:

FermionOperator

.. index:: pair: function; getCCS
.. _doxid-group___chemi_q_1ga24061dcef88f99903c778485d0b79e0e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` QPanda::getCCS(size_t qn, size_t en, :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& para)

get Coupled cluster single model with variational parameters.

Coupled cluster single model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3. returned FermionOperator like this: {{"2+ 0":var[0]},{"3+ 0":var[1]},{"2+ 1":var[2]},{"3+ 1":var[3]}}



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number

	*
		- var

		- parameters



.. rubric:: Returns:

VarFermionOperator

.. index:: pair: function; getCCS
.. _doxid-group___chemi_q_1ga14ad05ec8598381b3ae4719810e279f1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` QPanda::getCCS(size_t qn, size_t en, std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& para)

get Coupled cluster single model with variational parameters.

Coupled cluster single model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3. returned FermionOperator like this: {{"2+ 0":var[0]},{"3+ 0":var[1]},{"2+ 1":var[2]},{"3+ 1":var[3]}}



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number

	*
		- std::vector<var>&

		- parameters



.. rubric:: Returns:

VarFermionOperator

.. index:: pair: function; getCCSD
.. _doxid-group___chemi_q_1ga4eace51dd20fd3c5878174e6e3c95a59:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` QPanda::getCCSD(size_t qn, size_t en, const :ref:`vector_d<doxid-namespace_q_panda_1abd75614c36cdeea208f1fbcd1d857021>`& para_vec)

get Coupled cluster single and double model.

Coupled cluster single and double model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3,01->23. returned FermionOperator like this: {{"2+ 0":para0},{"3+ 0":para1},{"2+ 1":para2},{"3+ 1":para3}, {"3+ 2+ 1 0":para5}}



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number

	*
		- vector_d&

		- parameters



.. rubric:: Returns:

FermionOperator

.. index:: pair: function; getCCSD
.. _doxid-group___chemi_q_1ga5fd9958db5f1b82d4e10de9298b1a340:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` QPanda::getCCSD(size_t qn, size_t en, :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& para)

get Coupled cluster single and double model with variational parameters.

Coupled cluster single and double model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3,01->23. returned FermionOperator like this: {{"2+ 0":var[0]},{"3+ 0":var[1]},{"2+ 1":var[2]},{"3+ 1":var[3]}, {"3+ 2+ 1 0":var[4]}}



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number

	*
		- var&

		- parameters



.. rubric:: Returns:

VarFermionOperator

.. index:: pair: function; getCCSD
.. _doxid-group___chemi_q_1ga05b705ee2069c55b9c13781634f2b0f6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarFermionOperator<doxid-namespace_q_panda_1a17f74e31cddb92decd205da7b8e77607>` QPanda::getCCSD(size_t qn, size_t en, std::vector<:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`>& para)

get Coupled cluster single and double model with variational parameters.

Coupled cluster single and double model. e.g. 4 qubits, 2 electrons then 0 and 1 are occupied,just consider 0->2,0->3,1->2,1->3,01->23. returned FermionOperator like this: {{"2+ 0":var[0]},{"3+ 0":var[1]},{"2+ 1":var[2]},{"3+ 1":var[3]}, {"3+ 2+ 1 0":var[4]}}



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- quantum number(orbital number)

	*
		- size_t

		- electron number

	*
		- std::vector<var>&

		- parameters



.. rubric:: Returns:

VarFermionOperator

.. index:: pair: function; transCC2UCC
.. _doxid-group___chemi_q_1ga59ff6451901ac75cfce2308a8c9becc6:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` QPanda::transCC2UCC(const :ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`& cc)

Generate Hamiltonian form of unitary coupled cluster based on coupled cluster,H=1j\*(T-dagger(T)), then exp(-jHt)=exp(T-dagger(T)).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- PauliOperator&

		- pauli operator



.. rubric:: Returns:

PauliOperator



.. rubric:: See also:

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; transCC2UCC
.. _doxid-group___chemi_q_1gaae2511f96ce8c475dd606b1dbe279c82:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>` QPanda::transCC2UCC(const :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`& cc)

Generate Hamiltonian form of unitary coupled cluster based on coupled cluster,H=1j\*(T-dagger(T)), then exp(-jHt)=exp(T-dagger(T)).



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- VarPauliOperator&

		- pauli operator



.. rubric:: Returns:

VarPauliOperator



.. rubric:: See also:

:ref:`VarPauliOperator <doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`

.. index:: pair: function; simulateHamiltonian
.. _doxid-group___chemi_q_1gac65531ce19de3b5766bc33b1dca2c014:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` QPanda::simulateHamiltonian(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, :ref:`VarPauliOperator<doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`& pauli, double t, size_t slices)

Simulate a general case of hamiltonian by Trotter-Suzuki approximation. U=exp(-iHt)=(exp(-i H1 t/n)\*exp(-i H2 t/n))^n.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- the qubit needed to simulate the Hamiltonian

	*
		- VarPauliOperator&

		- Hamiltonian

	*
		- double

		- time

	*
		- size_t

		- the approximate slices



.. rubric:: Returns:

VQC



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

:ref:`VarPauliOperator <doxid-namespace_q_panda_1a50773dfd94ea5c4d4500db137ef3fd0b>`

:ref:`QPanda::Variational::VQC <doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>`

.. index:: pair: function; simulateOneTerm
.. _doxid-group___chemi_q_1ga97962c33b3af98a7a1e25d9ba716e82e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` QPanda::simulateOneTerm(
		:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec,
		const :ref:`QTerm<doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`& hamiltonian_term,
		const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& coef,
		double t
		)

Simulate a single term of Hamilonian like "X0 Y1 Z2" with coefficient and time. U=exp(-it\*coef\*H)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- the qubit needed to simulate the Hamiltonian

	*
		- QTerm&

		- Hamiltonian term, string like "X0 Y1 Z2"

	*
		- var&

		- the coefficient of hamiltonian

	*
		- double

		- time



.. rubric:: Returns:

VQC



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

:ref:`QTerm <doxid-namespace_q_panda_1a0985a180971aab50d40a76b537ce41b4>`

:ref:`QPanda::Variational::var <doxid-class_q_panda_1_1_variational_1_1var>`

.. index:: pair: function; simulateZTerm
.. _doxid-group___chemi_q_1gadf8fdd11093b481f74988c0330591a63:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`VQC<doxid-namespace_q_panda_1_1_variational_1aa01695a2d2bcd70b7b1e083bedca3a78>` QPanda::simulateZTerm(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubit_vec, const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& coef, double t)

Simulating z-only term like H=coef \* (Z0..Zn-1) U=exp(-iHt)



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- QVec&

		- the qubit needed to simulate the Hamiltonian

	*
		- var&

		- the coefficient of hamiltonian

	*
		- double

		- time



.. rubric:: Returns:

VQC



.. rubric:: See also:

:ref:`QVec <doxid-class_q_panda_1_1_q_vec>`

:ref:`QPanda::Variational::var <doxid-class_q_panda_1_1_variational_1_1var>`

.. index:: pair: function; parsePsi4DataToFermion
.. _doxid-group___chemi_q_1ga4995c648e2dc98bbb2344483ac2b31ab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`DLLEXPORT<doxid-_data_struct_8h_1a808e08638be3cba36e36759e5b150de0>` :ref:`FermionOperator<doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>` QPanda::parsePsi4DataToFermion(const std::string& data)

Parse psi4 data to fermion operator.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- fermon str



.. rubric:: Returns:

FermionOperator



.. rubric:: See also:

:ref:`FermionOperator <doxid-namespace_q_panda_1afcd83a197db0cc0e39bac53a6f0092b0>`

