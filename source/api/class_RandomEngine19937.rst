.. index:: pair: class; RandomEngine19937
.. _doxid-class_random_engine19937:

class RandomEngine19937
=======================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <RandomEngine.h>
	
	class RandomEngine19937
	{
	public:
		// methods
	
		void :target:`set_random_seed<doxid-class_random_engine19937_1a0784f207dd0e141b4b7944a803a3a971>`();
		void :target:`set_random_seed<doxid-class_random_engine19937_1a232e840cc763b175655d90a1fe5b7cd4>`(size_t seed);
	
		double :target:`random_double<doxid-class_random_engine19937_1a4996a40872b4d71b8effb446f30f33c3>`(
			double a = 0.,
			double b = 1.
			);
	
		template <typename Float = double>
		int :target:`random_discrete<doxid-class_random_engine19937_1ab65c8f0426b5f3f4ea813452b64bcc10>`(const std::vector<Float>& probs);
	};
