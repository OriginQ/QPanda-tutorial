.. index:: pair: class; AbstractQuantumGates
.. _doxid-class_abstract_quantum_gates:

class AbstractQuantumGates
==========================

.. toctree::
	:hidden:

Quantum Gates Abstract Class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPUImpl.h>
	
	class AbstractQuantumGates
	{
	public:
		// methods
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`DiagonalGate<doxid-class_abstract_quantum_gates_1a78cc1d15bb73259db199ed035362f808>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`controlDiagonalGate<doxid-class_abstract_quantum_gates_1a08d83f9dbc46ffab2eae6f5e6d04506e>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vQubit,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>`& matrix,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Reset<doxid-class_abstract_quantum_gates_1a00820295b63c5ddab850015ca7708c07>`(size_t qn) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Hadamard<doxid-class_abstract_quantum_gates_1a55abfc9edb5b481a8e8e58dd9828b5b0>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Hadamard<doxid-class_abstract_quantum_gates_1a0fdaf9c6d7f5c63cdb529fa7984e0dab>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`X<doxid-class_abstract_quantum_gates_1aa175a2b9d84e0a96e7239daea49035ec>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`X<doxid-class_abstract_quantum_gates_1a589268271ad2911b71521543cbf2c66e>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P0<doxid-class_abstract_quantum_gates_1aa3249fae7d44e63358b5183cb6acd2aa>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P0<doxid-class_abstract_quantum_gates_1a42c4a882e32b351e2586623f0d13ca38>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P1<doxid-class_abstract_quantum_gates_1a534f6f6aef56107d021d98c2c8650740>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`P1<doxid-class_abstract_quantum_gates_1afb921860cfd277adda464304908e0412>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Y<doxid-class_abstract_quantum_gates_1acb392fba6631ac12e5ade2753912f92a>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Y<doxid-class_abstract_quantum_gates_1a619b20095f7312e94506c825dee16c7e>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Z<doxid-class_abstract_quantum_gates_1a7b21ffe21f90dd0ec6f9eed2679ea502>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`Z<doxid-class_abstract_quantum_gates_1ab1c3d742e891b7502e130c0c9e0141ba>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`T<doxid-class_abstract_quantum_gates_1a8011a1f1985434e3a51168f495dd2787>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`T<doxid-class_abstract_quantum_gates_1aa09a2f9b91f191590392e3bcabd8f399>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`S<doxid-class_abstract_quantum_gates_1a50ed48b3702e1eb754d57900840f238e>`(
			size_t qn,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`S<doxid-class_abstract_quantum_gates_1aacbff8fab6ba3142da7272d91043f4df>`(
			size_t qn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`U1_GATE<doxid-class_abstract_quantum_gates_1a0897b2ab1384e2bdc387dedcf8b3e706>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RX_GATE<doxid-class_abstract_quantum_gates_1a3f25fa0f88fabc46feafb09f99980fd1>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RX_GATE<doxid-class_abstract_quantum_gates_1a3a03bc88a6050555b406fa3f22b48226>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RY_GATE<doxid-class_abstract_quantum_gates_1a18def18d6997e2d0778b4094bc9d0e2c>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RY_GATE<doxid-class_abstract_quantum_gates_1ac4b33afa1543170593cbea81b45d1756>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RZ_GATE<doxid-class_abstract_quantum_gates_1aeb947f50f5e11eeb0f11cb73ab0cf17d>`(
			size_t qn,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`RZ_GATE<doxid-class_abstract_quantum_gates_1a38c5c274dc664ade2a2552cdaec6b939>`(
			size_t qn,
			double theta,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CNOT<doxid-class_abstract_quantum_gates_1a3da6e802acda49c081906aaa74b43a94>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CNOT<doxid-class_abstract_quantum_gates_1ab391b4acb45fe38e9c5de4f4c0163154>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CR<doxid-class_abstract_quantum_gates_1a241e1bd23ca6530d8867fd448353dce0>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CR<doxid-class_abstract_quantum_gates_1ac11931f80f4470e2af2598a78cd70e40>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CZ<doxid-class_abstract_quantum_gates_1a691dc6df010e984c1946579e9b8deec2>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`CZ<doxid-class_abstract_quantum_gates_1a16b4a967ce69c2507990743153053760>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_abstract_quantum_gates_1a81383c53f2e1bff4cc6e94663c1a04da>`(
			size_t qn_0,
			size_t qn_1,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_abstract_quantum_gates_1a738e9c6b8a7a682a4ef44482e332bbdc>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			double theta,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_abstract_quantum_gates_1aadcee9056669d7ee040188e4d152ad1d>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`iSWAP<doxid-class_abstract_quantum_gates_1a77f58f532c8d481d4bf74aae890bca41>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`SqiSWAP<doxid-class_abstract_quantum_gates_1aaa5ed642ae9f360393abea95f672630a>`(
			size_t qn_0,
			size_t qn_1,
			bool isConjugate,
			double error_rate
			) = 0;
	
		virtual :ref:`QError<doxid-_q_error_8h_1af306abe1caf901637ac7f16626512874>` :target:`SqiSWAP<doxid-class_abstract_quantum_gates_1aa548a75b5ec73a5eb0ae44cab11c3a3b>`(
			size_t qn_0,
			size_t qn_1,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& vControlBit,
			bool isConjugate,
			double error_rate
			) = 0;
	};
