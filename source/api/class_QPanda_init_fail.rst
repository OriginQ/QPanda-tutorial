.. index:: pair: class; QPanda::init_fail
.. _doxid-class_q_panda_1_1init__fail:

class QPanda::init_fail
=======================

.. toctree::
	:hidden:

QPanda2 init failed exception.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class init_fail: public :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`
	{
	public:
		// construction
	
		:target:`init_fail<doxid-class_q_panda_1_1init__fail_1a2741317ae6125837c59082e62077488d>`();
		:target:`init_fail<doxid-class_q_panda_1_1init__fail_1a302305624f6aaa7ea1a012eb8ce049f5>`(std::string errmsg);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const char* :ref:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();

