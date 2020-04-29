.. index:: pair: class; QPanda::Variational::var
.. _doxid-class_q_panda_1_1_variational_1_1var:

class QPanda::Variational::var
==============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

The class denotes the variable. :ref:`More...<details-class_q_panda_1_1_variational_1_1var>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <var.h>
	
	class var
	{
	public:
		// fields
	
		std::shared_ptr<:ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl>`> :target:`pimpl<doxid-class_q_panda_1_1_variational_1_1var_1a3c333d0e48e6d4f8b15c273ca10bc384>`;

		// construction
	
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var_1a2be836e1cd4206b85b1afaf7be47b00e>`(std::shared_ptr<:ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl>`>);
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var_1a85b2b8873157bd60d8074fea72634e8d>`(double);
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var_1abfaa969c16de32bbc5c61898a9bfecf1>`(const MatrixXd&);
	
		:target:`var<doxid-class_q_panda_1_1_variational_1_1var_1a25d93a2c61e604aebc2db1b11e8e74fc>`(
			double,
			bool
			);
	
		:target:`var<doxid-class_q_panda_1_1_variational_1_1var_1a6b0e34ace8f2e50de55710035c3981ac>`(
			const MatrixXd&,
			bool
			);
	
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var_1a47c3186c59ecefc5d8ae7d884b6eee95>`(:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` op, const std::vector<var>& children);
		:ref:`var<doxid-class_q_panda_1_1_variational_1_1var_1a796ed20b2ee9d5ec2217199ebb0d8eb8>`(var&&);
		:target:`var<doxid-class_q_panda_1_1_variational_1_1var_1aa2ed62957cfeac78c9f72afbcf610aa2>`(const var&);

		// methods
	
		var& :ref:`operator =<doxid-class_q_panda_1_1_variational_1_1var_1af7babc0a6551403b34e617a2f70fa6be>` (var&&);
		var& :target:`operator =<doxid-class_q_panda_1_1_variational_1_1var_1af1936a6810bc3d3c0da87ac315679a04>` (const var&);
		var :target:`clone<doxid-class_q_panda_1_1_variational_1_1var_1a6f7ad210b868db968f66fc1cecfaf6e7>`();
		virtual size_t :target:`getNumOpArgs<doxid-class_q_panda_1_1_variational_1_1var_1ae638f5b10192cea9d72e7fea4ff5dc37>`();
		MatrixXd :target:`getValue<doxid-class_q_panda_1_1_variational_1_1var_1a721aef2221461099e94d24dee3a03281>`() const;
		void :target:`setValue<doxid-class_q_panda_1_1_variational_1_1var_1a1418e20203ea54bce6dd2430eabbcc38>`(const MatrixXd&);
		:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` :target:`getOp<doxid-class_q_panda_1_1_variational_1_1var_1a5fa572c78f919d9006d52b702485ed7e>`() const;
		void :target:`setOp<doxid-class_q_panda_1_1_variational_1_1var_1aec81f93a64fee840a803ec0de601e94d>`(:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>`);
		std::vector<var>& :target:`getChildren<doxid-class_q_panda_1_1_variational_1_1var_1adcfc84a5cce7eeb2421b6d856e0fb8b0>`() const;
		std::vector<var> :target:`getParents<doxid-class_q_panda_1_1_variational_1_1var_1a8c4addcf97283470bb913ec4e1813202>`() const;
		long :target:`getUseCount<doxid-class_q_panda_1_1_variational_1_1var_1a13cf62fcb48e8cbc497d23b4f3122af6>`() const;
		bool :target:`getValueType<doxid-class_q_panda_1_1_variational_1_1var_1a06f9f8a0e0bf017a9322e9d551357a56>`() const;
		MatrixXd :target:`_eval<doxid-class_q_panda_1_1_variational_1_1var_1a2182f1b8990f72c7adc984dee406e731>`();
	
		MatrixXd :target:`_back_single<doxid-class_q_panda_1_1_variational_1_1var_1af76a67df62a1d395560ba7e0e624a6b8>`(
			const MatrixXd& dx,
			size_t op_idx
			);
	
		std::vector<MatrixXd> :target:`_back<doxid-class_q_panda_1_1_variational_1_1var_1adf028023f5e253553dcf7a631b8fb4a8>`(
			const MatrixXd& dx,
			const std::unordered_set<var>& nonconsts
			);
	
		std::vector<MatrixXd> :target:`_back<doxid-class_q_panda_1_1_variational_1_1var_1aeaacde095b24614cded98d670d2e6ae4>`(const MatrixXd& dx);
		bool :target:`operator ==<doxid-class_q_panda_1_1_variational_1_1var_1ae47a78cd2012c3a7b90cace4f2e96995>` (const var& rhs) const;
		const var :target:`operator []<doxid-class_q_panda_1_1_variational_1_1var_1a9ed4d051bf5677deb8ede139a820a452>` (int subscript);
	};
.. _details-class_q_panda_1_1_variational_1_1var:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

The class denotes the variable.

Construction
------------

.. index:: pair: function; var
.. _doxid-class_q_panda_1_1_variational_1_1var_1a2be836e1cd4206b85b1afaf7be47b00e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	var(std::shared_ptr<:ref:`impl<doxid-struct_q_panda_1_1_variational_1_1impl>`>)

Construct a new var object by the impl object.

.. index:: pair: function; var
.. _doxid-class_q_panda_1_1_variational_1_1var_1a85b2b8873157bd60d8074fea72634e8d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	var(double)

Construct a new var object by a double.

.. index:: pair: function; var
.. _doxid-class_q_panda_1_1_variational_1_1var_1abfaa969c16de32bbc5c61898a9bfecf1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	var(const MatrixXd&)

Construct a new var object by a Eigen matrix.

.. index:: pair: function; var
.. _doxid-class_q_panda_1_1_variational_1_1var_1a47c3186c59ecefc5d8ae7d884b6eee95:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	var(:ref:`op_type<doxid-namespace_q_panda_1_1_variational_1a48cf3e66870553a1904112cfce0fd810>` op, const std::vector<var>& children)

Construct a new var object by the operator type and children.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- op

		- operator type

	*
		- children

		- children of the operator. For example, c = a + b. c is a and b's parent, a and b are c's children

.. index:: pair: function; var
.. _doxid-class_q_panda_1_1_variational_1_1var_1a796ed20b2ee9d5ec2217199ebb0d8eb8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	var(var&&)

move constructor of var

Methods
-------

.. index:: pair: function; operator=
.. _doxid-class_q_panda_1_1_variational_1_1var_1af7babc0a6551403b34e617a2f70fa6be:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	var& operator = (var&&)



.. rubric:: Returns:

var&

