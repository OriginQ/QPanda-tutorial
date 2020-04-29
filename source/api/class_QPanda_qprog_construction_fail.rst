.. index:: pair: class; QPanda::qprog_construction_fail
.. _doxid-class_q_panda_1_1qprog__construction__fail:

class QPanda::qprog_construction_fail
=====================================

.. toctree::
	:hidden:

QPanda2 quantum program construction failed exception.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class qprog_construction_fail: public :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`
	{
	public:
		// construction
	
		:target:`qprog_construction_fail<doxid-class_q_panda_1_1qprog__construction__fail_1add3f56ccf6429b4ec10973f4e3d1bde5>`();
		:target:`qprog_construction_fail<doxid-class_q_panda_1_1qprog__construction__fail_1a6cf4c7dfe4052a7a7d7a771884d34862>`(std::string err);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const char* :ref:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();

