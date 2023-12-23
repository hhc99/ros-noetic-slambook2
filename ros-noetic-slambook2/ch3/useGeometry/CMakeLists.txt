cmake_minimum_required( VERSION 2.8 )
project( geometry )

# 添加Eigen头文件
include_directories( "/usr/include/eigen3" )

# 编译成可执行文件
add_executable(eigenGeometry eigenGeometry.cpp)
