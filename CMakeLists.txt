cmake_minimum_required(VERSION 3.1)
project(test1 VERSION 1.0
              DESCRIPTION "Test project"
              LANGUAGES C)
find_package(MPI REQUIRED)
add_executable(test1 test1.c)
target_link_libraries(test1 PUBLIC MPI::MPI_C)