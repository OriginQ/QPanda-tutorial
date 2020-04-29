.. index:: pair: class; QPanda::Brent
.. _doxid-class_q_panda_1_1_brent:

class QPanda::Brent
===================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Given a function of one-variable, return the local minimum of the function isolated to a fractional precision of tol. :ref:`More...<details-class_q_panda_1_1_brent>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginPowell.h>
	
	class Brent
	{
	public:
		// construction
	
		:ref:`Brent<doxid-class_q_panda_1_1_brent_1a8b1b8b370ab4f3c0c33d8b7a159b363b>`(const Func& func, double tol = 1.48e-8, size_t maxiter = 500);
		:target:`Brent<doxid-class_q_panda_1_1_brent_1aa29261ea2e78fb370a00ce0ea54c59fe>`(const Brent&);

		// methods
	
		Brent& :target:`operator =<doxid-class_q_panda_1_1_brent_1abfd9b97209de7ab87c8a2832131f52e4>` (const Brent&);
		void :ref:`optimize<doxid-class_q_panda_1_1_brent_1a0659715752c2f9324f0a739d9c3125db>`();
		std::pair<double, :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`> :ref:`getResult<doxid-class_q_panda_1_1_brent_1a1c86398e34b833da2d1b78e65ca765b8>`();
	};
.. _details-class_q_panda_1_1_brent:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Given a function of one-variable, return the local minimum of the function isolated to a fractional precision of tol.

Uses inverse parabolic interpolation when possible to speed up convergence of golden section method.

Construction
------------

.. index:: pair: function; Brent
.. _doxid-class_q_panda_1_1_brent_1a8b1b8b370ab4f3c0c33d8b7a159b363b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Brent(const Func& func, double tol = 1.48e-8, size_t maxiter = 500)

Constructor of :ref:`Brent <doxid-class_q_panda_1_1_brent>`.

Methods
-------

.. index:: pair: function; optimize
.. _doxid-class_q_panda_1_1_brent_1a0659715752c2f9324f0a739d9c3125db:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void optimize()

execute optimization

.. index:: pair: function; getResult
.. _doxid-class_q_panda_1_1_brent_1a1c86398e34b833da2d1b78e65ca765b8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::pair<double, :ref:`QResultPair<doxid-namespace_q_panda_1a682554b30f0d919b39109220e89e5855>`> getResult()

get result



.. rubric:: Returns:

std::pair<double, QResultPair> result

