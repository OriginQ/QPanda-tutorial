.. index:: pair: class; QPanda::NodeSortProblemGenerator
.. _doxid-class_q_panda_1_1_node_sort_problem_generator:

class QPanda::NodeSortProblemGenerator
======================================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Node Sort Problem Generator. :ref:`More...<details-class_q_panda_1_1_node_sort_problem_generator>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <NodeSortProblemGenerator.h>
	
	class NodeSortProblemGenerator
	{
	public:
		// methods
	
		void :ref:`setProblemGraph<doxid-class_q_panda_1_1_node_sort_problem_generator_1a808a62a4a598d2568279bb9e1eacc8e9>`(const std::vector<std::vector<double>>& graph);
		void :ref:`setLambda1<doxid-class_q_panda_1_1_node_sort_problem_generator_1a27b7738a30950cab4054d8bbce8a9a85>`(double lambda);
		void :ref:`setLambda2<doxid-class_q_panda_1_1_node_sort_problem_generator_1a4f21a0f57a6d2b9472dde68a76412fe8>`(double lambda);
		void :ref:`setLambda3<doxid-class_q_panda_1_1_node_sort_problem_generator_1af76cfc3bcc882e2d180a059e816ef80f>`(double lambda);
		void :ref:`setArbitaryCofficient<doxid-class_q_panda_1_1_node_sort_problem_generator_1a3e70c6100a74d7c732ef9b3f6461a555>`(double arbitary_cofficient);
		void :ref:`exec<doxid-class_q_panda_1_1_node_sort_problem_generator_1a0d33c73f1e0fcc5521439814b5bc1663>`();
		:ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` :ref:`getHamiltonian<doxid-class_q_panda_1_1_node_sort_problem_generator_1ad88fba2da23be638a1a80395df86b84e>`() const;
		std::vector<AnsatzGate> :ref:`getAnsatz<doxid-class_q_panda_1_1_node_sort_problem_generator_1a2876926684bd0433dce3e43666eba698>`() const;
		Eigen::VectorXd :ref:`getLinearSolverResult<doxid-class_q_panda_1_1_node_sort_problem_generator_1a0d6ba7fd91b280202006134f4cd738ea>`() const;
		Eigen::MatrixXd :ref:`getMatrixA<doxid-class_q_panda_1_1_node_sort_problem_generator_1aed66ed7a76ec4c8e0cdf2c3cbf55aa63>`() const;
		Eigen::VectorXd :ref:`getVectorB<doxid-class_q_panda_1_1_node_sort_problem_generator_1ad3d7e7195a3ea4b528ac31a6ef9dd769>`() const;
	};
.. _details-class_q_panda_1_1_node_sort_problem_generator:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Node Sort Problem Generator.

Methods
-------

.. index:: pair: function; setProblemGraph
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1a808a62a4a598d2568279bb9e1eacc8e9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setProblemGraph(const std::vector<std::vector<double>>& graph)

Set problem graph.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- const

		- std::vector<std::vector<double>>& problem graph

.. index:: pair: function; setLambda1
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1a27b7738a30950cab4054d8bbce8a9a85:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLambda1(double lambda)

Set model parameter lamda1.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- lambda

.. index:: pair: function; setLambda2
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1a4f21a0f57a6d2b9472dde68a76412fe8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLambda2(double lambda)

Set model parameter lamda2.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- lambda

.. index:: pair: function; setLambda3
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1af76cfc3bcc882e2d180a059e816ef80f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setLambda3(double lambda)

Set model parameter lamda3.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- lambda

.. index:: pair: function; setArbitaryCofficient
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1a3e70c6100a74d7c732ef9b3f6461a555:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setArbitaryCofficient(double arbitary_cofficient)

Set arbitary cofficient.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- arbitary cofficient

.. index:: pair: function; exec
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1a0d33c73f1e0fcc5521439814b5bc1663:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void exec()

Execute.

.. index:: pair: function; getHamiltonian
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1ad88fba2da23be638a1a80395df86b84e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`PauliOperator<doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>` getHamiltonian() const

Get hamiltonian from the problem model.



.. rubric:: Returns:

PauliOperator hamiltonian



.. rubric:: See also:

:ref:`PauliOperator <doxid-namespace_q_panda_1af5b6b32163d7a2889972112001872916>`

.. index:: pair: function; getAnsatz
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1a2876926684bd0433dce3e43666eba698:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<AnsatzGate> getAnsatz() const

Get ansatz from the problem model.



.. rubric:: Returns:

std::vector<QITE::AnsatzGate> ansatz



.. rubric:: See also:

AnsatzGate

.. index:: pair: function; getLinearSolverResult
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1a0d6ba7fd91b280202006134f4cd738ea:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Eigen::VectorXd getLinearSolverResult() const

Get linear solver result of the problem model.



.. rubric:: Returns:

Eigen::VectorXd linear solver result



.. rubric:: See also:

AnsatzGate

.. index:: pair: function; getMatrixA
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1aed66ed7a76ec4c8e0cdf2c3cbf55aa63:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Eigen::MatrixXd getMatrixA() const

Get the coefficient matrix.



.. rubric:: Returns:

Eigen::MatrixXd parameters of Matirx



.. rubric:: See also:

AnsatzGate

.. index:: pair: function; getVectorB
.. _doxid-class_q_panda_1_1_node_sort_problem_generator_1ad3d7e7195a3ea4b528ac31a6ef9dd769:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	Eigen::VectorXd getVectorB() const

Get the constent term.



.. rubric:: Returns:

Eigen::VectorXd constent term



.. rubric:: See also:

AnsatzGate

