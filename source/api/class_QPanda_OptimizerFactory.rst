.. index:: pair: class; QPanda::OptimizerFactory
.. _doxid-class_q_panda_1_1_optimizer_factory:

class QPanda::OptimizerFactory
==============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Class of Optimizer factory. :ref:`More...<details-class_q_panda_1_1_optimizer_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OptimizerFactory.h>
	
	class OptimizerFactory
	{
	public:
		// methods
	
		static std::unique_ptr<:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`> :ref:`makeOptimizer<doxid-class_q_panda_1_1_optimizer_factory_1ae3619b2000d6e06a463cfb084a6edd3c>`(const :ref:`OptimizerType<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>`& optimizer);
		static std::unique_ptr<:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`> :ref:`makeOptimizer<doxid-class_q_panda_1_1_optimizer_factory_1a59140b212692fc73a39010d7e51c1c54>`(const std::string& optimizer);
	};
.. _details-class_q_panda_1_1_optimizer_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Class of Optimizer factory.

Methods
-------

.. index:: pair: function; makeOptimizer
.. _doxid-class_q_panda_1_1_optimizer_factory_1ae3619b2000d6e06a463cfb084a6edd3c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::unique_ptr<:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`> makeOptimizer(const :ref:`OptimizerType<doxid-namespace_q_panda_1ad1be07c72805502c7d002a53b303bd1e>`& optimizer)

create a Optimizer object by OptimizerType



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- OptimizerType

		- Optimizer Type



.. rubric:: Returns:

std::unique_ptr<AbstractOptimizer>

.. index:: pair: function; makeOptimizer
.. _doxid-class_q_panda_1_1_optimizer_factory_1a59140b212692fc73a39010d7e51c1c54:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::unique_ptr<:ref:`AbstractOptimizer<doxid-class_q_panda_1_1_abstract_optimizer>`> makeOptimizer(const std::string& optimizer)

create a Optimizer object by OptimizerType string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- Optimizer Type string



.. rubric:: Returns:

std::unique_ptr<AbstractOptimizer>

