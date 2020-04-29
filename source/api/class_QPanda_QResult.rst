.. index:: pair: class; QPanda::QResult
.. _doxid-class_q_panda_1_1_q_result:

class QPanda::QResult
=====================

.. toctree::
	:hidden:

:ref:`QResult <doxid-class_q_panda_1_1_q_result>` abstract class, this class contains the result of the quantum measurement.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QResultFactory.h>
	
	class QResult
	{
	public:
		// methods
	
		virtual std::map<std::string, bool> :target:`getResultMap<doxid-class_q_panda_1_1_q_result_1a93f97e70bb1d151dc994e4585b7e8c98>`() const = 0;
		virtual void :target:`append<doxid-class_q_panda_1_1_q_result_1a17fa20d5180973071f3f5af1f2b78dba>`(std::pair<std::string, bool>) = 0;
	};

	// direct descendants

	class :ref:`OriginQResult<doxid-class_q_panda_1_1_origin_q_result>`;
