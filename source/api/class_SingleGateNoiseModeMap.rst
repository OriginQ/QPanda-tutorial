.. index:: pair: class; SingleGateNoiseModeMap
.. _doxid-class_single_gate_noise_mode_map:

class SingleGateNoiseModeMap
============================

.. toctree::
	:hidden:

Single gate noise mode map.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NoiseModel.h>
	
	class SingleGateNoiseModeMap
	{
	public:
		// methods
	
		static SingleGateNoiseModeMap& :target:`getInstance<doxid-class_single_gate_noise_mode_map_1aa0bfba32404bf8e6219bb517d961daa0>`();
		:ref:`noise_mode_function<doxid-_noise_model_8h_1a23eefdad48b57ed970997f0938dcc4e3>` :target:`operator []<doxid-class_single_gate_noise_mode_map_1a5c56dd419f23c54603358a14ebeee757>` (:ref:`NOISE_MODEL<doxid-_noise_model_8h_1a4e433c5ef943716bf3d7b430a596f8a0>`);
	};
