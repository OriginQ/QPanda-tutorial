.. index:: pair: class; QPanda::QResultFactory
.. _doxid-class_q_panda_1_1_q_result_factory:

class QPanda::QResultFactory
============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Factory for class :ref:`QResult <doxid-class_q_panda_1_1_q_result>`. :ref:`More...<details-class_q_panda_1_1_q_result_factory>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QResultFactory.h>
	
	class QResultFactory
	{
	public:
		// typedefs
	
		typedef std::function<:ref:`QResult<doxid-class_q_panda_1_1_q_result>`*()> :target:`constructor_t<doxid-class_q_panda_1_1_q_result_factory_1a55d4101b537f9ae90ac31d13c803446e>`;
		typedef std::map<std::string, :ref:`constructor_t<doxid-class_q_panda_1_1_q_result_factory_1a55d4101b537f9ae90ac31d13c803446e>`> :target:`constructor_Map_t<doxid-class_q_panda_1_1_q_result_factory_1a6564a647f2141afee3b87b1c16db5b86>`;

		// fields
	
		:ref:`constructor_Map_t<doxid-class_q_panda_1_1_q_result_factory_1a6564a647f2141afee3b87b1c16db5b86>` :target:`_QResult_Constructor<doxid-class_q_panda_1_1_q_result_factory_1a0f82ceb00ce9bf47c399204c5840d996>`;

		// methods
	
		:ref:`QResult<doxid-class_q_panda_1_1_q_result>`* :target:`GetEmptyQResult<doxid-class_q_panda_1_1_q_result_factory_1a8702e5d77a1d43f70a68a350aa9cbacd>`();
	
		void :target:`registerclass<doxid-class_q_panda_1_1_q_result_factory_1a8dcabe5141f4e98b432bf9839e7fb354>`(
			std::string&,
			:ref:`constructor_t<doxid-class_q_panda_1_1_q_result_factory_1a55d4101b537f9ae90ac31d13c803446e>`
			);
	
		static QResultFactory& :ref:`GetFactoryInstance<doxid-class_q_panda_1_1_q_result_factory_1aace8423fdf154bc1fcddee3dfbe3ef96>`();
	};
.. _details-class_q_panda_1_1_q_result_factory:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Factory for class :ref:`QResult <doxid-class_q_panda_1_1_q_result>`.

Methods
-------

.. index:: pair: function; GetFactoryInstance
.. _doxid-class_q_panda_1_1_q_result_factory_1aace8423fdf154bc1fcddee3dfbe3ef96:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static QResultFactory& GetFactoryInstance()

Get the static instance of factory.



.. rubric:: Returns:

:ref:`QResultFactory <doxid-class_q_panda_1_1_q_result_factory>` &

