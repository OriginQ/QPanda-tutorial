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
	
		static void :target:`split<doxid-class_tensor_engine_1a3219a318563162ae44452302dd82613d>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map,
			:ref:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`& qubit_vertice
			);
	
		static :ref:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>` :target:`getNoValueVertice<doxid-class_tensor_engine_1a102947d28c93520bda0baedb5c987f7f>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map,
			size_t contect_edge
			);
	
		static :ref:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>` :target:`getNoValueAndContectEdgeMaxVertice<doxid-class_tensor_engine_1a78b1cbd0816ab3d36fe1ea7628081d60>`(:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map);
	
		static :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` :target:`Merge<doxid-class_tensor_engine_1a325a7be8487a0cade7431d049d77f492>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map,
			const :ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`& sequence
			);
	
		static :ref:`qcomplex_data_t<doxid-_tensor_8h_1a4cadf8bed635e0bf84c11804444d3151>` :target:`computing<doxid-class_tensor_engine_1a88a6adbd315ae0ce9bf1fa18aae80fba>`(:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map);
	
		static std::map<:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>`, :ref:`Vertice<doxid-class_vertice>`>::iterator :target:`MergeQuantumProgMap<doxid-class_tensor_engine_1a5a18c3e23459b254d0b99051040cb7d9>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`&,
			:ref:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`&,
			bool& is_success
			);
	
		static void :target:`MergeByVerticeVector<doxid-class_tensor_engine_1ad92e3350bd2d9e40effcee9bf242309a>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`&,
			:ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`& sequence
			);
	
		static void :target:`dimDecrementbyValue<doxid-class_tensor_engine_1a57cfa04deb11300f84e267ec3d9c208e>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`&,
			:ref:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`&,
			int value
			);
	
		static void :target:`dimDecrementbyValueAndNum<doxid-class_tensor_engine_1a33711f009cedde40af202eed7a3d92d8>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`&,
			:ref:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>`&,
			int value
			);
	
		static void :target:`getVerticeMap<doxid-class_tensor_engine_1a3721eec9888c4eff2de2dfef468bf4f5>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`&,
			std::vector<std::pair<size_t, size_t>>&
			);
	
		static size_t :target:`getMaxRank<doxid-class_tensor_engine_1a5f256833d7ce918eb26b05c09013db14>`(:ref:`QProgMap<doxid-class_q_prog_map>`&);
		static :ref:`qubit_vertice_t<doxid-_tensor_node_8h_1a7a7a3d1a9a71fab5e9a866e96a30cffa>` :target:`getMaxQubitVertice<doxid-class_tensor_engine_1a11e9430d450198b7e5a9b1ff7d6bb075>`(:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map);
	
		static void :target:`seq_merge_by_vertices<doxid-class_tensor_engine_1aec0628ef11e070c43328f12f817e0230>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map,
			std::vector<size_t> vertice_vector,
			:ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`& sequence
			);
	
		static void :target:`seq_merge<doxid-class_tensor_engine_1a03035af2d4ffa49e1b21db862ff16a4d>`(
			:ref:`QProgMap<doxid-class_q_prog_map>`& prog_map,
			:ref:`qprog_sequence_t<doxid-_tensor_engine_8h_1ab1fd320f4cc67d35c6c2d2b6b23c39ec>`& vertice_vector
			);
	};
