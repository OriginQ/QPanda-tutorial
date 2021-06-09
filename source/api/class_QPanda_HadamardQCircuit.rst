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
	
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1aab8aacb324825696cf2c7735b8ce17bc>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1af035a5d190751faeea05132aefe1d6c6>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1ad2f723e4ab1bfbb499226d0a6939bd18>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_abstract_node_manager_1abffeb4cc2327ec65520da3b127999393>`() = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_abstract_node_manager_1a9b5dc4a55201cd684f010f60835dd40d>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_abstract_node_manager_1a1aab80e3d5b0a1dab7f0804458c6628e>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&) = 0;
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_abstract_node_manager_1ae4b5be219a36fc04e671f00dfe3b6b11>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>) = 0;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a9901ebf6ad22292cba7f9911ec3b600f>`() const = 0;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ac4e834af252b8cefb1a9de6ae8781a7d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) = 0;
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad25e733d7f1a6bb837ca764135db1c8b>`(bool isDagger) = 0;
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a0d810051304b282991d6fd1b87bb437d>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`) = 0;
		virtual void :ref:`clearControl<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a3e61c68f5be51f3716506b42e6cf2359>`() = 0;
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_abstract_quantum_circuit_1a5b7386321461dff5dcee0ae6dcd4812a>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const = 0;
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_abstract_quantum_circuit_1ad054a6feb7cca5f960df1420f0b9a629>`() = 0;
		std::shared_ptr<:ref:`AbstractQuantumCircuit<doxid-class_q_panda_1_1_abstract_quantum_circuit>`> :ref:`getImplementationPtr<doxid-class_q_panda_1_1_q_circuit_1a305f41c1b523203e43b01fe42df5c7c1>`();
		virtual void :ref:`pushBackNode<doxid-class_q_panda_1_1_q_circuit_1afee8bb25ac24c51e4c37c5d957139713>`(std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
	
		template <typename T>
		:ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>`& :ref:`operator <<<doxid-class_q_panda_1_1_q_circuit_1a0bfc0cbf8c6e7d8364c7b1c286ff2952>` (:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` node);
	
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`dagger<doxid-class_q_panda_1_1_q_circuit_1ab3c4c560b2b45b89469a00b38ddbebe9>`();
		virtual :ref:`QCircuit<doxid-class_q_panda_1_1_q_circuit>` :ref:`control<doxid-class_q_panda_1_1_q_circuit_1a895b9bbb1b6c9bf825436dd8b3d69aa5>`(const QVec);
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_circuit_1ab3a37b3d981285ad7127eedbb9e0c6b5>`() const;
		virtual bool :ref:`isDagger<doxid-class_q_panda_1_1_q_circuit_1aa09cf54785a8c09befeddf5eff6bc4cc>`() const;
		virtual bool :ref:`getControlVector<doxid-class_q_panda_1_1_q_circuit_1a56414aa73904b6ec9433297a62187101>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getFirstNodeIter<doxid-class_q_panda_1_1_q_circuit_1aa469d1cffaf63059e04c3e1dde9d5c1b>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getLastNodeIter<doxid-class_q_panda_1_1_q_circuit_1ad69ffc60fb639ac326e68a72ae26aed9>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getEndNodeIter<doxid-class_q_panda_1_1_q_circuit_1aaa07e04eb4206ec2f22288263ff4e868>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`getHeadNodeIter<doxid-class_q_panda_1_1_q_circuit_1a57f22108948500db0b56032ceb39a720>`();
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`insertQNode<doxid-class_q_panda_1_1_q_circuit_1a3bca05ba8250155feacfa03d01b56e8b>`(const :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&, std::shared_ptr<:ref:`QNode<doxid-class_q_panda_1_1_q_node>`>);
		virtual :ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>` :ref:`deleteQNode<doxid-class_q_panda_1_1_q_circuit_1abaca2f9009304097977ab01e5f935009>`(:ref:`NodeIter<doxid-class_q_panda_1_1_node_iter>`&);
		bool :ref:`is_empty<doxid-class_q_panda_1_1_q_circuit_1a2d4ece37b1a27194521d80d569704c65>`();
		virtual void :ref:`setDagger<doxid-class_q_panda_1_1_q_circuit_1a40036d789e82cbf24f711674a825e7c6>`(bool isDagger);
		virtual void :ref:`setControl<doxid-class_q_panda_1_1_q_circuit_1a0217be0bb49add047fdc6f43e40909bb>`(const QVec);
		virtual size_t :ref:`get_used_qubits<doxid-class_q_panda_1_1_q_circuit_1adba3dfe84e87dbbd3303cc545cb96219>`(:ref:`QVec<doxid-class_q_panda_1_1_q_vec>`&) const;
		virtual size_t :ref:`get_qgate_num<doxid-class_q_panda_1_1_q_circuit_1a5d63e1573c3f5d55064a0f9714a8b545>`();

