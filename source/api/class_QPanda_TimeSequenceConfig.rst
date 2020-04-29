.. index:: pair: class; QPanda::TimeSequenceConfig
.. _doxid-class_q_panda_1_1_time_sequence_config:

class QPanda::TimeSequenceConfig
================================

.. toctree::
	:hidden:

Time Sequence Config.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <XMLConfigParam.h>
	
	class TimeSequenceConfig
	{
	public:
		// methods
	
		static TimeSequenceConfig& :target:`get_instance<doxid-class_q_panda_1_1_time_sequence_config_1ab17afad7cf33c5243f2a5a12bf9ea9d1>`();
		int :target:`get_measure_time_sequence<doxid-class_q_panda_1_1_time_sequence_config_1a3336e93301801a6fac41af2172fb1420>`();
		int :target:`get_ctrl_node_time_sequence<doxid-class_q_panda_1_1_time_sequence_config_1a53ec71115210eeecab1adeaf54354828>`();
		int :target:`get_swap_gate_time_sequence<doxid-class_q_panda_1_1_time_sequence_config_1acf34c15dc6c634969db70cfa079f9b83>`();
		int :target:`get_single_gate_time_sequence<doxid-class_q_panda_1_1_time_sequence_config_1aa66e08fa7f0e686356675590cb17d4b7>`();
		int :target:`get_reset_time_sequence<doxid-class_q_panda_1_1_time_sequence_config_1ab1677f5abbfa9365e101324b96955b2c>`();
	
		template <typename config_type>
		int :target:`read_config<doxid-class_q_panda_1_1_time_sequence_config_1ab044710189c4d523f9d384153cbc92d1>`(
			config_type type_str,
			int val
			);
	};
