.. index:: pair: struct; QPanda::KakDescription
.. _doxid-struct_q_panda_1_1_kak_description:

struct QPanda::KakDescription
=============================

.. toctree::
	:hidden:

Kak description of an arbitrary two-qubit operation. U = g x (Gate A1 Gate A0) x exp(i(xXX + yYY + zZZ))x(Gate b1 Gate b0) A global phase factor Two single-qubit operations (before): Gate b0, b1 The Exp() circuit specified by 3 coefficients (x, y, z) Two single-qubit operations (after): Gate a0, a1.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <KAK.h>
	
	struct KakDescription
	{
		// fields
	
		Eigen::Matrix4cd :target:`in_matrix<doxid-struct_q_panda_1_1_kak_description_1a368fa867fb72e5f8cd0bb00339bbc4fb>`;
		std::complex<double> :target:`global_phase<doxid-struct_q_panda_1_1_kak_description_1ae3f22f312d166884000d6c0dcd353948>`;
		Eigen::Matrix2cd :target:`b0<doxid-struct_q_panda_1_1_kak_description_1ab5cc88d52426852ca62a833131e4e226>`;
		Eigen::Matrix2cd :target:`b1<doxid-struct_q_panda_1_1_kak_description_1aed10a5dd9dbadd5557e8cf09b7e54ca0>`;
		Eigen::Matrix2cd :target:`a0<doxid-struct_q_panda_1_1_kak_description_1a68da29f31b78be2d9fc3ef77f6e813e6>`;
		Eigen::Matrix2cd :target:`a1<doxid-struct_q_panda_1_1_kak_description_1a09614d18b18f55f7116e79ec47e7f79e>`;
		double :target:`x<doxid-struct_q_panda_1_1_kak_description_1a38d17a1f3b412e0e53abd678a5bfb44b>`;
		double :target:`y<doxid-struct_q_panda_1_1_kak_description_1ae635a0efd5845859278e9f7d5b3adb13>`;
		double :target:`z<doxid-struct_q_panda_1_1_kak_description_1a8f0c02ce7e10205ae57d08e7428153f4>`;

		// methods
	
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`to_qcircuit<doxid-struct_q_panda_1_1_kak_description_1adbb49e660a31c275c4a48b4a7b1ba9dd>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* in_bit1,
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* in_bit2
			) const;
	
		Eigen::MatrixXcd :target:`to_matrix<doxid-struct_q_panda_1_1_kak_description_1abb75a44e2550ec53fbc70505148584ea>`() const;
	};
