.. index:: pair: class; XC_RandomEngine16807
.. _doxid-class_x_c___random_engine16807:

class XC_RandomEngine16807
==========================

.. toctree::
	:hidden:

XC Random Engine.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <RandomEngine.h>
	
	class XC_RandomEngine16807: public :ref:`RandomEngine<doxid-class_random_engine>`
	{
	public:
		// construction
	
		:target:`XC_RandomEngine16807<doxid-class_x_c___random_engine16807_1a038e0714d79c773090205e98397bd0c4>`();
		:target:`XC_RandomEngine16807<doxid-class_x_c___random_engine16807_1a1da22b98aeed83465b4629e687f33f95>`(long long _seed);

		// methods
	
		virtual double :target:`operator ()<doxid-class_x_c___random_engine16807_1adc80d4f226d96edef6b1f83b3ad86854>` ();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual double :ref:`operator ()<doxid-class_random_engine_1a66f6026e7e0305b31b8819d751336109>` () = 0;
		virtual std::vector<double> :ref:`operator ()<doxid-class_random_engine_1a7aec2ba07830e43f20bcf69513aebf85>` (size_t n);

