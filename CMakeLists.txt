cmake_minimum_required(VERSION 3.23)

project("CDebug")

add_library(CDebug STATIC cdebug.c)

add_executable(testme testme.c)

target_link_libraries(testme PUBLIC CDebug)