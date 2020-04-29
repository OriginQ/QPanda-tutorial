.. index:: pair: struct; std::hash<QPanda::Variational::var>
.. _doxid-structstd_1_1hash_3_01_q_panda_1_1_variational_1_1var_01_4:

template struct std::hash<QPanda::Variational::var>
===================================================

.. toctree::
	:hidden:

hash function to enable unordered_map<var, _Ty> and unordered_set **


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	template <>
	struct hash<QPanda::Variational::var>
	{
		// methods
	
		size_t :target:`operator ()<doxid-structstd_1_1hash_3_01_q_panda_1_1_variational_1_1var_01_4_1a5f7288caefd34059d9a768540c63174e>` (const :ref:`QPanda::Variational::var<doxid-class_q_panda_1_1_variational_1_1var>`&) const;
	};
