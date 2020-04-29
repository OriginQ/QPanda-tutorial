.. index:: pair: class; QPanda::OriginQResult
.. _doxid-class_q_panda_1_1_origin_q_result:

class QPanda::OriginQResult
===========================

.. toctree::
	:hidden:

Implementation class of :ref:`QResult <doxid-class_q_panda_1_1_q_result>`.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginQuantumMachine.h>
	
	class OriginQResult: public :ref:`QPanda::QResult<doxid-class_q_panda_1_1_q_result>`
	{
	public:
		// methods
	
		virtual std::map<std::string, bool> :target:`getResultMap<doxid-class_q_panda_1_1_origin_q_result_1a53b5554637e349b4da6ad914f1978a51>`() const;
		virtual void :target:`append<doxid-class_q_panda_1_1_origin_q_result_1aad1187c91abf0f67400e382648d7ca03>`(std::pair<std::string, bool>);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual std::map<std::string, bool> :ref:`getResultMap<doxid-class_q_panda_1_1_q_result_1a93f97e70bb1d151dc994e4585b7e8c98>`() const = 0;
		virtual void :ref:`append<doxid-class_q_panda_1_1_q_result_1a17fa20d5180973071f3f5af1f2b78dba>`(std::pair<std::string, bool>) = 0;

