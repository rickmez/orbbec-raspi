cmake_minimum_required(VERSION 3.5.0)
project(projectName VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

# set directories if needed with: set(<LIBRARY_DIR> "/path/to/lib" )
# example with Open3D set(Open3D_DIR "/home/misc/installing/Open3D")


# use find_package( package REQUIERED)
# example find_package(Open3D REQUIRED)


# include directories with: include_directories if needed

add_executable(projectName main.cpp)

# target_link_librariestarget_link_libraries(projectName Open3D::Open3D)


set_property(TARGET projectName PROPERTY CXX_STANDARD 17)