# CMakeList.txt : CMake project for SFMLRPG, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project ("SFMLRPG")

# Add source to this project's executable.
add_executable (SFMLRPG "main.cpp")



if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET SFMLRPG PROPERTY CXX_STANDARD 20)
endif()

add_subdirectory(dependencies)

# TODO: Add tests and install targets if needed.
