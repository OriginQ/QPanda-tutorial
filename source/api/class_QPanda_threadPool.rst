.. index:: pair: class; QPanda::threadPool
.. _doxid-class_q_panda_1_1thread_pool:

class QPanda::threadPool
========================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ThreadPool.h>
	
	class threadPool
	{
	public:
		// methods
	
		bool :ref:`init_thread_pool<doxid-class_q_panda_1_1thread_pool_1a6a40bdbf0dc7415e10541f6c1daf1ce4>`(size_t thread_cnt = :ref:`DEFAULT_THREAD_CNT<doxid-_thread_pool_8h_1afaec1f11c35702b38040be5ed91dfd5e>`);
		bool :target:`append<doxid-class_q_panda_1_1thread_pool_1a53de8c5a8e2a0e2b93d5a4d6e1c45ea6>`(:ref:`Task<doxid-namespace_q_panda_1a4e7214f955f8b0df9fceed3d90b5645c>` task);
	};
.. _details-class_q_panda_1_1thread_pool:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; init_thread_pool
.. _doxid-class_q_panda_1_1thread_pool_1a6a40bdbf0dc7415e10541f6c1daf1ce4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool init_thread_pool(size_t thread_cnt = :ref:`DEFAULT_THREAD_CNT<doxid-_thread_pool_8h_1afaec1f11c35702b38040be5ed91dfd5e>`)

init thread pool



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- size_t

		- Number of threads in the thread pool, 8 by default



.. rubric:: Returns:

void

