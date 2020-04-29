.. index:: pair: class; QPanda::ClassicalProgRegisterAction
.. _doxid-class_q_panda_1_1_classical_prog_register_action:

class QPanda::ClassicalProgRegisterAction
=========================================

.. toctree::
	:hidden:

classical program register action Provide :ref:`ClassicalProgFactory <doxid-class_q_panda_1_1_classical_prog_factory>` class registration interface for the outside


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ClassicalProgram.h>
	
	class ClassicalProgRegisterAction
	{
	public:
		// construction
	
		:target:`ClassicalProgRegisterAction<doxid-class_q_panda_1_1_classical_prog_register_action_1a2489afaa0a63428ffc580468addf2821>`(
			std::string className,
			:ref:`CreateClassicalQProgram<doxid-namespace_q_panda_1a8e863438215e55293e6888776d035fed>` ptrCreateFn
			);
	};
