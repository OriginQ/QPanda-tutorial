.. index:: pair: class; QPanda::OriginCollection
.. _doxid-class_q_panda_1_1_origin_collection:

class QPanda::OriginCollection
==============================

.. toctree::
	:hidden:

Overview
~~~~~~~~

Origin Collection A relatively free data collection class for saving data. :ref:`More...<details-class_q_panda_1_1_origin_collection>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <OriginCollection.h>
	
	class OriginCollection
	{
	public:
		// construction
	
		:ref:`OriginCollection<doxid-class_q_panda_1_1_origin_collection_1a2db9090428e3bca5d0500b4edf2d67bb>`();
		:ref:`OriginCollection<doxid-class_q_panda_1_1_origin_collection_1a90beb2307c443825a1de635364355857>`(const std::string& file_path, bool is_suffix = true);
		:ref:`OriginCollection<doxid-class_q_panda_1_1_origin_collection_1ab5969c7dd36f81149e2f196d0da6bf70>`(const OriginCollection& old);

		// methods
	
		template <typename T>
		void :ref:`addValue<doxid-class_q_panda_1_1_origin_collection_1a1b23255ce901261e80080cac25f2da86>`(const std::string& key_name, const :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& value);
	
		template <typename T>
		void :ref:`addValue<doxid-class_q_panda_1_1_origin_collection_1a3fe4d2e2bc0c28a0e302cf5e696dbc55>`(
			const std::string& key_name,
			const std::vector<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>& value
			);
	
		void :ref:`addValue<doxid-class_q_panda_1_1_origin_collection_1a76309cea6d008a1512b1b0b8875d0e58>`(const std::string& key_name, const std::vector<std::string>& value);
		void :ref:`addValue<doxid-class_q_panda_1_1_origin_collection_1aba87a7379dc26d5401a32f11ec7b345f>`(const std::string& key_name, const std::string& value);
		void :ref:`addValue<doxid-class_q_panda_1_1_origin_collection_1a50403ce6a3815e311b336fa033f88485>`(const std::string& key_name, const char* value);
		void :target:`addValue<doxid-class_q_panda_1_1_origin_collection_1a3a563cdecda0c0cdd862ce8f9c3285e0>`(const std::string& key_name);
		OriginCollection& :ref:`operator =<doxid-class_q_panda_1_1_origin_collection_1af70a170b317e6daa1c689a561ceddbb4>` (const std::initializer_list<std::string>& args);
		OriginCollection& :ref:`operator =<doxid-class_q_panda_1_1_origin_collection_1a1610d2f3e676f0b16e3bb31506c83e5e>` (const std::vector<std::string>& args);
		OriginCollection& :ref:`operator =<doxid-class_q_panda_1_1_origin_collection_1a2889d90b947b8dd108189da61feed720>` (const OriginCollection& old);
	
		template <typename T>
		void :ref:`setValueByKey<doxid-class_q_panda_1_1_origin_collection_1a52fa7a394c3c771b564e595b4ff59086>`(
			const std::string& name,
			const std::initializer_list<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> args
			);
	
		void :ref:`setValueByKey<doxid-class_q_panda_1_1_origin_collection_1a9ed765942441afe84fd2b65cb4683dd8>`(const std::string& name, const std::initializer_list<std::string> args);
		void :ref:`setValueByKey<doxid-class_q_panda_1_1_origin_collection_1a182051f584319046dbd797d803f3daee>`(const std::string& name, const std::initializer_list<const char*> args);
	
		template <typename T>
		void :ref:`setValueByKey<doxid-class_q_panda_1_1_origin_collection_1a770daee31b97319f3a49fe5e1f0ff13a>`(
			const std::string& name,
			const std::vector<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>& value
			);
	
		template <class... ARG>
		void :ref:`insertValue<doxid-class_q_panda_1_1_origin_collection_1aa3c34eda75cf8394fcb6a7242a6d8c70>`(const std::string& key, ARG... arg);
	
		template <class... ARG>
		void :ref:`insertValue<doxid-class_q_panda_1_1_origin_collection_1a87ed70221697f6fe85c4eca29a8240ae>`(const int key, ARG... arg);
	
		template <class... ARG>
		void :target:`insertValue<doxid-class_q_panda_1_1_origin_collection_1a3994ea23c9d5eb12d12f9ed55d2511b8>`(
			const std::vector<std::string>& name_vector,
			const std::string& key,
			ARG... args
			);
	
		template <class... ARG>
		void :target:`insertValue<doxid-class_q_panda_1_1_origin_collection_1a866fefc1bda365ff01b02d4b1fc90c1f>`(
			const std::vector<std::string>& name_vector,
			const int key,
			ARG... args
			);
	
		std::vector<std::string> :ref:`getValue<doxid-class_q_panda_1_1_origin_collection_1a3a73c463a16b1965b7b48b8eae5c48c1>`(const std::string name);
		std::string :ref:`getValueByKey<doxid-class_q_panda_1_1_origin_collection_1aa79459025e63422c5411d1ea4078e018>`(const std::string& key_value);
		std::string :ref:`getValueByKey<doxid-class_q_panda_1_1_origin_collection_1a83ea3aa5ed955b28bcd74ff4993473e8>`(int key_value);
		bool :ref:`open<doxid-class_q_panda_1_1_origin_collection_1ae13a49fb1f6b433df13414d9fcb7837e>`(const std::string& file_name);
		bool :ref:`write<doxid-class_q_panda_1_1_origin_collection_1aba7ae90d963da6dcf0a0806eaf817912>`();
		std::string :ref:`getJsonString<doxid-class_q_panda_1_1_origin_collection_1a69ff1f08d2ee8e16ba7945b044c4a209>`();
		std::string :ref:`getFilePath<doxid-class_q_panda_1_1_origin_collection_1a0555c6e1549bcd3e2966bce9725f2756>`();
		std::vector<std::string> :target:`getKeyVector<doxid-class_q_panda_1_1_origin_collection_1a580b3eb9d662ec1597050405da6ec622>`();
	};
.. _details-class_q_panda_1_1_origin_collection:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

Origin Collection A relatively free data collection class for saving data.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- number

		- The num of key

Construction
------------

.. index:: pair: function; OriginCollection
.. _doxid-class_q_panda_1_1_origin_collection_1a2db9090428e3bca5d0500b4edf2d67bb:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginCollection()

Construct a new Origin Collection object.

.. index:: pair: function; OriginCollection
.. _doxid-class_q_panda_1_1_origin_collection_1a90beb2307c443825a1de635364355857:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginCollection(const std::string& file_path, bool is_suffix = true)

Construct a new Origin Collection Construct a new Origin Collection by file_path.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- file_path

		- File path

.. index:: pair: function; OriginCollection
.. _doxid-class_q_panda_1_1_origin_collection_1ab5969c7dd36f81149e2f196d0da6bf70:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginCollection(const OriginCollection& old)

Construct a new Origin Collection object by other Origin Collection.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- old

		- target :ref:`OriginCollection <doxid-class_q_panda_1_1_origin_collection>`

Methods
-------

.. index:: pair: function; addValue
.. _doxid-class_q_panda_1_1_origin_collection_1a1b23255ce901261e80080cac25f2da86:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	void addValue(const std::string& key_name, const :ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`& value)

