.. index:: pair: class; QPanda::qcircuit_construction_fail
.. _doxid-class_q_panda_1_1qcircuit__construction__fail:

class QPanda::qcircuit_construction_fail
========================================

.. toctree::
	:hidden:

QPanda2 qcircuit construction failed exception.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class qcircuit_construction_fail: public :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`
	{
	public:
		// construction
	
		:target:`qcircuit_construction_fail<doxid-class_q_panda_1_1qcircuit__construction__fail_1a096f4da0679f16736edd52768c8bd16f>`();
		:target:`qcircuit_construction_fail<doxid-class_q_panda_1_1qcircuit__construction__fail_1a8734ce27f8dadb4fd12993b676e75312>`(std::string err);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const char* :ref:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();

