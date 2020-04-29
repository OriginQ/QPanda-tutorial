.. index:: pair: class; QPanda::QReset
.. _doxid-class_q_panda_1_1_q_reset:

class QPanda::QReset
====================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Quantum Reset basic class. :ref:`More...<details-class_q_panda_1_1_q_reset>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QReset.h>
	
	class QReset: public :ref:`QPanda::AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`
	{
	public:
		// construction
	
		:target:`QReset<doxid-class_q_panda_1_1_q_reset_1a0ea5e216e7c93cdf18801b30854a7c59>`();
		:target:`QReset<doxid-class_q_panda_1_1_q_reset_1a7dd3140d019ac37d572a4ddbe34b5637>`(const QReset&);
		:target:`QReset<doxid-class_q_panda_1_1_q_reset_1a4a6758ac349879628be0fdbd9edcc992>`(:ref:`Qubit<doxid-class_q_panda_1_1_qubit>`*);
		:target:`QReset<doxid-class_q_panda_1_1_q_reset_1a444fe0531aafc92909d8316fe846ecf6>`(std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> node);

		// methods
	
		std::shared_ptr<:ref:`AbstractQuantumReset<doxid-class_q_panda_1_1_abstract_quantum_reset>`> :target:`getImplementationPtr<doxid-class_q_panda_1_1_q_reset_1ac29ee99ce05836811c39cd7a252b5faf>`();
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_q_reset_1a63a6330db52d8f32a0d456838df3511f>`() const;
		:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` :ref:`getNodeType<doxid-class_q_panda_1_1_q_reset_1a08d729ca24aa6843957119e6980040f4>`() const;
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// methods
	
		virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* :ref:`getQuBit<doxid-class_q_panda_1_1_abstract_quantum_reset_1a60c3a60eff08e2cfeba20c3662cdb4cb>`() const = 0;

.. _details-class_q_panda_1_1_q_reset:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Quantum Reset basic class.

Methods
-------

.. index:: pair: function; getQuBit
.. _doxid-class_q_panda_1_1_q_reset_1a63a6330db52d8f32a0d456838df3511f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	virtual :ref:`Qubit<doxid-class_q_panda_1_1_qubit>`* getQuBit() const

Get reset node qubit address.



.. rubric:: Returns:

:ref:`QPanda::Qubit <doxid-class_q_panda_1_1_qubit>` \* QuBit address

.. index:: pair: function; getNodeType
.. _doxid-class_q_panda_1_1_q_reset_1a08d729ca24aa6843957119e6980040f4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`NodeType<doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>` getNodeType() const

Get current node type.



.. rubric:: Returns:

NodeType current node type



.. rubric:: See also:

:ref:`NodeType <doxid-_q_global_variable_8h_1acac9cbaeea226ed297804c012dc12b16>`

