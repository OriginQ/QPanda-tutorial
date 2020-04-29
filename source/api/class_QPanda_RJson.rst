.. index:: pair: class; QPanda::RJson
.. _doxid-class_q_panda_1_1_r_json:

class QPanda::RJson
===================

.. toctree::
	:hidden:

Overview
~~~~~~~~

a wrapper class of rapidjson. :ref:`More...<details-class_q_panda_1_1_r_json>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <RJson.h>
	
	class RJson
	{
	public:
		// methods
	
		static int :ref:`GetValue<doxid-class_q_panda_1_1_r_json_1a7ad74363f6b93693716a5baf79dd33ee>`(
			const rapidjson::Value** value,
			const char* name,
			const rapidjson::Value* parent
			);
	
		static int :ref:`GetValue<doxid-class_q_panda_1_1_r_json_1a16acb2a171ec115202d4171737dbd0d4>`(
			const rapidjson::Value** value,
			const size_t idx,
			const rapidjson::Value* parent
			);
	
		template <typename T>
		static int :ref:`GetObject<doxid-class_q_panda_1_1_r_json_1aeaadc3170a9dcdaaff480ba3837ffa8d>`(
			const rapidjson::Value** value,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
			const rapidjson::Value* parent
			);
	
		template <typename T>
		static int :ref:`GetArray<doxid-class_q_panda_1_1_r_json_1a228d59ffaa9c55811539579206b030fb>`(
			const rapidjson::Value** value,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
			const rapidjson::Value* parent
			);
	
		template <typename T>
		static int :ref:`GetStr<doxid-class_q_panda_1_1_r_json_1acbc41c84398ae1192ffbed56983ad65c>`(
			std::string& str,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
			const rapidjson::Value* parent
			);
	
		template <typename T>
		static int :ref:`GetBool<doxid-class_q_panda_1_1_r_json_1ab27f180373f16b61ed7a04b9a34d6dd5>`(
			bool& n,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
			const rapidjson::Value* parent
			);
	
		template <typename T>
		static int :ref:`GetInt<doxid-class_q_panda_1_1_r_json_1a4105a7484889d37e52b4a02f067e41af>`(int& n, :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag, const rapidjson::Value* parent);
	
		template <typename T>
		static int :ref:`GetDouble<doxid-class_q_panda_1_1_r_json_1aced730b4fd25111b83788a9725e3f514>`(
			double& n,
			:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
			const rapidjson::Value* parent
			);
	
		template <typename T1, typename T2>
		static int :ref:`GetValue<doxid-class_q_panda_1_1_r_json_1a452e159ea1c96c11034681398f983e29>`(
			const rapidjson::Value** value,
			T1 t1,
			T2 t2,
			const rapidjson::Value* parent
			);
	
		template <typename T1, typename T2>
		static int :ref:`GetObject<doxid-class_q_panda_1_1_r_json_1ac91302d5ad54658c49fa042d38ad5ace>`(
			const rapidjson::Value** value,
			T1 t1,
			T2 t2,
			const rapidjson::Value* parent
			);
	
		template <typename T1, typename T2>
		static int :ref:`GetArray<doxid-class_q_panda_1_1_r_json_1ad6f83a66226df2765e1189a8aae413cc>`(
			const rapidjson::Value** value,
			T1 t1,
			T2 t2,
			const rapidjson::Value* parent
			);
	
		template <typename T1, typename T2>
		static int :ref:`GetStr<doxid-class_q_panda_1_1_r_json_1a2aed65d735604c20dafdca38dff8b5db>`(
			std::string& str,
			T1 t1,
			T2 t2,
			const rapidjson::Value* parent
			);
	
		template <typename T1, typename T2>
		static int :ref:`GetBool<doxid-class_q_panda_1_1_r_json_1a76979bdd18dc50d4bcea1caaef3813d9>`(
			bool& n,
			T1 t1,
			T2 t2,
			const rapidjson::Value* parent
			);
	
		template <typename T1, typename T2>
		static int :ref:`GetInt<doxid-class_q_panda_1_1_r_json_1aad0e83966e10ed3022d7e21169801061>`(
			int& n,
			T1 t1,
			T2 t2,
			const rapidjson::Value* parent
			);
	
		template <typename T1, typename T2>
		static int :ref:`GetDouble<doxid-class_q_panda_1_1_r_json_1ab207a097578ffd3a226e90b85c19dbf0>`(
			double& n,
			T1 t1,
			T2 t2,
			const rapidjson::Value* parent
			);
	
		static int :ref:`ToString<doxid-class_q_panda_1_1_r_json_1a82bfe5b843f22d8c367e6c9b3563ea6e>`(std::string& str, const rapidjson::Value* node);
		static std::string :ref:`ToString<doxid-class_q_panda_1_1_r_json_1a56fb6907cb114d3107de6f1f0300d80a>`(const rapidjson::Value* node);
		static bool :ref:`parse<doxid-class_q_panda_1_1_r_json_1a1ba87365fab1ba31be3643d0ce4486f8>`(const std::string& filename, rapidjson::Document& doc);
	
		static bool :ref:`validate<doxid-class_q_panda_1_1_r_json_1a230b5be0eadebdf645a4a7f915869c58>`(
			const std::string& filename,
			const std::string& config_schema,
			rapidjson::Document& doc
			);
	};
.. _details-class_q_panda_1_1_r_json:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

a wrapper class of rapidjson.

Methods
-------

.. index:: pair: function; GetValue
.. _doxid-class_q_panda_1_1_r_json_1a7ad74363f6b93693716a5baf79dd33ee:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static int GetValue(
		const rapidjson::Value** value,
		const char* name,
		const rapidjson::Value* parent
		)

get the val by the name of a key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*\*

		- Pointer of a pointer, pointer to the storage Memory address.

	*
		- char\*

		- the name of key

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetValue
.. _doxid-class_q_panda_1_1_r_json_1a16acb2a171ec115202d4171737dbd0d4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static int GetValue(
		const rapidjson::Value** value,
		const size_t idx,
		const rapidjson::Value* parent
		)

get the val by index



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*\*

		- Pointer of a pointer, pointer to the storage Memory address.

	*
		- size_t

		- the target index

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetObject
.. _doxid-class_q_panda_1_1_r_json_1aeaadc3170a9dcdaaff480ba3837ffa8d:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static int GetObject(
		const rapidjson::Value** value,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
		const rapidjson::Value* parent
		)

get the object by tag



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*\*

		- Pointer of a pointer, pointer to the storage Memory address.

	*
		- T

		- tag

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetArray
.. _doxid-class_q_panda_1_1_r_json_1a228d59ffaa9c55811539579206b030fb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static int GetArray(
		const rapidjson::Value** value,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
		const rapidjson::Value* parent
		)

get the array by tag



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*\*

		- Pointer of a pointer, pointer to the storage Memory address.

	*
		- T

		- tag

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetStr
.. _doxid-class_q_panda_1_1_r_json_1acbc41c84398ae1192ffbed56983ad65c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static int GetStr(
		std::string& str,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
		const rapidjson::Value* parent
		)

get the string of tag



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- the string of tag

	*
		- T

		- tag

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetBool
.. _doxid-class_q_panda_1_1_r_json_1ab27f180373f16b61ed7a04b9a34d6dd5:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static int GetBool(
		bool& n,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
		const rapidjson::Value* parent
		)

get the bool val of tag



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool&

		- the bool val

	*
		- T

		- tag

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetInt
.. _doxid-class_q_panda_1_1_r_json_1a4105a7484889d37e52b4a02f067e41af:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static int GetInt(
		int& n,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
		const rapidjson::Value* parent
		)

get the int val of tag



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int&

		- the int val

	*
		- T

		- tag

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetDouble
.. _doxid-class_q_panda_1_1_r_json_1aced730b4fd25111b83788a9725e3f514:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	static int GetDouble(
		double& n,
		:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>` tag,
		const rapidjson::Value* parent
		)

