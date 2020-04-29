.. index:: pair: class; QPanda::ClassicalProgFactory
.. _doxid-class_q_panda_1_1_classical_prog_factory:

class QPanda::ClassicalProgFactory
==================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`AbstractClassicalProg <doxid-class_q_panda_1_1_abstract_classical_prog>`. :ref:`More...<details-class_q_panda_1_1_classical_prog_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <ClassicalProgram.h>
	
	class ClassicalProgFactory
	{
	public:
		// methods
	
		void :target:`registClass<doxid-class_q_panda_1_1_classical_prog_factory_1a8e29a2b719ba5e8046a85d583da3bbfe>`(
			std::string name,
			:ref:`CreateClassicalQProgram<doxid-namespace_q_panda_1a8e863438215e55293e6888776d035fed>` method
			);
	
		:ref:`AbstractClassicalProg<doxid-class_q_panda_1_1_abstract_classical_prog>`* :target:`getClassicalProgm<doxid-class_q_panda_1_1_classical_prog_factory_1a365e6cfcb67b4c7c32653784e716e3f9>`(
			std::string& name,
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& classical_cond
			);
	
		static ClassicalProgFactory& :ref:`getInstance<doxid-class_q_panda_1_1_classical_prog_factory_1a26991caaf83f4e3c18a9bbf704735ae1>`();
	};
.. _details-class_q_panda_1_1_classical_prog_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`AbstractClassicalProg <doxid-class_q_panda_1_1_abstract_classical_prog>`.

Methods
-------

.. index:: pair: function; getInstance
.. _doxid-class_q_panda_1_1_classical_prog_factory_1a26991caaf83f4e3c18a9bbf704735ae1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static ClassicalProgFactory& getInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`ClassicalProgFactory <doxid-class_q_panda_1_1_classical_prog_factory>` &

