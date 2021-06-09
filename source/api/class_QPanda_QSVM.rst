.. index:: pair: class; QPanda::QSVM
.. _doxid-class_q_panda_1_1_q_s_v_m:

class QPanda::QSVM
==================

.. toctree::
	:hidden:

Quantum Support Vector Machines.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QSVMAlgorithm.h>
	
	class QSVM
	{
	public:
		// construction
	
		:target:`QSVM<doxid-class_q_panda_1_1_q_s_v_m_1a103d2467fb170b181f122da1a3e10d2c>`(std::vector<std::vector<double>> data);

		// methods
	
		bool :target:`run<doxid-class_q_panda_1_1_q_s_v_m_1afd1eab89cfe0eadd5ad052eb00802885>`(std::vector<double> query_x);
	};
