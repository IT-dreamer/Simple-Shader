cmake_minimum_required(VERSION 3.10)
project(Rasterizer)
set(CMAKE_PREFIX_PATH "C:\\Program Files\\vcpkg-master\\installed\\x64-windows\\share")

include_directories(${CMAKE_CURRENT_LIST_DIR}/inc)

set(CPP_FILE "${CMAKE_CURRENT_LIST_DIR}/src/main.cpp" "${CMAKE_CURRENT_LIST_DIR}/src/rasterizer.cpp" "${CMAKE_CURRENT_LIST_DIR}/src/Triangle.cpp" "${CMAKE_CURRENT_LIST_DIR}/src/Texture.cpp")
set(HPP_FILE "${CMAKE_CURRENT_LIST_DIR}/inc/rasterizer.hpp" "${CMAKE_CURRENT_LIST_DIR}/inc/Triangle.hpp")

find_package(OpenCV REQUIRED)
include_directories(${OpenCV_INCLUDE_DIRS})

find_package(EIGEN3 REQUIRED)
include_directories(${EIGEN3_INCLUDE_DIR})

set(CMAKE_CXX_STANDARD 17)

target_link_libraries(Rasterizer ${OpenCV_LIBS})

add_executable(${PROJECT_NAME} ${CPP_FILE} ${HPP_FILE})