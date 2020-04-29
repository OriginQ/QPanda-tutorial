.. index:: pair: class; QuantumProgMap
.. _doxid-class_quantum_prog_map:

class QuantumProgMap
====================

.. toctree::
	:hidden:




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <TensorNode.h>
	
	class QuantumProgMap
	{
	public:
		// construction
	
		:target:`QuantumProgMap<doxid-class_quantum_prog_map_1a75df81dd19572c418860e2a2218b6f6a>`();
		:target:`QuantumProgMap<doxid-class_quantum_prog_map_1aa46f03ce13c87428615ba8b066e4ade0>`(const QuantumProgMap& old);

		// methods
	
		:ref:`VerticeMatrix<doxid-class_vertice_matrix>`* :target:`getVerticeMatrix<doxid-class_quantum_prog_map_1a4ce3fa38f982164dc243f596228d97ef>`();
		void :target:`setQubitNum<doxid-class_quantum_prog_map_1aa81c00e5476e3ef5fc98c731489e70c6>`(size_t num);
		bool :target:`isEmptyQProg<doxid-class_quantum_prog_map_1a0a83b0c56e1f8a9e75cd7a38488e6704>`();
		size_t :target:`getQubitNum<doxid-class_quantum_prog_map_1ac251336bd85bbbc7df3ca870d6329ef9>`();
		:ref:`EdgeMap<doxid-_tensor_node_8h_1a6ae5033ce14f4186e6c7063d177d75e2>`* :target:`getEdgeMap<doxid-class_quantum_prog_map_1acc25a2fcacfe00d1aa07a58dbfac4dd5>`();
		void :target:`clearVerticeValue<doxid-class_quantum_prog_map_1a0bc776b663007084204c235ec8f66e0d>`();
		void :target:`clear<doxid-class_quantum_prog_map_1ac32d15ce38616ea7f06dc255b4284587>`();
		:ref:`qsize_t<doxid-_tensor_node_8h_1a9695bf30eeb2fa028ee7c75690380572>` :target:`getVerticeCount<doxid-class_quantum_prog_map_1ae9e6a0ea659ceb2ffd92f6a523fd176f>`() const;
	};
