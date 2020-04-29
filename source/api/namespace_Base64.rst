.. index:: pair: namespace; Base64
.. _doxid-namespace_base64:

namespace Base64
================

.. toctree::
	:hidden:

Overview
~~~~~~~~




.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	
	namespace Base64 {

	// global functions

	uint8_t :target:`uc_decode<doxid-namespace_base64_1aaeabb0dfd5c415d7fe35e3ff503f9975>`(uint8_t uc);
	uint8_t :target:`uc_encode<doxid-namespace_base64_1ae734d4c27f998bcb17f0b72745534060>`(uint8_t uc);
	std::vector<uint8_t> :ref:`encode<doxid-namespace_base64_1a321717cb4ea6f85b62da5e80c4bba528>`(const void* input, size_t length);
	std::vector<uint8_t> :ref:`encode<doxid-namespace_base64_1aebe1ea0855fe7b750db0569da4045236>`(const std::vector<uint8_t>& bin);
	std::vector<uint8_t> :ref:`decode<doxid-namespace_base64_1a02c0ac9d4538b847dd84371910807483>`(const void* input, size_t length);
	std::vector<uint8_t> :ref:`decode<doxid-namespace_base64_1a7c2be7ea4870b4a5d8db38058535fcf1>`(const std::vector<uint8_t>& input);

	} // namespace Base64
.. _details-namespace_base64:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~



Global Functions
----------------

.. index:: pair: function; encode
.. _doxid-namespace_base64_1a321717cb4ea6f85b62da5e80c4bba528:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<uint8_t> encode(const void* input, size_t length)

Encodes supplied bytes into base64 encoded octets.

.. index:: pair: function; encode
.. _doxid-namespace_base64_1aebe1ea0855fe7b750db0569da4045236:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<uint8_t> encode(const std::vector<uint8_t>& bin)

Encodes supplied bytes into base64 encoded octets.

.. index:: pair: function; decode
.. _doxid-namespace_base64_1a02c0ac9d4538b847dd84371910807483:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<uint8_t> decode(const void* input, size_t length)

Decodes supplied base64 encoded octets into raw bytes.

.. index:: pair: function; decode
.. _doxid-namespace_base64_1a7c2be7ea4870b4a5d8db38058535fcf1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<uint8_t> decode(const std::vector<uint8_t>& input)

Decodes supplied base64 encoded octets into raw bytes.

