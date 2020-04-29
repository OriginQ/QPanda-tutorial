.. index:: pair: class; QPanda::qvm_attributes_error
.. _doxid-class_q_panda_1_1qvm__attributes__error:

class QPanda::qvm_attributes_error
==================================

.. toctree::
	:hidden:

QPanda2 quantum machine attributes error exception.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class qvm_attributes_error: public :ref:`QPanda::QPandaException<doxid-class_q_panda_1_1_q_panda_exception>`
	{
	public:
		// construction
	
		:target:`qvm_attributes_error<doxid-class_q_panda_1_1qvm__attributes__error_1a8e39297c6a3f112629ad2c8ca9530261>`();
		:target:`qvm_attributes_error<doxid-class_q_panda_1_1qvm__attributes__error_1adc1d958339b9aa0f54ee10e5d1381028>`(std::string err);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual const char* :ref:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();

