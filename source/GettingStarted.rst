快速入门
==============

.. _pyqpanda: https://pyqpanda-toturial.readthedocs.io/zh/latest/
QPanda2提供了C++ 和 Python两个版本，本文中主要介绍C++版本的使用。
如要了解和学习python版本的使用请移步 pyqpanda_。

编译环境
>>>>>>>>>

QPanda-2是以C++为宿主语言，其对系统的环境要求如下：

.. list-table::

    * - software
      - version
    * - CMake
      - >= 3.1
    * - GCC
      - >= 5.4.0 
    * - Python
      - >= 3.6.0  


4. 解压下载的文件，就会看到我们的QPanda-2项目， 下面就以linux系统为例简单介绍QPanda2的使用。

    .. code-block:: c
    
        $ cd qpanda-2
        $ mkdir build
        $ cd build
        $ cmake -DCMAKE_INSTALL_PREFIX=/usr/local .. 
        $ make
    
安装
>>>>>>>>

编译完成后，安装就简单的多，只需要输入以下命令：

    .. code-block:: c

        $ make install

开始量子编程
>>>>>>>>>>>>>>

现在我们来到最后一关，创建和编译自己的量子应用。

我相信对于关心如何使用QPanda 2的朋友来说，如何创建C++项目，不需要我多说。不过，我还是需要提供CMakelist.txt的示例，方便大家参考。

    .. code-block:: c

        cmake_minimum_required(VERSION 3.1)
        project(testQPanda)
        SET(CMAKE_INSTALL_PREFIX "/usr/local")
        SET(CMAKE_MODULE_PATH  ${CMAKE_MODULE_PATH} "${CMAKE_INSTALL_PREFIX} lib/cmake")

        add_definitions("-std=c++14 -w -DGTEST_USE_OWN_TR1_TUPLE=1")
        set(CMAKE_BUILD_TYPE "Release")
        set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -g -ggdb")
        set(CMAKE_CXX_FLAGS_RELEASE "$ENV{CXXFLAGS} -O3")
        add_compile_options(-fPIC -fpermissive)
        find_package(QPANDA REQUIRED)
        if (QPANDA_FOUND)

            include_directories(${QPANDA_INCLUDE_DIR}
                            ${THIRD_INCLUDE_DIR})
            add_executable(${PROJECT_NAME} test.cpp)
            target_link_libraries(${PROJECT_NAME} ${QPANDA_LIBRARIES})
        endif (QPANDA_FOUND)




最后，编译，齐活。

    .. code-block:: c

        $ mkdir build
        $ cd build
        $ cmake .. 
        $ make

运行结果如下:

    .. code-block:: c

        00 : 512
        11 : 488 

