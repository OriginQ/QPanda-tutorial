.. index:: pair: class; QPanda::OriginMeasure
.. _doxid-class_q_panda_1_1_origin_measure:

class QPanda::OriginMeasure
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Qrigin quantum measure basic class. :ref:`More...<details-class_q_panda_1_1_origin_measure>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QuantumMeasure.h>
	
	class OriginMeasure:
	    public :ref:`QPanda::QNode<doxid-class_q_panda_1_1_q_node>`,
	    public :ref:`QPanda::AbstractQuantumMeasure<doxid-class_q_panda_1_1_abstract_quantum_measure>`
	{
	public:
		// construction
	
		:target:`OriginMeasure<doxid-class_q_panda_1_1_origin_measure_1a411010903a03ccdbc598d498d9f0132e>`(
			:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*,
			:ref:`CBit<doxid-class_q_panda_1_1_c_bit>`*
			);

		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_origin_measure_1a9ab73da73866b817a7501d47ebbfbff4>`() const;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_origin_measure_1a99b51e4698a03e575adb0409562ea9ba>`() const;
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_origin_measure_1a2d7ced771a83d22f723f60b8d4573819>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_node_1a8e8793fe1aabcd13db3ed1f79892c011>`() const = 0;
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_abstract_quantum_measure_1ae377dd6d809e3c4c97fa6ec1fab23513>`() const = 0;
		virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* :ref:`getCBit<doxid-class_q_panda_1_1_abstract_quantum_measure_1ab08d02223fc2440ff809ff277857f74b>`() const = 0;

.. _details-class_q_panda_1_1_origin_measure:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Qrigin quantum measure basic class.

Methods
-------

.. index:: pair: function; getQuBit
.. _doxid-class_q_panda_1_1_origin_measure_1a9ab73da73866b817a7501d47ebbfbff4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* getQuBit() const

Get measure node qubit address.



.. rubric:: Returns:

:ref:`QPanda::Qubit <doxid-class_q_panda_1_1_qubit>` \* QuBit address

.. index:: pair: function; getCBit
.. _doxid-class_q_panda_1_1_origin_measure_1a99b51e4698a03e575adb0409562ea9ba:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`CBit<doxid-class_q_panda_1_1_c_bit>`* getCBit() const

Get measure node cbit address.



.. rubric:: Returns:

:ref:`QPanda::CBit <doxid-class_q_panda_1_1_c_bit>` \* cBit address

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_origin_measure_1a2d7ced771a83d22f723f60b8d4573819:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

