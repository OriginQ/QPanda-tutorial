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
		double :target:`m_rotation_angle_error<doxid-class_q_panda_1_1_traversal_config_1a91ccdf594763fe2eb33eed77ea17ba86>` { 0 };
		bool :target:`m_can_optimize_measure<doxid-class_q_panda_1_1_traversal_config_1ab832bbcbd90ed32200effb4c2abc924d>` = true;
		std::vector<size_t> :target:`m_measure_qubits<doxid-class_q_panda_1_1_traversal_config_1ad789db57bdb944cd78c5a741f925429a>`;
		std::vector<:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*> :target:`m_measure_cc<doxid-class_q_panda_1_1_traversal_config_1aab4ee007994eb04ddf6afa126ed65920>`;

		// construction
	
		:target:`TraversalConfig<doxid-class_q_panda_1_1_traversal_config_1a573f5b6e7e15dd85c02b1f147dbca0a5>`(double rotation_angle_error = 0);
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

