.. index:: pair: class; QPanda::QMachineTypeTarnfrom
.. _doxid-class_q_panda_1_1_q_machine_type_tarnfrom:

class QPanda::QMachineTypeTarnfrom
==================================

.. toctree::
	:hidden:

Quantum machine type and name transformation.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <Factory.h>
	
	class QMachineTypeTarnfrom
	{
	public:
		// methods
	
		static QMachineTypeTarnfrom& :target:`getInstance<doxid-class_q_panda_1_1_q_machine_type_tarnfrom_1a49f113d80101ad665c1515c24da44061>`();
		std::string :target:`operator []<doxid-class_q_panda_1_1_q_machine_type_tarnfrom_1a5d09e58a074a4220d80e57e31b879830>` (:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` type);
		:ref:`QMachineType<doxid-namespace_q_panda_1a49e43bfca791e92de2939590de4dcc13>` :target:`operator []<doxid-class_q_panda_1_1_q_machine_type_tarnfrom_1a26ef2d8ac1ebc98184dd865ef09d6036>` (std::string gate_name);
	};
