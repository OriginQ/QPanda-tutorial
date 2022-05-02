.. index:: pair: class; QPanda::QCircuitGenerator
.. _doxid-class_q_panda_1_1_q_circuit_generator:

class QPanda::QCircuitGenerator
===============================

.. toctree::
	:hidden:

	struct_QPanda_QCircuitGenerator_CircuitNode.rst




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuitGenerator.h>
	
	class QCircuitGenerator
	{
	public:
		// typedefs
	
		typedef std::shared_ptr<QCircuitGenerator::CircuitNode> :target:`CircuitNodeRef<doxid-class_q_panda_1_1_q_circuit_generator_1a536a691e60d73fbc7d1365eb79c9dcba>`;
		typedef std::shared_ptr<QCircuitGenerator> :target:`Ref<doxid-class_q_panda_1_1_q_circuit_generator_1a27882a6e598c32bafffa9ea630a31d32>`;

		// structs
	
		struct :ref:`CircuitNode<doxid-struct_q_panda_1_1_q_circuit_generator_1_1_circuit_node>`;

		// methods
	
		void :target:`set_param<doxid-class_q_panda_1_1_q_circuit_generator_1a64717752dd518e9614991079e1b28f69>`(
			const :ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& qubits,
			const std::vector<double>& angle
			);
	
		:ref:`CircuitNodeRef<doxid-class_q_panda_1_1_q_circuit_generator_1a536a691e60d73fbc7d1365eb79c9dcba>` :target:`build_cir_node<doxid-class_q_panda_1_1_q_circuit_generator_1a94a914cb792b0203cd52bb8d8f7bdd26>`(
			std::string op,
			const std::vector<uint32_t>& target_q,
			const std::vector<std::string>& angle = {},
			const std::vector<uint32_t>& control_q = {},
			bool is_dagger = false
			);
	
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :target:`get_cir<doxid-class_q_panda_1_1_q_circuit_generator_1a8d7e23d9661f46bbdc8c54374445c2b0>`();
		void :target:`append_cir_node<doxid-class_q_panda_1_1_q_circuit_generator_1afae33fa7e7d3ecf6206249b15cb8644c>`(:ref:`CircuitNodeRef<doxid-class_q_panda_1_1_q_circuit_generator_1a536a691e60d73fbc7d1365eb79c9dcba>` node);
	
		void :target:`append_cir_node<doxid-class_q_panda_1_1_q_circuit_generator_1a2eab76e8aa9cec513606c9732ad3eb9e>`(
			std::string op,
			const std::vector<uint32_t>& target_q,
			const std::vector<std::string>& angle = {},
			const std::vector<uint32_t>& control_q = {},
			bool is_dagger = false
			);
	
		const std::vector<:ref:`CircuitNodeRef<doxid-class_q_panda_1_1_q_circuit_generator_1a536a691e60d73fbc7d1365eb79c9dcba>`>& :target:`get_cir_node_vec<doxid-class_q_panda_1_1_q_circuit_generator_1a64c513b79044e89a8adb006219141887>`() const;
		uint32_t :target:`get_circuit_width<doxid-class_q_panda_1_1_q_circuit_generator_1a9c26b16ce0ae20ac0636c1957998582f>`();
		void :target:`set_circuit_width<doxid-class_q_panda_1_1_q_circuit_generator_1a7111c3146c3052881ef0b585e0552613>`(uint32_t w);
	};
