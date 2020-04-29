.. index:: pair: class; QPanda::QPandaException
.. _doxid-class_q_panda_1_1_q_panda_exception:

class QPanda::QPandaException
=============================

.. toctree::
	:hidden:

QPanda2 exception basic class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QPandaException.h>
	
	class QPandaException: public exception
	{
	public:
		// construction
	
		:target:`QPandaException<doxid-class_q_panda_1_1_q_panda_exception_1ac7e9edcfef3881928fd79c8ba66b0f13>`();
		:target:`QPandaException<doxid-class_q_panda_1_1_q_panda_exception_1aeb315683d93ef436e0d82b55df82f176>`(const char* str);
		:target:`QPandaException<doxid-class_q_panda_1_1_q_panda_exception_1af8c97da6705b2d62bd2557bb2ed72cc9>`(std::string str);

		// methods
	
		virtual const char* :target:`what<doxid-class_q_panda_1_1_q_panda_exception_1af7f773b6c79e72e396f06e868390428d>`();
	};

	// direct descendants

	class :ref:`calloc_fail<doxid-class_q_panda_1_1calloc__fail>`;
	class :ref:`gate_alloc_fail<doxid-class_q_panda_1_1gate__alloc__fail>`;
	class :ref:`init_fail<doxid-class_q_panda_1_1init__fail>`;
	class :ref:`qalloc_fail<doxid-class_q_panda_1_1qalloc__fail>`;
	class :ref:`qcircuit_construction_fail<doxid-class_q_panda_1_1qcircuit__construction__fail>`;
	class :ref:`qprog_construction_fail<doxid-class_q_panda_1_1qprog__construction__fail>`;
	class :ref:`qprog_syntax_error<doxid-class_q_panda_1_1qprog__syntax__error>`;
	class :ref:`qvm_attributes_error<doxid-class_q_panda_1_1qvm__attributes__error>`;
	class :ref:`result_get_fail<doxid-class_q_panda_1_1result__get__fail>`;
	class :ref:`run_fail<doxid-class_q_panda_1_1run__fail>`;
	class :ref:`undefine_error<doxid-class_q_panda_1_1undefine__error>`;
