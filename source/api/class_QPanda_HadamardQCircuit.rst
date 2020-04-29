.. index:: pair: class; QPanda::HadamardQCircuit
.. _doxid-class_q_panda_1_1_hadamard_q_circuit:

class QPanda::HadamardQCircuit
==============================

.. toctree::
	:hidden:

Hadamard quantum circuit program.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QCircuit.h>
	
	class HadamardQCircuit: public :ref:`QPanda::QCircuit<doxid-class_q_panda_1_1_q_circuit>`
	{
	public:
		// construction
	
		:target:`HadamardQCircuit<doxid-class_q_panda_1_1_hadamard_q_circuit_1ab72b9c13d464d2ddb32fb63ab8966d5d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`& pQubitVector);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad13a60e0771b9bf6a984aff13967c15e>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0c958083867fb03f0606ccc74ed13800>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a4732224c13dc949d2ed26388138dd0d3>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_abstract_quantum_circuit_1af6f1864ea355c13eaa4e14bddf64934c>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_abstract_quantum_circuit_1aeabd63772ee53de4c41141b7afef6d5f>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_abstract_quantum_circuit_1aded25dd1af1558f04d6ad72736ab2ce9>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&) = 0;
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a99f9d60e21e0e4d49c64e3253ff03001>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a9901ebf6ad22292cba7f9911ec3b600f>`() const = 0;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ac4e834af252b8cefb1a9de6ae8781a7d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad25e733d7f1a6bb837ca764135db1c8b>`(bool isDagger) = 0;
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0d810051304b282991d6fd1b87bb437d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0;
		virtual void :ref:`clearControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a3e61c68f5be51f3716506b42e6cf2359>`() = 0;
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> :ref:`getImplementationPtr<doxid-class_q_panda_1_1_q_circuit_1a305f41c1b523203e43b01fe42df5c7c1>`();
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_q_circuit_1afee8bb25ac24c51e4c37c5d957139713>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
	
		template <typename T>
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& :ref:`operator <<<doxid-class_q_panda_1_1_q_circuit_1a0bfc0cbf8c6e7d8364c7b1c286ff2952>` (:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` node);
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`dagger<doxid-class_q_panda_1_1_q_circuit_1ab3c4c560b2b45b89469a00b38ddbebe9>`();
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`control<doxid-class_q_panda_1_1_q_circuit_1a686e7f335e37faa5da17005856a6356b>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_circuit_1ab3a37b3d981285ad7127eedbb9e0c6b5>`() const;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_q_circuit_1aa09cf54785a8c09befeddf5eff6bc4cc>`() const;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_q_circuit_1a56414aa73904b6ec9433297a62187101>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_q_circuit_1aa469d1cffaf63059e04c3e1dde9d5c1b>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_q_circuit_1ad69ffc60fb639ac326e68a72ae26aed9>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_q_circuit_1aaa07e04eb4206ec2f22288263ff4e868>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_q_circuit_1a57f22108948500db0b56032ceb39a720>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_q_circuit_1a101b00b026129a0de08542dff60c305a>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_q_circuit_1abaca2f9009304097977ab01e5f935009>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&);
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_q_circuit_1a40036d789e82cbf24f711674a825e7c6>`(bool isDagger);
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_q_circuit_1afa5b3b8c7aa6ed8d424521df3a02b3b7>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`);

