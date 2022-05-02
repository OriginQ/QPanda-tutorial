.. index:: pair: class; QPanda::UncompletedGridDevice
.. _doxid-class_q_panda_1_1_uncompleted_grid_device:

class QPanda::UncompletedGridDevice
===================================

.. toctree::
	:hidden:

:ref:`UncompletedGridDevice <doxid-class_q_panda_1_1_uncompleted_grid_device>` is a derived class of :ref:`SimpleGridDevice <doxid-class_q_panda_1_1_simple_grid_device>` Compared with :ref:`SimpleGridDevice <doxid-class_q_panda_1_1_simple_grid_device>`, some qubits are NOT AVAILABLE, but the adjacent relation is the same e.g. google Sycamore q54.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <GridDevice.h>
	
	class UncompletedGridDevice: public :ref:`QPanda::SimpleGridDevice<doxid-class_q_panda_1_1_simple_grid_device>`
	{
	public:
		// construction
	
		:target:`UncompletedGridDevice<doxid-class_q_panda_1_1_uncompleted_grid_device_1ad868241a9e489ad4b81562fd171819fb>`(
			int m,
			int n,
			const bool* available_qubits
			);

		// methods
	
		void :target:`resetAvailableQubits<doxid-class_q_panda_1_1_uncompleted_grid_device_1a01625838beb6d55c6628b3c822db9202>`(const bool* available_qubits);
	
		bool :target:`isQubitAvailable<doxid-class_q_panda_1_1_uncompleted_grid_device_1a4039eb1f1468321f1dd54be47b1f2785>`(
			int i,
			int j
			);
	};

Inherited Members
-----------------

.. ref-code-block:: cpp
	:class: doxyrest-overview-inherited-code-block

	public:
		// structs
	
		struct :ref:`PhysicalQubit<doxid-struct_q_panda_1_1_basic_grid_device_1_1_physical_qubit>`;

		// methods
	
		void :ref:`clear<doxid-class_q_panda_1_1_basic_grid_device_1a09714a4863204df35d7eb25b8cf62659>`();
		int :ref:`getM<doxid-class_q_panda_1_1_basic_grid_device_1a4580350edef0102343846a7859ae8660>`();
		int :ref:`getN<doxid-class_q_panda_1_1_basic_grid_device_1a7a8225fdebcd7613e91b7e90f66c8f42>`();
		auto& :ref:`getQubit<doxid-class_q_panda_1_1_basic_grid_device_1a5a459002641fd59163c9e401432f3067>`(int i, int j);
		bool :ref:`canApplyGate<doxid-class_q_panda_1_1_basic_grid_device_1a8503407bf9a2886c42df382a06ab8d26>`(int i1, int j1, int i2, int j2, int);
		bool :ref:`canApplyGate<doxid-class_q_panda_1_1_basic_grid_device_1a1742ac2b23467a88d610d0126dc75cae>`(int i, int j, int);
		bool :ref:`canSwap<doxid-class_q_panda_1_1_basic_grid_device_1a76a46b2811d866d2091f218f90674e03>`(int i1, int j1, int i2, int j2);
		void :ref:`applySingleGate<doxid-class_q_panda_1_1_basic_grid_device_1a8009420486f96cc0d115dfe8c8529a45>`(int i, int j);
		void :ref:`applyGate<doxid-class_q_panda_1_1_basic_grid_device_1a80b82b2592f6c40f0aa6198b60f7a299>`(int i1, int j1, int i2, int j2, int time);
		void :ref:`applyDoubleGate<doxid-class_q_panda_1_1_basic_grid_device_1a3e3eae315a5215d359b061bc9a204d54>`(int i1, int j1, int i2, int j2);
		void :ref:`applySwap<doxid-class_q_panda_1_1_basic_grid_device_1ad29ed551bb09088370097b93e3987f30>`(int i1, int j1, int i2, int j2);
		virtual bool :ref:`isNearBy<doxid-class_q_panda_1_1_basic_grid_device_1ad876b3453ae76379e449267a8cfcb3f4>`(int i1, int j1, int i2, int j2) = 0;
		virtual int :ref:`getDistance<doxid-class_q_panda_1_1_basic_grid_device_1aae022b1fcadc203e9d3a92b9ab57afe5>`(int i1, int j1, int i2, int j2) = 0;
		void :ref:`map<doxid-class_q_panda_1_1_basic_grid_device_1acf0aea261a0e455057e23901c170b78e>`(int dest, int i, int j);
		void :ref:`resetTime<doxid-class_q_panda_1_1_basic_grid_device_1a4e341e62b3a245f3a7dba6607458a2a9>`();
		void :ref:`nextCycle<doxid-class_q_panda_1_1_basic_grid_device_1af9af37dfc8f684a1a42fdcef19509ede>`();
		int :ref:`maxTime<doxid-class_q_panda_1_1_basic_grid_device_1a809242f417ef1be38236a72963553cae>`();
		int :ref:`getTime<doxid-class_q_panda_1_1_basic_grid_device_1af8e0c15aa673ab3ddc97674bda1b638c>`();
		bool :ref:`isQubitFree<doxid-class_q_panda_1_1_basic_grid_device_1ae55c1f5d2e3f711d775ad7c2ea1a2e5b>`(int i, int j);
		bool :ref:`isAllQubitFree<doxid-class_q_panda_1_1_basic_grid_device_1a5397662e8b72e6e7d7578f4ee9bb74a7>`();
		bool :ref:`isSimpleGridDevice<doxid-class_q_panda_1_1_basic_grid_device_1a31d1b5609b7ae5054a52fcc60bc21563>`();
		bool :ref:`isSupportSwapGate<doxid-class_q_panda_1_1_basic_grid_device_1a3d340361c313fd45466f2971e8fce525>`();
		virtual bool :ref:`isNearBy<doxid-class_q_panda_1_1_simple_grid_device_1abfbf15807f8f08aa472fc4d9eb80a304>`(int i1, int j1, int i2, int j2);
		virtual int :ref:`getDistance<doxid-class_q_panda_1_1_simple_grid_device_1ad4473632999fa14c59a59758588dafc1>`(int i1, int j1, int i2, int j2);