get the double val of tag



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double&

		- the double val

	*
		- T

		- tag

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetValue
.. _doxid-class_q_panda_1_1_r_json_1a452e159ea1c96c11034681398f983e29:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T1, typename T2>
	static int GetValue(
		const rapidjson::Value** value,
		T1 t1,
		T2 t2,
		const rapidjson::Value* parent
		)

get the val of t1.t2



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*\*

		- Pointer of a pointer, pointer to the storage Memory address.

	*
		- T1

		- t1

	*
		- T2

		- t2

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetObject
.. _doxid-class_q_panda_1_1_r_json_1ac91302d5ad54658c49fa042d38ad5ace:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T1, typename T2>
	static int GetObject(
		const rapidjson::Value** value,
		T1 t1,
		T2 t2,
		const rapidjson::Value* parent
		)

get the object pointer of t1.t2



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*\*

		- Pointer of a pointer, pointer to the storage Memory address.

	*
		- T1

		- t1

	*
		- T2

		- t2

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetArray
.. _doxid-class_q_panda_1_1_r_json_1ad6f83a66226df2765e1189a8aae413cc:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T1, typename T2>
	static int GetArray(
		const rapidjson::Value** value,
		T1 t1,
		T2 t2,
		const rapidjson::Value* parent
		)

get the Array pointer of t1.t2



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*\*

		- Pointer of a pointer, pointer to the storage Memory address.

	*
		- T1

		- t1

	*
		- T2

		- t2

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetStr
.. _doxid-class_q_panda_1_1_r_json_1a2aed65d735604c20dafdca38dff8b5db:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T1, typename T2>
	static int GetStr(
		std::string& str,
		T1 t1,
		T2 t2,
		const rapidjson::Value* parent
		)

