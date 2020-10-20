cmake_minimum_required(VERSION 3.6)
# 设置项目名称
project(cmake_test)
 
# 设置C++的版本号
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
 
# 搜集当前目录下的源文件
aux_source_directory(. SRCS)

# 生成可执行程序
add_executable(cmake_exec ${SRCS})
target_link_libraries(cmake_exec StaticLib2)