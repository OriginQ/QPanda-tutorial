.. index:: pair: class; RandomEngine
.. _doxid-class_random_engine:

class RandomEngine
==================

.. toctree::
	:hidden:

Random Engine.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <RandomEngine.h>
	
	class RandomEngine
	{
	public:
		// methods
	
		virtual double :target:`operator ()<doxid-class_random_engine_1a66f6026e7e0305b31b8819d751336109>` () = 0;
		virtual std::vector<double> :target:`operator ()<doxid-class_random_engine_1a7aec2ba07830e43f20bcf69513aebf85>` (size_t n);
	};

	// direct descendants

	class :ref:`DefaultRandomEngine<doxid-class_default_random_engine>`;
	class :ref:`XC_RandomEngine16807<doxid-class_x_c___random_engine16807>`;
