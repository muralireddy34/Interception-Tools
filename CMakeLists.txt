cmake_minimum_required(VERSION 3.0)

project(interception-tools)

add_executable(udevmon udevmon.cpp)

add_executable(intercept intercept.c)

add_executable(uinput uinput.cpp)

add_executable(mux mux.cpp)

install(TARGETS udevmon RUNTIME DESTINATION bin)
install(TARGETS intercept RUNTIME DESTINATION bin)
install(TARGETS uinput RUNTIME DESTINATION bin)
install(TARGETS mux RUNTIME DESTINATION bin)
