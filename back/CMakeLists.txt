cmake_minimum_required(VERSION 3.28)
project(back)

set(CMAKE_CXX_STANDARD 23)
set(BOOST_ROOT C:/Users/dimak/Desktop/pluss/project/back/lib/boost_1_85_0)


find_package(Boost REQUIRED)
include_directories(${Boost_INCLUDE_DIRS})
link_directories(/lib/boost_1_85_0/)




add_executable(back main.cpp)
target_link_libraries(back ${Boost_FILESYSTEM_LIBRARY})