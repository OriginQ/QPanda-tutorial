.. index:: pair: class; QPanda::Psi4Wrapper
.. _doxid-class_q_panda_1_1_psi4_wrapper:

class QPanda::Psi4Wrapper
=========================

.. toctree::
	:hidden:

Overview
~~~~~~~~

wrapper class for Psi4. :ref:`More...<details-class_q_panda_1_1_psi4_wrapper>`


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Psi4Wrapper.h>
	
	class Psi4Wrapper
	{
	public:
		// methods
	
		void :ref:`setMolecule<doxid-class_q_panda_1_1_psi4_wrapper_1a44fafb225eb2028045bfa8cd22761751>`(const std::string& molecule);
		std::string :ref:`getMolecule<doxid-class_q_panda_1_1_psi4_wrapper_1a9b474c45d92e1374f0c0c6ebd0bf7122>`();
		void :ref:`setMultiplicity<doxid-class_q_panda_1_1_psi4_wrapper_1aafdc230c6c5e31ecdfbbb02e50039c8a>`(int multiplicity);
		int :ref:`getMultiplicity<doxid-class_q_panda_1_1_psi4_wrapper_1a945868b58e407afcbfa02a1dc5fa4add>`();
		void :ref:`setCharge<doxid-class_q_panda_1_1_psi4_wrapper_1acc265d23678a3f3f209c894b776cd68f>`(int charge);
		int :ref:`getCharge<doxid-class_q_panda_1_1_psi4_wrapper_1a188f47dde0d5f1d88fe74b91f6ed086c>`();
		void :ref:`setBasis<doxid-class_q_panda_1_1_psi4_wrapper_1abbc5afe5c224c4770325c6d5590b0713>`(const std::string basis);
		std::string :ref:`getBasis<doxid-class_q_panda_1_1_psi4_wrapper_1aca05bd856836415210cfe21526e03058>`();
		void :ref:`setEqTolerance<doxid-class_q_panda_1_1_psi4_wrapper_1a256f7801bebddb73960836c860b61790>`(const double val);
		double :ref:`getEqTolerance<doxid-class_q_panda_1_1_psi4_wrapper_1a353c6cbb37bc92ff7f878a8340ef723e>`();
		std::string :ref:`getLastError<doxid-class_q_panda_1_1_psi4_wrapper_1a47160c669e6a816861e1c6758502f01e>`();
		std::string :ref:`getData<doxid-class_q_panda_1_1_psi4_wrapper_1af310c4c4cdce0c9bed1866ea1fc94cab>`();
		void :ref:`initialize<doxid-class_q_panda_1_1_psi4_wrapper_1ad85d432b3fb694912801c49df92ec4a3>`(const std::string& dir);
		bool :ref:`run<doxid-class_q_panda_1_1_psi4_wrapper_1a2e339ec2fe224de53a847ae2b2a9df40>`();
		void :ref:`finalize<doxid-class_q_panda_1_1_psi4_wrapper_1a8dbd2d2c3ba225034a94e38abf206063>`();
	};
.. _details-class_q_panda_1_1_psi4_wrapper:

Detailed Documentation
~~~~~~~~~~~~~~~~~~~~~~

wrapper class for Psi4.

Methods
-------

.. index:: pair: function; setMolecule
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a44fafb225eb2028045bfa8cd22761751:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMolecule(const std::string& molecule)

set molecule



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- string&

		- the name of molecule

.. index:: pair: function; getMolecule
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a9b474c45d92e1374f0c0c6ebd0bf7122:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getMolecule()

get molecule



.. rubric:: Returns:

the name string of the molecule

.. index:: pair: function; setMultiplicity
.. _doxid-class_q_panda_1_1_psi4_wrapper_1aafdc230c6c5e31ecdfbbb02e50039c8a:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setMultiplicity(int multiplicity)

set multiplicity



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- multiplicity val

.. index:: pair: function; getMultiplicity
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a945868b58e407afcbfa02a1dc5fa4add:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int getMultiplicity()

get multiplicity



.. rubric:: Returns:

return the val of the multiplicity

.. index:: pair: function; setCharge
.. _doxid-class_q_panda_1_1_psi4_wrapper_1acc265d23678a3f3f209c894b776cd68f:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setCharge(int charge)

set charge



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- int

		- charge val

.. index:: pair: function; getCharge
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a188f47dde0d5f1d88fe74b91f6ed086c:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	int getCharge()

get charge



.. rubric:: Returns:

return the val of charge

.. index:: pair: function; setBasis
.. _doxid-class_q_panda_1_1_psi4_wrapper_1abbc5afe5c224c4770325c6d5590b0713:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setBasis(const std::string basis)

set Basis



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string

		- the string of Basis

.. index:: pair: function; getBasis
.. _doxid-class_q_panda_1_1_psi4_wrapper_1aca05bd856836415210cfe21526e03058:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getBasis()

get Basis



.. rubric:: Returns:

return the val of Basis

.. index:: pair: function; setEqTolerance
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a256f7801bebddb73960836c860b61790:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void setEqTolerance(const double val)

set Eq Tolerance



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- double

		- the val of Tolerance

.. index:: pair: function; getEqTolerance
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a353c6cbb37bc92ff7f878a8340ef723e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	double getEqTolerance()

get Eq Tolerance



.. rubric:: Returns:

return the val of Tolerance

.. index:: pair: function; getLastError
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a47160c669e6a816861e1c6758502f01e:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getLastError()

get last error string



.. rubric:: Returns:

return the last error string

.. index:: pair: function; getData
.. _doxid-class_q_panda_1_1_psi4_wrapper_1af310c4c4cdce0c9bed1866ea1fc94cab:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	std::string getData()

get the data



.. rubric:: Returns:

return the data string

.. index:: pair: function; initialize
.. _doxid-class_q_panda_1_1_psi4_wrapper_1ad85d432b3fb694912801c49df92ec4a3:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void initialize(const std::string& dir)

Initialize.



.. rubric:: Parameters:

.. list-table::
	:widths: 20 80

	*
		- std::string&

		- the dir of chemiq

.. index:: pair: function; run
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a2e339ec2fe224de53a847ae2b2a9df40:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	bool run()

run Psi4

.. index:: pair: function; finalize
.. _doxid-class_q_panda_1_1_psi4_wrapper_1a8dbd2d2c3ba225034a94e38abf206063:

.. ref-code-block:: cpp
	:class: doxyrest-title-code-block

	void finalize()

release resource

