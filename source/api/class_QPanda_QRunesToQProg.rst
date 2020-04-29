.. index:: pair: class; QPanda::QRunesToQProg
.. _doxid-class_q_panda_1_1_q_runes_to_q_prog:

class QPanda::QRunesToQProg
===========================

.. toctree::
	:hidden:

Transform QRunes instruction set To Quantum program.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QRunesToQProg.h>
	
	class QRunesToQProg
	{
	public:
		// fields
	
		:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`* :target:`qvm<doxid-class_q_panda_1_1_q_runes_to_q_prog_1ac41a3f732e3af54799b383c2fd762c4f>`;
		std::vector<:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`> :target:`m_cbit_vec<doxid-class_q_panda_1_1_q_runes_to_q_prog_1a29a9dc59fc354054c62f78dbc721b9d7>`;

		// methods
	
		void :target:`qRunesParser<doxid-class_q_panda_1_1_q_runes_to_q_prog_1a6555a301d1166bc1b193948a8f4e73a3>`(
			std::string,
			:ref:`QProg<doxid-class_q_panda_1_1_q_prog>`&,
			:ref:`QuantumMachine<doxid-class_q_panda_1_1_quantum_machine>`*
			);
	};
