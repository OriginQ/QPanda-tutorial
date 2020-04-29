.. index:: pair: class; AbstractDistributedFullAmplitudeEngine
.. _doxid-class_abstract_distributed_full_amplitude_engine:

class AbstractDistributedFullAmplitudeEngine
============================================

.. toctree::
	:hidden:

Distributed full amplitude engine abstract class.


.. ref-code-block:: cpp
	:class: doxyrest-overview-code-block

	#include <AbstractFullAmplitudeEngine.h>
	
	class AbstractDistributedFullAmplitudeEngine
	{
	public:
		// methods
	
		virtual void :target:`initState<doxid-class_abstract_distributed_full_amplitude_engine_1a056f4917f93f243a6396bae1288f05fb>`(
			int head_rank,
			int rank_size,
			int qubit_num
			) = 0;
	
		virtual :ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` :target:`getQState<doxid-class_abstract_distributed_full_amplitude_engine_1af43a2eea45896b430ac18e0a9bc74829>`() = 0;
	
		virtual void :target:`singleQubitOperation<doxid-class_abstract_distributed_full_amplitude_engine_1a8c4d3d81e6bab86e2a6bfc0450f54646>`(
			const int& iQn,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` U,
			bool isConjugate
			) = 0;
	
		virtual void :target:`controlsingleQubitOperation<doxid-class_abstract_distributed_full_amplitude_engine_1a75f9cf0d79431e9c0916efb95549ca34>`(
			const int& iQn,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` U,
			bool isConjugate
			) = 0;
	
		virtual void :target:`doubleQubitOperation<doxid-class_abstract_distributed_full_amplitude_engine_1a3b0e0d4c12af33994444e24065026082>`(
			const int& iQn1,
			const int& iQn2,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` U,
			bool isConjugate
			) = 0;
	
		virtual void :target:`controldoubleQubitOperation<doxid-class_abstract_distributed_full_amplitude_engine_1a77ffbe1c12354e692881060e640cd3d3>`(
			const int& iQn1,
			const int& iQn2,
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`QStat<doxid-_q_panda_namespace_8h_1aef94fce258d1c9c8e692cf39254aa0ae>` U,
			bool isConjugate
			) = 0;
	
		virtual int :target:`measureQubitOperation<doxid-class_abstract_distributed_full_amplitude_engine_1aa7e01a839c3bea51511fbd12d386476c>`(const int& qn) = 0;
	
		virtual void :target:`PMeasureQubitOperation<doxid-class_abstract_distributed_full_amplitude_engine_1a74388fee7cbf9ab2911e11f3dcd333cb>`(
			:ref:`Qnum<doxid-_q_panda_namespace_8h_1ae79dd36dc218ce815071e5a63b7713f7>`& qnum,
			:ref:`prob_vec<doxid-_q_panda_namespace_8h_1ac5ad900acfc23913f3100fa747b940c0>`& mResult
			) = 0;
	
		virtual void :target:`reset_qubit_operation<doxid-class_abstract_distributed_full_amplitude_engine_1aa2015925f5ef8b39e7b562c709f3342e>`(const int& qn) = 0;
	};
