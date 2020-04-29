.. index:: pair: class; QPanda::TraversalConfig
.. _doxid-class_q_panda_1_1_traversal_config:

class QPanda::TraversalConfig
=============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

traversal config :ref:`More...<details-class_q_panda_1_1_traversal_config>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Traversal.h>
	
	class TraversalConfig
	{
	public:
		// fields
	
		size_t :ref:`m_qubit_number<doxid-class_q_panda_1_1_traversal_config_1a7aeaf1a66ae4261814e6adc85bc68923>`;
		std::map<std::string, bool> :ref:`m_return_value<doxid-class_q_panda_1_1_traversal_config_1af77872e3296a453c0817ec99f4d7d92f>`;
		bool :target:`m_is_dagger<doxid-class_q_panda_1_1_traversal_config_1a86672e068eae3a91fcd0173666dea174>`;
		std::vector<:ref:`QPanda::Qubit<doxid-class_q_panda_1_1_qubit>`*> :target:`m_control_qubit_vector<doxid-class_q_panda_1_1_traversal_config_1a8bc36425897348ddb2a6a2d1df096c97>`;
	};
.. _details-class_q_panda_1_1_traversal_config:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

traversal config

Fields
------

.. index:: pair: variable; m_qubit_number
.. _doxid-class_q_panda_1_1_traversal_config_1a7aeaf1a66ae4261814e6adc85bc68923:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	size_t m_qubit_number

quantum bit number

.. index:: pair: variable; m_return_value
.. _doxid-class_q_panda_1_1_traversal_config_1af77872e3296a453c0817ec99f4d7d92f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::map<std::string, bool> m_return_value

MonteCarlo result

