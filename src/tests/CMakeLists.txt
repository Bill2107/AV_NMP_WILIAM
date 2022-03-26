cmake_minimum_required(VERSION 3.8)
project(nmp)

set(THIS TESTS)

set(SOURCES 
	Mytest.cpp
)

add_executable(${THIS} ${SOURCES})
target_link_libraries(${THIS} PUBLIC 
	gtest_main
	nmp
)

add_test(
	NAME ${THIS}
	COMMAND ${THIS}
)