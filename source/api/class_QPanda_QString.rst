.. index:: pair: class; QPanda::QString
.. _doxid-class_q_panda_1_1_q_string:

class QPanda::QString
=====================

.. toctree::
	:hidden:

	enum_QPanda_QString_BaseCovert.rst
	enum_QPanda_QString_SplitBehavior.rst

:ref:`QString <doxid-class_q_panda_1_1_q_string>`.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <QString.h>
	
	class QString
	{
	public:
		// enums
	
		enum :ref:`BaseCovert<doxid-class_q_panda_1_1_q_string_1aaf67f3d8f35752b8c5a3b2d740e72527>`;
		enum :ref:`SplitBehavior<doxid-class_q_panda_1_1_q_string_1aba63cc1d2eae7186fdac7c8c6628f6f8>`;

		// construction
	
		:target:`QString<doxid-class_q_panda_1_1_q_string_1a9d741c11930a536a13124743e2fd9fe2>`();
		:target:`QString<doxid-class_q_panda_1_1_q_string_1ae61a6ea12853ee42bca888ffbe47462f>`(char c);
		:target:`QString<doxid-class_q_panda_1_1_q_string_1ae8235c4d6214fed20710b8fb93812b21>`(const char* s);
	
		:target:`QString<doxid-class_q_panda_1_1_q_string_1a00851e35d225642d15e1b9b2d08faa7a>`(
			const char* s,
			size_t n
			);
	
		:target:`QString<doxid-class_q_panda_1_1_q_string_1a90d556d04e908a190b62ed329e7eecfb>`(
			size_t n,
			char c
			);
	
		:target:`QString<doxid-class_q_panda_1_1_q_string_1ab878edb39f34c3dd69ecd8f928cdcaf7>`(const std::string& str);
	
		:target:`QString<doxid-class_q_panda_1_1_q_string_1aed4cda29b375dbcd2c7b3f0bb417e706>`(
			const std::string& str,
			size_t pos,
			size_t len = std::string::npos
			);
	
		template <class InputIterator>
		:target:`QString<doxid-class_q_panda_1_1_q_string_1a35948ac6a084a585dada08279dc83471>`(
			InputIterator first,
			InputIterator last
			);
	
		:target:`QString<doxid-class_q_panda_1_1_q_string_1afc152b7f69ef608af259e3bbcec6ab8c>`(std::string&& str);
		:target:`QString<doxid-class_q_panda_1_1_q_string_1a63f70dff1f5da13fc6d79f0272a3ae8b>`(const QString& str);
		:target:`QString<doxid-class_q_panda_1_1_q_string_1a3d5e157704a4f366c7c36d552d4d3fc6>`(QString&& str);

		// methods
	
		QString& :target:`operator =<doxid-class_q_panda_1_1_q_string_1a2b4bc4c2375dcd51da024d4424d3d863>` (const char* s);
		QString& :target:`operator =<doxid-class_q_panda_1_1_q_string_1aec0d292fe9bf6c6af3b7024d25b6fa2f>` (const std::string& str);
		QString& :target:`operator =<doxid-class_q_panda_1_1_q_string_1a4f65fe25e1bb03c67334d53c402d3cf7>` (const QString& str);
		size_t :target:`size<doxid-class_q_panda_1_1_q_string_1af607578b343b50b3b7ae44a7e0c52535>`() const;
		bool :target:`isEmpty<doxid-class_q_panda_1_1_q_string_1a679876fd464fd4d160c94a3bcfb7e3d3>`() const;
	
		size_t :target:`find<doxid-class_q_panda_1_1_q_string_1aa2a74f17f1af03281f524ac20f75f39f>`(
			const QString& sub_str,
			size_t pos = 0
			) const;
	
		char :target:`at<doxid-class_q_panda_1_1_q_string_1ae451c0ffa31828b58be3da015bca5c6c>`(size_t i) const;
		char :target:`operator []<doxid-class_q_panda_1_1_q_string_1a04f5edab6bb9b4c6a43ea9f5abb88c9b>` (size_t i) const;
		char :target:`front<doxid-class_q_panda_1_1_q_string_1a67bb4fbea8d3826d5ac0c6a66e138629>`() const;
		char :target:`back<doxid-class_q_panda_1_1_q_string_1a5406eddb0a2ea729937dc91a97893828>`() const;
		QString :target:`left<doxid-class_q_panda_1_1_q_string_1a11710f1729843d526b2a0b3e1f99ba87>`(size_t n) const;
		QString :target:`right<doxid-class_q_panda_1_1_q_string_1ab6b41f9f5fdcc8ecc63b0f4b6510cee9>`(size_t n) const;
	
		QString :target:`mid<doxid-class_q_panda_1_1_q_string_1a28a1aad1782aacdb79289a8f057011cb>`(
			size_t pos,
			size_t n = std::string::npos
			) const;
	
		std::vector<QString> :target:`split<doxid-class_q_panda_1_1_q_string_1a27ed3c237b5803829af55a4d3b550470>`(
			const QString& sep,
			:ref:`SplitBehavior<doxid-class_q_panda_1_1_q_string_1aba63cc1d2eae7186fdac7c8c6628f6f8>` behavior = :ref:`KeepEmptyParts<doxid-class_q_panda_1_1_q_string_1aba63cc1d2eae7186fdac7c8c6628f6f8a7558c0fb7a9b2ac8457b1233895b3ab4>`
			) const;
	
		std::vector<QString> :target:`splitByStr<doxid-class_q_panda_1_1_q_string_1a018a09bf3acdec56c84a5f901d5734a0>`(
			const QString& sep,
			:ref:`SplitBehavior<doxid-class_q_panda_1_1_q_string_1aba63cc1d2eae7186fdac7c8c6628f6f8>` behavior = :ref:`KeepEmptyParts<doxid-class_q_panda_1_1_q_string_1aba63cc1d2eae7186fdac7c8c6628f6f8a7558c0fb7a9b2ac8457b1233895b3ab4>`
			) const;
	
		QString :target:`trimmed<doxid-class_q_panda_1_1_q_string_1afc5d1779f501585a26bb6ac471b06bc4>`() const;
		QString :target:`toUpper<doxid-class_q_panda_1_1_q_string_1a8af9291f49af8f73def855f4074ca455>`() const;
		QString :target:`toLower<doxid-class_q_panda_1_1_q_string_1a7c367769763d9a69239c0a8e4996e6cc>`() const;
	
		int :target:`toInt<doxid-class_q_panda_1_1_q_string_1a8a01cafe5d0f0bdfe6f1aa6714285ece>`(
			bool* ok = nullptr,
			:ref:`BaseCovert<doxid-class_q_panda_1_1_q_string_1aaf67f3d8f35752b8c5a3b2d740e72527>` base = :ref:`DEC<doxid-class_q_panda_1_1_q_string_1aaf67f3d8f35752b8c5a3b2d740e72527ad9163b52176b3930c7aaf6a82a1b5f69>`
			) const;
	
		float :target:`toFloat<doxid-class_q_panda_1_1_q_string_1a94dcd339bfb528b332545645a3d99086>`(bool* ok = nullptr) const;
		double :target:`toDouble<doxid-class_q_panda_1_1_q_string_1a4bfdd08fd4a1a755ce93763661c84e71>`(bool* ok = nullptr) const;
		const std::string& :target:`data<doxid-class_q_panda_1_1_q_string_1a73e6f1b9acbc4f27c2ea28fded2865af>`() const;
		bool :target:`operator ==<doxid-class_q_panda_1_1_q_string_1a01511af48e007d73bc0e2edec4d1ba54>` (const char* s) const;
		bool :target:`operator !=<doxid-class_q_panda_1_1_q_string_1a7f74a0bd615d79e274a457772898ca26>` (const char* s) const;
		bool :target:`operator <<doxid-class_q_panda_1_1_q_string_1aff03fe087ba3cdfee4d46ff6192cd90f>` (const char* s) const;
		bool :target:`operator ><doxid-class_q_panda_1_1_q_string_1adddc6ae718e5143f2e18114debef3b6b>` (const char* s) const;
		bool :target:`operator <=<doxid-class_q_panda_1_1_q_string_1ab7619f306c436687166e77afac1b4ff2>` (const char* s) const;
		bool :target:`operator >=<doxid-class_q_panda_1_1_q_string_1a67459cfd65d9745b224115318144f33d>` (const char* s) const;
		bool :target:`operator ==<doxid-class_q_panda_1_1_q_string_1aefaa98f04df47d37b1389e3b16f4a4f0>` (const std::string& s) const;
		bool :target:`operator !=<doxid-class_q_panda_1_1_q_string_1a0adb55f4e41c253a92a15a63f115923c>` (const std::string& s) const;
		bool :target:`operator <<doxid-class_q_panda_1_1_q_string_1af6ed4c55f7a47490db694e872d00e386>` (const std::string& s) const;
		bool :target:`operator ><doxid-class_q_panda_1_1_q_string_1a3de4791c6bd9529d51c01ae573be5317>` (const std::string& s) const;
		bool :target:`operator <=<doxid-class_q_panda_1_1_q_string_1a1ead5e6c8dcf65a4c9c71672bce64d9b>` (const std::string& s) const;
		bool :target:`operator >=<doxid-class_q_panda_1_1_q_string_1acae4cb9e29e21d403f2f267c310529a9>` (const std::string& s) const;
	};
