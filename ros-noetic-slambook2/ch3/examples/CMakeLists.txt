include_directories("/usr/include/eigen3")
add_executable(coordinateTransform coordinateTransform.cpp)

# 与Pangolin建立链接
find_package(Pangolin REQUIRED)
include_directories(${Pangolin_INCLUDE_DIRS})
add_executable(plotTrajectory plotTrajectory.cpp)
target_link_libraries(plotTrajectory ${Pangolin_LIBRARIES})# 将plotTrajectory与Pangolin库进行链接