add value Assign a value to the specified key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- value type

	*
		- value_name

		- Key name

	*
		- num

		- Key position in json

	*
		- value

		- key value

.. index:: pair: function; addValue
.. _doxid-class_q_panda_1_1_origin_collection_1a3fe4d2e2bc0c28a0e302cf5e696dbc55:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	void addValue(
		const std::string& key_name,
		const std::vector<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>& value
		)

add value Assign a value to the specified key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- value type

	*
		- value_name

		- Key name

	*
		- num

		- Key position in json

	*
		- value

		- key value

.. index:: pair: function; addValue
.. _doxid-class_q_panda_1_1_origin_collection_1a76309cea6d008a1512b1b0b8875d0e58:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void addValue(
		const std::string& key_name,
		const std::vector<std::string>& value
		)

add value Assign a value to the specified key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- value type

	*
		- value_name

		- Key name

	*
		- num

		- Key position in json

	*
		- value

		- key value

.. index:: pair: function; addValue
.. _doxid-class_q_panda_1_1_origin_collection_1aba87a7379dc26d5401a32f11ec7b345f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void addValue(const std::string& key_name, const std::string& value)

add value Set the value corresponding to the key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value_name

		- Key name

	*
		- num

		- Key position in json

	*
		- value

		- Key value

.. index:: pair: function; addValue
.. _doxid-class_q_panda_1_1_origin_collection_1a50403ce6a3815e311b336fa033f88485:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void addValue(const std::string& key_name, const char* value)

add value Set the value corresponding to the key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- value_name

		- Key name

	*
		- num

		- Key position in json

	*
		- value

		- Key value

.. index:: pair: function; operator=
.. _doxid-class_q_panda_1_1_origin_collection_1af70a170b317e6daa1c689a561ceddbb4:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginCollection& operator = (const std::initializer_list<std::string>& args)

operator= Set the key of the object



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- args

		- arg list Key list



.. rubric:: Returns:

:ref:`OriginCollection <doxid-class_q_panda_1_1_origin_collection>` &

.. index:: pair: function; operator=
.. _doxid-class_q_panda_1_1_origin_collection_1a1610d2f3e676f0b16e3bb31506c83e5e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginCollection& operator = (const std::vector<std::string>& args)

operator= Set the key of the object



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- args

		- arg list Key list



.. rubric:: Returns:

