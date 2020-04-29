.. index:: pair: class; QPanda::complex_var
.. _doxid-class_q_panda_1_1complex__var:

class QPanda::complex_var
=========================

.. toctree::
	:hidden:

complex number variate


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <complex_var.h>
	
	class complex_var
	{
	public:
		// construction
	
		:target:`complex_var<doxid-class_q_panda_1_1complex__var_1a822933951877bae9a28fadf6f4e1bcf1>`();
		:target:`complex_var<doxid-class_q_panda_1_1complex__var_1ac781c5aa5741360954415e1739e5fbbf>`(const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& value);
	
		:target:`complex_var<doxid-class_q_panda_1_1complex__var_1a4d2081718998f8b2e85b4d86c68d8af2>`(
			const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& v1,
			const :ref:`var<doxid-class_q_panda_1_1_variational_1_1var>`& v2
			);

		// methods
	
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`real<doxid-class_q_panda_1_1complex__var_1a064d20f8ad1f9ff57b90cdc0c5e7f33f>`();
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var>` :target:`imag<doxid-class_q_panda_1_1complex__var_1a7b5226c2a611fb7c2fc342982b362673>`();
		const complex_var :target:`operator +<doxid-class_q_panda_1_1complex__var_1aa974a0d2fed6bc02a9755fa8b24e94ea>` (const complex_var& value);
		const complex_var :target:`operator -<doxid-class_q_panda_1_1complex__var_1a23b2ae8f7485f3d5ff82607841549e10>` (const complex_var& value);
		const complex_var :target:`operator *<doxid-class_q_panda_1_1complex__var_1a74e4f5e97fe0e6ad495b8f1916f95d37>` (const complex_var& value);
		const complex_var :target:`operator/<doxid-class_q_panda_1_1complex__var_1ac2c3fff0771ee379eaa3b0ec88cddb88>` (const complex_var& value);
	};
