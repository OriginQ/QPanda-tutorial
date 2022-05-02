.. index:: pair: class; QProgMap
.. _doxid-class_q_prog_map:

class QProgMap
==============

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorNode.h>
	
	class QProgMap
	{
	public:
		// fields
	
		size_t :target:`m_count<doxid-class_q_prog_map_1afddc8870f2f0eb5738c973ca4e8913c0>` {0};

		// construction
	
		:target:`QProgMap<doxid-class_q_prog_map_1a6c60c18bfcfbc36ac5be9d97d646097b>`();
		:target:`QProgMap<doxid-class_q_prog_map_1acddca306433a1d88461911ff6ef82091>`(const QProgMap& old);

		// methods
	
		size_t :target:`getMaxRank<doxid-class_q_prog_map_1abb8942b8ac0155c69fcef66159ea207c>`();
		size_t :target:`setMaxRank<doxid-class_q_prog_map_1a6f07cfbbf94a786d24699b197d250c57>`(size_t rank);
		void :target:`deleteMap<doxid-class_q_prog_map_1a11cdf841ef3dc9c8c1f7b6a6cfe60f05>`();
		QProgMap& :target:`operator =<doxid-class_q_prog_map_1a566e982276977f3ac2151cccd25cf3ad>` (const QProgMap& old);
		:ref:`VerticeMatrix<doxid-class_vertice_matrix>`* :target:`getVerticeMatrix<doxid-class_q_prog_map_1a7e5dee5a1c6bd8f29a7de04cf26f1fb5>`();
		size_t :target:`getQubitVerticeCount<doxid-class_q_prog_map_1a228db5d85334aec30b48b52cd1cb05d6>`(:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` qubit_num);
		void :target:`setQubitNum<doxid-class_q_prog_map_1abfd8869c6b4be76fcbaece38145fa310>`(size_t num);
		bool :target:`isEmptyQProg<doxid-class_q_prog_map_1a404e6854f5ded5f7e5aa5ed2ee741a86>`();
		size_t :target:`getQubitNum<doxid-class_q_prog_map_1a2d7436b6e9b565db939620ca90409e32>`();
		:ref:`edge_map_t<doxid-_tensor_node_8h_1aa2ec0dbc2b2371ca27fda6883430e1d5>`* :target:`getEdgeMap<doxid-class_q_prog_map_1aeba6ecc00ff928ea12856611b0a605bf>`();
		void :target:`clearVerticeValue<doxid-class_q_prog_map_1ad2f4bf6c5a1518414774040b9c1ed3c1>`();
		void :target:`clear<doxid-class_q_prog_map_1a993777ff8b9e65a780a8479f52f47b9a>`();
		:ref:`qsize_t<doxid-_tensor_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getVerticeCount<doxid-class_q_prog_map_1a2b636db673ca4949b8b3dca346d023d0>`() const;
	};
