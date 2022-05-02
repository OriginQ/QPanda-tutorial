.. index:: pair: class; QPanda::QVec
.. _doxid-class_q_panda_1_1_q_vec:

class QPanda::QVec
==================

.. toctree::
	:hidden:

:ref:`Qubit <doxid-class_q_panda_1_1_qubit>` vector basic class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QVec.h>
	
	class QVec: public std::vector< Qubit * >
	{
	public:
		// construction
	
		:target:`QVec<doxid-class_q_panda_1_1_q_vec_1a80289892f90b3d1a243cceaa05383d14>`(
			BaseClass::iterator iter_begin,
			BaseClass::iterator iter_end
			);
	
		:target:`QVec<doxid-class_q_panda_1_1_q_vec_1adc43c7984a6ab4ad7af3bc588eddcdd8>`(const std::initializer_list<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*>& args);
		:target:`QVec<doxid-class_q_panda_1_1_q_vec_1aa65b4b0b4a7a6ff588ea9ead6d15be94>`();
		:target:`QVec<doxid-class_q_panda_1_1_q_vec_1a0a5592c63af91a98f21d46e8ac309951>`(const QVec& old);
		:target:`QVec<doxid-class_q_panda_1_1_q_vec_1ac0caea1df1a1c6a778bac02d98ba55ca>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* q);
		:target:`QVec<doxid-class_q_panda_1_1_q_vec_1afb5abbec08fc45a6b4d1cc322ef26c91>`(BaseClass& vector);

		// methods
	
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :target:`operator []<doxid-class_q_panda_1_1_q_vec_1a9d1d01c894ac4181f4c1ecc48b43632f>` (:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& classical_cond);
		:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :target:`operator []<doxid-class_q_panda_1_1_q_vec_1a644d0e5e93622e405b42e732867b23f0>` (size_t pos) const;
		reference :target:`operator []<doxid-class_q_panda_1_1_q_vec_1a04234464aac80a7d9f64e02c24a13572>` (size_type _Pos);
		QVec& :target:`operator <<<doxid-class_q_panda_1_1_q_vec_1ab8765740f0841085a7613ec3ac536dac>` (int);
		QVec :target:`operator +<doxid-class_q_panda_1_1_q_vec_1ada011b04064089acab6982fcda7e608a>` (QVec vec) const;
		QVec& :target:`operator +=<doxid-class_q_panda_1_1_q_vec_1acf9426af7bdc30e85583ccc5c456692a>` (QVec vec);
		QVec :target:`operator -<doxid-class_q_panda_1_1_q_vec_1a019b83968b0d5717dc23d202328e928b>` (QVec vec) const;
		QVec& :target:`operator -=<doxid-class_q_panda_1_1_q_vec_1adf95630d28d8122d24e7dc7bc85e76d8>` (QVec vec);
	};
