.. index:: pair: class; SharedMutex
.. _doxid-class_shared_mutex:

class SharedMutex
=================

.. toctree::
	:hidden:

Shared Mutex.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ReadWriteLock.h>
	
	class SharedMutex
	{
	public:
		// methods
	
		void :target:`read<doxid-class_shared_mutex_1aef8e97d77f53845a197e9c13534ff265>`();
		void :target:`unread<doxid-class_shared_mutex_1a33d771a7b909887e22c714de65259705>`();
		void :target:`write<doxid-class_shared_mutex_1af91758e1961d8d6a26dd2ab675f32f2e>`();
		void :target:`unwrite<doxid-class_shared_mutex_1a25d984199159730b26467702b4ae55f9>`();
	};
