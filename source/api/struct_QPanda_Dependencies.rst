.. index:: pair: struct; QPanda::Dependencies
.. _doxid-struct_q_panda_1_1_dependencies:

struct QPanda::Dependencies
===========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Represents a sequence of dependencies (should be treated as parallel dependencies) for each node. :ref:`More...<details-struct_q_panda_1_1_dependencies>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OBMTQMapping.h>
	
	struct Dependencies
	{
		// typedefs
	
		typedef std::vector<:ref:`Dep<doxid-struct_q_panda_1_1_dep>`>::iterator :target:`Iterator<doxid-struct_q_panda_1_1_dependencies_1acd3ae687374d6e5da27881b919a36648>`;
		typedef std::vector<:ref:`Dep<doxid-struct_q_panda_1_1_dep>`>::const_iterator :target:`ConstIterator<doxid-struct_q_panda_1_1_dependencies_1a02cd451c1b1cdaa346997911315eaf95>`;

		// fields
	
		std::vector<:ref:`Dep<doxid-struct_q_panda_1_1_dep>`> :target:`mDeps<doxid-struct_q_panda_1_1_dependencies_1a2d1919c1a9c502a0e08bda8142c136a7>`;
		:ref:`QNodeRef<doxid-_qubit_mapping_8h_1a5cd44073de95edede4a142612af4ae41>` :target:`mCallPoint<doxid-struct_q_panda_1_1_dependencies_1af7c1078c69d40b245f760328f2e4e3c8>`;

		// methods
	
		const :ref:`Dep<doxid-struct_q_panda_1_1_dep>`& :ref:`operator []<doxid-struct_q_panda_1_1_dependencies_1aebc6b6a0750c67546e8da73b974ba519>` (uint32_t i) const;
		:ref:`Dep<doxid-struct_q_panda_1_1_dep>`& :ref:`operator []<doxid-struct_q_panda_1_1_dependencies_1afb66d78ad376fb8984b6b8d598ea4ba1>` (uint32_t i);
		bool :ref:`empty<doxid-struct_q_panda_1_1_dependencies_1a919e7fac52645e61f677e463719452df>`() const;
		uint32_t :ref:`size<doxid-struct_q_panda_1_1_dependencies_1a2bab898dfff36adc814fafca50c40cc4>`() const;
		:ref:`Iterator<doxid-struct_q_panda_1_1_dependencies_1acd3ae687374d6e5da27881b919a36648>` :ref:`begin<doxid-struct_q_panda_1_1_dependencies_1a314f3b07cdeaafe0626058e08b0aa875>`();
		:ref:`ConstIterator<doxid-struct_q_panda_1_1_dependencies_1a02cd451c1b1cdaa346997911315eaf95>` :ref:`begin<doxid-struct_q_panda_1_1_dependencies_1a8df6e4ae2ef64cd9a6173ea51cc796a3>`() const;
		:ref:`Iterator<doxid-struct_q_panda_1_1_dependencies_1acd3ae687374d6e5da27881b919a36648>` :ref:`end<doxid-struct_q_panda_1_1_dependencies_1a47110431b8e8dcf91f4248f32f950674>`();
		:ref:`ConstIterator<doxid-struct_q_panda_1_1_dependencies_1a02cd451c1b1cdaa346997911315eaf95>` :ref:`end<doxid-struct_q_panda_1_1_dependencies_1aa692f887cbf5ae03a78681ca6c4644f8>`() const;
	};
.. _details-struct_q_panda_1_1_dependencies:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Represents a sequence of dependencies (should be treated as parallel dependencies) for each node.

Methods
-------

.. index:: pair: function; operator[]
.. _doxid-struct_q_panda_1_1_dependencies_1aebc6b6a0750c67546e8da73b974ba519:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	const :ref:`Dep<doxid-struct_q_panda_1_1_dep>`& operator [] (uint32_t i) const

Forwards to the *mDeps* attribute.

.. index:: pair: function; operator[]
.. _doxid-struct_q_panda_1_1_dependencies_1afb66d78ad376fb8984b6b8d598ea4ba1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Dep<doxid-struct_q_panda_1_1_dep>`& operator [] (uint32_t i)

Forwards to the *mDeps* attribute.

.. index:: pair: function; empty
.. _doxid-struct_q_panda_1_1_dependencies_1a919e7fac52645e61f677e463719452df:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool empty() const

Forwards to the *mDeps* attribute.

.. index:: pair: function; size
.. _doxid-struct_q_panda_1_1_dependencies_1a2bab898dfff36adc814fafca50c40cc4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	uint32_t size() const

Forwards to the *mDeps* attribute.

.. index:: pair: function; begin
.. _doxid-struct_q_panda_1_1_dependencies_1a314f3b07cdeaafe0626058e08b0aa875:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Iterator<doxid-struct_q_panda_1_1_dependencies_1acd3ae687374d6e5da27881b919a36648>` begin()

Forwards to the *mDeps* attribute.

.. index:: pair: function; begin
.. _doxid-struct_q_panda_1_1_dependencies_1a8df6e4ae2ef64cd9a6173ea51cc796a3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ConstIterator<doxid-struct_q_panda_1_1_dependencies_1a02cd451c1b1cdaa346997911315eaf95>` begin() const

Forwards to the *mDeps* attribute.

.. index:: pair: function; end
.. _doxid-struct_q_panda_1_1_dependencies_1a47110431b8e8dcf91f4248f32f950674:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`Iterator<doxid-struct_q_panda_1_1_dependencies_1acd3ae687374d6e5da27881b919a36648>` end()

Forwards to the *mDeps* attribute.

.. index:: pair: function; end
.. _doxid-struct_q_panda_1_1_dependencies_1aa692f887cbf5ae03a78681ca6c4644f8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	:ref:`ConstIterator<doxid-struct_q_panda_1_1_dependencies_1a02cd451c1b1cdaa346997911315eaf95>` end() const

Forwards to the *mDeps* attribute.

