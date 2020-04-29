.. index:: pair: class; DefaultRandomEngine
.. _doxid-class_default_random_engine:

class DefaultRandomEngine
=========================

.. toctree::
	:hidden:

Default Random Engine.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <RandomEngine.h>
	
	class DefaultRandomEngine: public :ref:`RandomEngine<doxid-class_random_engine>`
	{
	public:
		// construction
	
		:target:`DefaultRandomEngine<doxid-class_default_random_engine_1a15bac1ca6463c675ca607d96f7775896>`();
		:target:`DefaultRandomEngine<doxid-class_default_random_engine_1ad9df05419db42c60175d461dbcd69e63>`(long long seed);

		// methods
	
		virtual double :target:`operator ()<doxid-class_default_random_engine_1aa63d5499057c1475d693499415ca4774>` ();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual double :ref:`operator ()<doxid-class_random_engine_1a66f6026e7e0305b31b8819d751336109>` () = 0;
		virtual std::vector<double> :ref:`operator ()<doxid-class_random_engine_1a7aec2ba07830e43f20bcf69513aebf85>` (size_t n);

