.. index:: pair: class; QPanda::QubitReferenceInterface
.. _doxid-class_q_panda_1_1_qubit_reference_interface:

class QPanda::QubitReferenceInterface
=====================================

.. toctree::
	:hidden:

:ref:`QubitReferenceInterface <doxid-class_q_panda_1_1_qubit_reference_interface>` abstract class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitFactory.h>
	
	class QubitReferenceInterface
	{
	public:
		// methods
	
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :target:`getExprPtr<doxid-class_q_panda_1_1_qubit_reference_interface_1ae5b90745e942726dfe3d875601265141>`() = 0;
	};

	// direct descendants

	class :ref:`QubitReference<doxid-class_q_panda_1_1_qubit_reference>`;
