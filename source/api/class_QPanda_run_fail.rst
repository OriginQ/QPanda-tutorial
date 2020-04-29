.. index:: pair: class; QPanda::run_fail
.. _doxid-class_q_panda_1_1run__fail:

class QPanda::run_fail
======================

.. toctree::
	:hidden:

QPanda2 running time error exception.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class run_fail: public :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`
	{
	public:
		// construction
	
		:target:`run_fail<doxid-class_q_panda_1_1run__fail_1aa0c418b2b08efe912714aead157f4758>`(std::string cls);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const char* :ref:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();

