.. index:: pair: class; QPanda::QubitReference
.. _doxid-class_q_panda_1_1_qubit_reference:

class QPanda::QubitReference
============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

The position of the qubit is an expression. :ref:`More...<details-class_q_panda_1_1_qubit_reference>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QubitReference.h>
	
	class QubitReference:
	    public :ref:`QPanda::Qubit<doxid-class_q_panda_1_1_qubit>`,
	    public :ref:`QPanda::QubitReferenceInterface<doxid-class_q_panda_1_1_qubit_reference_interface>`
	{
	public:
		// construction
	
		:target:`QubitReference<doxid-class_q_panda_1_1_qubit_reference_1a917b281a727948976f03a8862a99e4a9>`(
			:ref:`ClassicalCondition<doxid-class_q_panda_1_1_classical_condition>`& cc,
			std::vector<:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*> qvec
			);
	
		:target:`QubitReference<doxid-class_q_panda_1_1_qubit_reference_1a43c19299d78d3a3dc4bf5610e23c9b3a>`(const QubitReference& old);

		// methods
	
		virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* :ref:`getPhysicalQubitPtr<doxid-class_q_panda_1_1_qubit_reference_1ac52025ebf1860482ecf8e47d932c526b>`();
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_qubit_reference_1a7eed27269ff858ef49e6a1a2d2162833>`();
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :target:`getExprPtr<doxid-class_q_panda_1_1_qubit_reference_1ad106c44aafb7d5be0497d7ed585d3ef0>`();
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* :ref:`getPhysicalQubitPtr<doxid-class_q_panda_1_1_qubit_1a05b7dd4dcfe023c3f341fc8d09d90943>`() = 0;
		virtual bool :ref:`getOccupancy<doxid-class_q_panda_1_1_qubit_1a50abaaae859256175922cae0e07ea9f6>`() = 0;
		virtual std::shared_ptr<:ref:`CExpr<doxid-class_q_panda_1_1_c_expr>`> :ref:`getExprPtr<doxid-class_q_panda_1_1_qubit_reference_interface_1ae5b90745e942726dfe3d875601265141>`() = 0;

.. _details-class_q_panda_1_1_qubit_reference:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

The position of the qubit is an expression.

Methods
-------

.. index:: pair: function; getPhysicalQubitPtr
.. _doxid-class_q_panda_1_1_qubit_reference_1ac52025ebf1860482ecf8e47d932c526b:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`PhysicalQubit<doxid-class_q_panda_1_1_physical_qubit>`* getPhysicalQubitPtr()

Get physical qubit pointer.



.. rubric:: Returns:

:ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` \*

.. index:: pair: function; getOccupancy
.. _doxid-class_q_panda_1_1_qubit_reference_1a7eed27269ff858ef49e6a1a2d2162833:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual bool getOccupancy()

get the occupancy status of this qubit



.. rubric:: Returns:

:ref:`PhysicalQubit <doxid-class_q_panda_1_1_physical_qubit>` \*