get the string of t1.t2



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- the target string

	*
		- T1

		- t1

	*
		- T2

		- t2

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetBool
.. _doxid-class_q_panda_1_1_r_json_1a76979bdd18dc50d4bcea1caaef3813d9:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T1, typename T2>
	static int GetBool(
		bool& n,
		T1 t1,
		T2 t2,
		const rapidjson::Value* parent
		)

get the bool val of t1.t2



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- bool&

		- the target bool val

	*
		- T1

		- t1

	*
		- T2

		- t2

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetInt
.. _doxid-class_q_panda_1_1_r_json_1aad0e83966e10ed3022d7e21169801061:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T1, typename T2>
	static int GetInt(
		int& n,
		T1 t1,
		T2 t2,
		const rapidjson::Value* parent
		)

get the int val of t1.t2



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int&

		- the target int val

	*
		- T1

		- t1

	*
		- T2

		- t2

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; GetDouble
.. _doxid-class_q_panda_1_1_r_json_1ab207a097578ffd3a226e90b85c19dbf0:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T1, typename T2>
	static int GetDouble(
		double& n,
		T1 t1,
		T2 t2,
		const rapidjson::Value* parent
		)

get the double val of t1.t2



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double&

		- the target double val

	*
		- T1

		- t1

	*
		- T2

		- t2

	*
		- rapidjson::Value\*

		- parent node pointer



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; ToString
.. _doxid-class_q_panda_1_1_r_json_1a82bfe5b843f22d8c367e6c9b3563ea6e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static int ToString(std::string& str, const rapidjson::Value* node)

node data to string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- the string of node data

	*
		- rapidjson::Value\*

		- the target node



.. rubric:: Returns:

int 0: on success, -1: others

.. index:: pair: function; ToString
.. _doxid-class_q_panda_1_1_r_json_1a56fb6907cb114d3107de6f1f0300d80a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static std::string ToString(const rapidjson::Value* node)

node data to string



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- rapidjson::Value\*

		- the target node



.. rubric:: Returns:

std::string the string of node data. if any error occurred, the returned string is empty.

.. index:: pair: function; parse
.. _doxid-class_q_panda_1_1_r_json_1a1ba87365fab1ba31be3643d0ce4486f8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool parse(const std::string& filename, rapidjson::Document& doc)

parse a faile



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- the target file name

	*
		- rapidjson::Document&

		- JSON file parser



.. rubric:: Returns:

bool return true on success, or else false on any error occurred

.. index:: pair: function; validate
.. _doxid-class_q_panda_1_1_r_json_1a230b5be0eadebdf645a4a7f915869c58:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	static bool validate(
		const std::string& filename,
		const std::string& config_schema,
		rapidjson::Document& doc
		)

judge the file whether valid or not.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- the target file name

	*
		- std::string&

		- the config schema

	*
		- rapidjson::Document&

		- JSON file parser



.. rubric:: Returns:

bool if file is valid return true, or else return false

