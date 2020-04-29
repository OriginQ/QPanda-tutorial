.. index:: pair: group; MaxCutProblemGenerator
.. _doxid-group___max_cut_problem_generator:

MaxCutProblemGenerator
======================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	// global functions

	double :ref:`QPanda::vector_dot<doxid-group___max_cut_problem_generator_1gaabca13165ac231f4d1432a127051fcae>`(std::vector<double>& x, std::vector<double>& y);

	double :ref:`QPanda::all_cut_of_graph<doxid-group___max_cut_problem_generator_1ga86d1510c5d9a68fa500efc1a696749e4>`(
		std::vector<std::vector<double>> adjacent_matrix,
		std::vector<double>& all_cut_list,
		std::vector<size_t>& target_value_list
		);

.. _details-group___max_cut_problem_generator:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. index:: pair: function; vector_dot
.. _doxid-group___max_cut_problem_generator_1gaabca13165ac231f4d1432a127051fcae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	double QPanda::vector_dot(std::vector<double>& x, std::vector<double>& y)

vector dot product



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<double>&

		- vector x, x will be clear

	*
		- std::vector<double>&

		- vector y, y will be clear



.. rubric:: Returns:

double the dot product result of the two input vectors

.. index:: pair: function; all_cut_of_graph
.. _doxid-group___max_cut_problem_generator_1ga86d1510c5d9a68fa500efc1a696749e4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	double QPanda::all_cut_of_graph(
		std::vector<std::vector<double>> adjacent_matrix,
		std::vector<double>& all_cut_list,
		std::vector<size_t>& target_value_list
		)

all cut of graph



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<std::vector<double>>

		- the adjacent matrix

	*
		- std::vector<double>&

		- all cut list

	*
		- std::vector<size_t>&

		- target value list



.. rubric:: Returns:

double the max cut value

