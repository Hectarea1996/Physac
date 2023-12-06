
cmake_minimum_required(VERSION 3.18)

project(physac VERSION 1.1 LANGUAGES CXX)

set(CMAKE_CXX_COMPILER "g++")
# set(CMAKE_CXX_STANDARD 20)

add_library(physac SHARED src/physac.h)
set_target_properties(physac PROPERTIES LINKER_LANGUAGE CXX)

install(FILES src/physac.h DESTINATION include)
install(TARGETS physac DESTINATION lib)
