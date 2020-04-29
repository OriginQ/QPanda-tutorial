.. index:: pair: class; QPanda::qprog_syntax_error
.. _doxid-class_q_panda_1_1qprog__syntax__error:

class QPanda::qprog_syntax_error
================================

.. toctree::
	:hidden:

QPanda2 quantum program syntax error exception.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class qprog_syntax_error: public :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`
	{
	public:
		// construction
	
		:target:`qprog_syntax_error<doxid-class_q_panda_1_1qprog__syntax__error_1ab2ab6fab73042bdb1df4d125f4ecf2eb>`();
		:target:`qprog_syntax_error<doxid-class_q_panda_1_1qprog__syntax__error_1accf63bb78c9e79750794e7b6a560d1d3>`(std::string err);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const char* :ref:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();

