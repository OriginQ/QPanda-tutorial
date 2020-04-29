.. index:: pair: class; QPanda::undefine_error
.. _doxid-class_q_panda_1_1undefine__error:

class QPanda::undefine_error
============================

.. toctree::
	:hidden:

QPanda2 undefined error exception.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class undefine_error: public :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`
	{
	public:
		// construction
	
		:target:`undefine_error<doxid-class_q_panda_1_1undefine__error_1a3c05b2b677586b7e7520edd5a0692549>`();
		:target:`undefine_error<doxid-class_q_panda_1_1undefine__error_1a5be9e2570a2438656339e86ca36c2fcb>`(std::string err);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const char* :ref:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();

