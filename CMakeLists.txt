cmake_minimum_required(VERSION 3.3)

project(boost_bind)

add_library(boost_bind INTERFACE)

target_include_directories(boost_bind BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_bind DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