:ref:`OriginCollection <doxid-class_q_panda_1_1_origin_collection>` &

.. index:: pair: function; operator=
.. _doxid-class_q_panda_1_1_origin_collection_1a2889d90b947b8dd108189da61feed720:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	OriginCollection& operator = (const OriginCollection& old)

operator= by other :ref:`OriginCollection <doxid-class_q_panda_1_1_origin_collection>`



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- old

		- target :ref:`OriginCollection <doxid-class_q_panda_1_1_origin_collection>`



.. rubric:: Returns:

:ref:`OriginCollection <doxid-class_q_panda_1_1_origin_collection>` &

.. index:: pair: function; setValueByKey
.. _doxid-class_q_panda_1_1_origin_collection_1a52fa7a394c3c771b564e595b4ff59086:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	void setValueByKey(
		const std::string& name,
		const std::initializer_list<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`> args
		)

Set the Value set value list by key.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- args type

	*
		- name

		- key name

	*
		- args

		- value array

.. index:: pair: function; setValueByKey
.. _doxid-class_q_panda_1_1_origin_collection_1a9ed765942441afe84fd2b65cb4683dd8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setValueByKey(
		const std::string& name,
		const std::initializer_list<std::string> args
		)

Set the Value set value list by key.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- key name

	*
		- args

		- value array

.. index:: pair: function; setValueByKey
.. _doxid-class_q_panda_1_1_origin_collection_1a182051f584319046dbd797d803f3daee:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setValueByKey(
		const std::string& name,
		const std::initializer_list<const char*> args
		)

Set the Value set value list by key.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- key name

	*
		- args

		- value array

.. index:: pair: function; setValueByKey
.. _doxid-class_q_panda_1_1_origin_collection_1a770daee31b97319f3a49fe5e1f0ff13a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <typename T>
	void setValueByKey(
		const std::string& name,
		const std::vector<:ref:`T<doxid-group___quantum_circuit_1ga1a3a2817333d06885d20303a8746e658>`>& value
		)

Set the Value set vector<T> value by key.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- T

		- args type

	*
		- name

		- key name

	*
		- args

		- value array

.. index:: pair: function; insertValue
.. _doxid-class_q_panda_1_1_origin_collection_1aa3c34eda75cf8394fcb6a7242a6d8c70:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class... ARG>
	void insertValue(const std::string& key, ARG... arg)

insert value Set the value of other properties by the value of the primary key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ARG

		- Variable length parameter tparam

	*
		- key

		- Key value

	*
		- arg

		- the value of other properties

.. index:: pair: function; insertValue
.. _doxid-class_q_panda_1_1_origin_collection_1a87ed70221697f6fe85c4eca29a8240ae:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	template <class... ARG>
	void insertValue(const int key, ARG... arg)

insert value Set the value of other properties by the value of the primary key



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- ARG

		- Variable length parameter tparam

	*
		- key

		- Key value

	*
		- arg

		- the value of other properties

.. index:: pair: function; getValue
.. _doxid-class_q_panda_1_1_origin_collection_1a3a73c463a16b1965b7b48b8eae5c48c1:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::vector<std::string> getValue(const std::string name)

Get value by Key.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- name

		- Key name



.. rubric:: Returns:

std::vector<std::string> value vector

.. index:: pair: function; getValueByKey
.. _doxid-class_q_panda_1_1_origin_collection_1aa79459025e63422c5411d1ea4078e018:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getValueByKey(const std::string& key_value)

Get value by primary Key value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- key_value

		- primary Key value



.. rubric:: Returns:

std::string

.. index:: pair: function; getValueByKey
.. _doxid-class_q_panda_1_1_origin_collection_1a83ea3aa5ed955b28bcd74ff4993473e8:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getValueByKey(int key_value)

Get value by primary Key value.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- key_value

		- primary Key value



.. rubric:: Returns:

std::string

.. index:: pair: function; open
.. _doxid-class_q_panda_1_1_origin_collection_1ae13a49fb1f6b433df13414d9fcb7837e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool open(const std::string& file_name)

open Read the json file of the specified path



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- file_name

		- file path



.. rubric:: Returns:

true open success

false open fail

.. index:: pair: function; write
.. _doxid-class_q_panda_1_1_origin_collection_1aba7ae90d963da6dcf0a0806eaf817912:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool write()

write Write json file



.. rubric:: Returns:

true Write success

false Write fail

.. index:: pair: function; getJsonString
.. _doxid-class_q_panda_1_1_origin_collection_1a69ff1f08d2ee8e16ba7945b044c4a209:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getJsonString()

Get the Json String Get object json string.



.. rubric:: Returns:

std::string

.. index:: pair: function; getFilePath
.. _doxid-class_q_panda_1_1_origin_collection_1a0555c6e1549bcd3e2966bce9725f2756:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getFilePath()

Get the File Path.



.. rubric:: Returns:

std::string

