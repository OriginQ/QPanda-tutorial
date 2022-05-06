.. index:: pair: class; QuickBB
.. _doxid-class_quick_b_b:

class QuickBB
=============

.. toctree::
	:hidden:

	class_QuickBB_Graph.rst

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuickBB.h>
	
	class QuickBB
	{
	public:
		// classes
	
		class :ref:`Graph<doxid-class_quick_b_b_1_1_graph>`;

		// methods
	
		static std::pair<size_t, :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`> :ref:`compute<doxid-class_quick_b_b_1a1fc5874accc182f993ddfb82e3571f35>`(:ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph, size_t alloted_time);
	
		static std::pair<size_t, :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`> :ref:`compute<doxid-class_quick_b_b_1af9726818e17ad373c392f084b538c46f>`(
			const std::vector<std::pair<size_t, size_t>>& vertice_vect,
			size_t alloted_time
			);
	
		static void :target:`make_clique<doxid-class_quick_b_b_1aea9471cec143c25689c950750a6bb229>`(
			:ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph,
			const :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`& vertices
			);
	
		static bool :target:`is_clique<doxid-class_quick_b_b_1a4509490431432e1392d112cd42bc9066>`(
			const :ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph,
			const :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`& vertices
			);
	
		static bool :target:`simplicial<doxid-class_quick_b_b_1a5ed9884d01db55f7224921149dc24c9a>`(
			const :ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph,
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` vertex
			);
	
		static bool :target:`almost_simplicial<doxid-class_quick_b_b_1adac41b74b21626adb0482dc9193f3b32>`(
			const :ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph,
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` vertex
			);
	
		static void :target:`eliminate<doxid-class_quick_b_b_1a2e5669de0a90ec653fb339d375962f67>`(
			:ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph,
			:ref:`vertex_index_t<doxid-_quick_b_b_8h_1a4c64fe2c1542d68195dfae3b74316c2b>` vertex
			);
	
		static size_t :target:`count_fillin<doxid-class_quick_b_b_1a51a8f81c2643afb87f1d5e63c02550ab>`(
			const :ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph,
			:ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>` vertices
			);
	
		static std::pair<:ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`, size_t> :target:`upper_bound<doxid-class_quick_b_b_1ae7f8ed1cf51550cc306013716a9292f5>`(const :ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph);
		static size_t :target:`lower_bound<doxid-class_quick_b_b_1a239b24c90c8e5643e8a607bf29e2dfee>`(const :ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph);
	};
.. _details-class_quick_b_b:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Methods
-------

.. index:: pair: function; compute
.. _doxid-class_quick_b_b_1a1fc5874accc182f993ddfb82e3571f35:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::pair<size_t, :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`> compute(:ref:`Graph<doxid-class_quick_b_b_1_1_graph>`& graph, size_t alloted_time)

compute the optimal order



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- :ref:`Graph <doxid-class_quick_b_b_1_1_graph>`

		- :ref:`QuickBB <doxid-class_quick_b_b>` graph

	*
		- size_t

		- alloted compute time



.. rubric:: Returns:

std::pair<size_t, adj_arr_t> first : tree width , second : order

.. index:: pair: function; compute
.. _doxid-class_quick_b_b_1af9726818e17ad373c392f084b538c46f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::pair<size_t, :ref:`adj_arr_t<doxid-_quick_b_b_8h_1a2ee0029834ebe914c20b78588d15cac6>`> compute(
		const std::vector<std::pair<size_t, size_t>>& vertice_vect,
		size_t alloted_time
		)

compute the optimal order



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::vector<std::pair<size_t

		- 

	*
		- size_t>>

		- :ref:`QuickBB <doxid-class_quick_b_b>` graph

	*
		- size_t

		- alloted compute time



.. rubric:: Returns:

std::pair<size_t, adj_arr_t> first : tree width , second : order

