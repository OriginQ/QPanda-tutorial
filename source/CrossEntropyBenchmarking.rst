
交叉熵基准
==========================

简介
--------------
交叉熵基准测试（xeb）是一种通过应用随机电路并测量观察到的位串测量值与从模拟获得的这些位串的预期概率之间的交叉熵来评估门性能的方法。

接口说明
--------------
``double_gate_xeb`` 输入参数分别噪声虚拟机或者量子云机器、待测量的量子比特0、待测量的量子比特1、线路不同层数、随机线路的数量、测量次数、验证双门类型（默认CZ门）。
输出为 ``std::map`` 数据，关键值为线路层数，数值对应符合期望概率的大小。

实例
--------------
.. code-block:: c

    #include "QPanda.h"
    USING_QPANDA
    using namespace std;
    int main()
    {
        // 创建噪声虚拟机
        auto qvm = new NoiseQVM();
        qvm->init();
        
        // 同样可以申请云计算机器（采用真实芯片）
        //auto qvm = new QCloudMachine();
        //qvm->init("898D47CF515A48CEAA9F2326394B85C6")

        auto qv = qvm->qAllocMany(4);

        // 设置噪声参数
        std::vector<QVec> qvs = { { qv[0], qv[1] } };
        qvm->set_noise_model(DEPOLARIZING_KRAUS_OPERATOR, CZ_GATE, 0.1, qvs);

        // 设置不同层数组合
        std::vector<int> range = { 2,4,6,8,10 };
        auto res = double_gate_xeb(qvm, qv[0], qv[1], range, 10, 1000, CZ_GATE);
       
        // 对应的数值随噪声影响，噪声数值越大，所得结果越小，且层数增多，结果数值越小。
        for (auto it : res)
        {
            std::cout << it.first << "  :  " << it.second << std::endl;
        }
        qvm->finalize();
        delete qvm;
        return 0;
    }

运行结果：
::

    2   :  0.963627
    4   :  0.914385
    6   :  0.752838
    8   :  0.722809
    10  :  0.742715