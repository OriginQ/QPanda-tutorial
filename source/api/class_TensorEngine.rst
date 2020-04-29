.. index:: pair: class; TensorEngine
.. _doxid-class_tensor_engine:

class TensorEngine
==================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorEngine.h>
	
	class TensorEngine
	{
	public:
		// methods
	
		static :ref:`qubit_vertice_t<doxid-_tensor_engine_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>` :target:`getNoValueVertice<doxid-class_tensor_engine_1afb7d6bcdc5e8b883b5765622af8b01ee>`(
			:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
			size_t contect_edge
			);
	
		static :ref:`qubit_vertice_t<doxid-_tensor_engine_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>` :target:`getNoValueAndContectEdgeMaxVertice<doxid-class_tensor_engine_1a79a0b1a557262d13f08e82f25d31eca4>`(:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map);
		static void :target:`Merge<doxid-class_tensor_engine_1a86171896f6b0f6370096693167315c2c>`(:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map);
	
		static :ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>` :target:`Merge<doxid-class_tensor_engine_1a7e538230928b53ba585cd01056b4e2e3>`(
			:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map,
			:ref:`qubit_vertice_t<doxid-_tensor_engine_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`*
			);
	
		static :ref:`qcomplex_data_t<doxid-_tensor_node_8h_1a4d2a0644088f58f60fb50a9113074a99>` :target:`computing<doxid-class_tensor_engine_1a668a0fe72d37f7667ce3b15c5be8cf55>`(:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`& prog_map);
	
		static map<:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`Vertice<doxid-class_vertice>`>::iterator :target:`MergeQuantumProgMap<doxid-class_tensor_engine_1a4e9b77ec1f457fa531d982c8fdf0e9aa>`(
			:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`&,
			:ref:`qubit_vertice_t<doxid-_tensor_engine_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`&
			);
	
		static void :target:`dimDecrementbyValue<doxid-class_tensor_engine_1a267ff756e1c9c5a621524cec0e0716c8>`(
			:ref:`QuantumProgMap<doxid-class_quantum_prog_map>`&,
			:ref:`qubit_vertice_t<doxid-_tensor_engine_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`&,
			int value
			);
	};
