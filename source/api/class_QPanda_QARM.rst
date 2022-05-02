.. index:: pair: class; QPanda::QARM
.. _doxid-class_q_panda_1_1_q_a_r_m:

class QPanda::QARM
==================

.. toctree::
	:hidden:

Quantum Association Rules Mining.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QARMAlgorithm.h>
	
	class QARM
	{
	public:
		// construction
	
		:target:`QARM<doxid-class_q_panda_1_1_q_a_r_m_1ab40fa2919b029f1b71c398b957d33466>`(std::vector<std::vector<std::string>> data);

		// methods
	
		std::map<std::string, double> :target:`run<doxid-class_q_panda_1_1_q_a_r_m_1af6b9581a793ed73f504b10da0a7b3423>`();
	};
